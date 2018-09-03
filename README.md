Generates OpenSSL 1.1.0i for Linux Debian stretch-backports. 
It can be installed it over older (2017) openssl 1.1.0f-x for Stretch.
 
Once inside the source directory:

ln -s debian/patches

quilt --fuzz=1 push -a

dpkg-buildpackage -F -us -uc -T binary-arch,binary-indep

generates:

libssl1.1_1.1.0i-1_amd64.deb
libssl-dev_1.1.0i-1_amd64.deb
openssl_1.1.0i-1_amd64.deb
libssl1.1-dbgsym_1.1.0i-1_amd64.deb
libssl-doc_1.1.0i-1_all.deb
openssl-dbgsym_1.1.0i-1_amd64.deb

UDEBs suitable for debian-installer (d-i)
libcrypto1.1-udeb_1.1.0i-1_amd64.udeb
libssl1.1-udeb_1.1.0i-1_amd64.udeb
