# repo-bin
Repository of RPM Packages without source

To import this repository:

	dnf install https://github.com/chinese-opendesktop/repo-bin/raw/master/src/chinese-opendesktop-bin-release-23-1.src.rpm

or:

	cat > /etc/yum.repos.d/chinese-opendesktop-bin.repo << EOF
	[chinese-opendesktop-bin]
	name=Chinese-Opendesktop-Binary
	baseurl=https://github.com/chinese-opendesktop/repo-bin/raw/master/
	skip_if_unavailable=True
	gpgcheck=0
	sslverify=False
	enabled=1
	EOF
