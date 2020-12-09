Generates OpenSSL 1.1.1i for Linux Debian Buster / buster-backports. 
December 08, 2020, Ustream release fix (CVE-2020-1971)
 
After git clone and once inside the source directory:

dpkg-buildpackage -F -us -uc -T binary-arch,binary-indep

generates DEBs:
libssl1.1_1.1.1i-1_amd64.deb
libssl-dev_1.1.1i-1_amd64.deb
openssl_1.1.1i-1_amd64.deb
libssl1.1-dbgsym_1.1.1i-1_amd64.deb
libssl-doc_1.1.1i-1_all.deb
openssl-dbgsym_1.1.1i-1_amd64.deb

and UDEBs suitable for debian-installer (d-i):
libcrypto1.1-udeb_1.1.1i-1_amd64.udeb
libssl1.1-udeb_1.1.1i-1_amd64.udeb

NO WARRANTIES WHATSOEVER!


Huelmati [Enjoy]!
