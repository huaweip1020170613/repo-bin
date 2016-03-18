# repo-bin
Repository of RPM Packages without source

To import this repository:

 dnf install https://github.com/chinese-opendesktop/repo/raw/master/src/chinese-opendesktop-release-23-1.src.rpm

or:

 cat > /etc/yum.repo.d/chinese-opendesktop.repo << EOF
 [chinese-opendesktop]
 name=Chinese-Opendesktop
 baseurl=https://github.com/chinese-opendesktop/repo/raw/master/
 skip_if_unavailable=True
 gpgcheck=0
 sslverify=False
 enabled=1
 
 [chinese-opendesktop-bin]
 name=Chinese-Opendesktop-Binary
 baseurl=https://github.com/chinese-opendesktop/repo-bin/raw/master/
 skip_if_unavailable=True
 gpgcheck=0
 sslverify=False
 enabled=1
 EOF
