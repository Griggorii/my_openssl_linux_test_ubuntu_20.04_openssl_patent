# my_openssl_linux_test_ubuntu_20.04_openssl_patent
openssl , patent , сборка , подходит только надо библиотеки перекинуть не в local , а по стандартному пути и переправить pkgconfig-и тогда возможно можно будет пересобрать

https://github.com/Griggorii/openssl_3.4.3-1_amd64.deb

Ubuntu 20.04 example

openssl_3.4.3-1_amd64.deb inpack data.tar.xz inpack data.tar.xz next /usr/local/lib 

sudo cp -r libcrypto.so libcrypto.so.1.1 libssl.so libssl.so.1.1 /usr/lib/x86_64-linux-gnu

next /usr/local/ssl 

sudo rm -rf /usr/lib/ssl/* && sudo cp -r misc ct_log_list.cnf ct_log_list.cnf.dist openssl.cnf.dist /usr/lib/ssl
