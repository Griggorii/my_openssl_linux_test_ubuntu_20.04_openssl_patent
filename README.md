# my_openssl_linux_test_ubuntu_20.04_openssl_patent
openssl , patent , сборка , подходит только надо библиотеки перекинуть не в local , а по стандартному пути и переправить pkgconfig-и тогда возможно можно будет пересобрать

https://github.com/Griggorii/openssl_3.4.3-1_amd64.deb

Ubuntu 20.04 example

openssl_3.4.3-1_amd64.deb inpack data.tar.xz inpack data.tar.xz next /usr/local/lib 

sudo cp -r libcrypto.so libcrypto.so.1.1 libssl.so libssl.so.1.1 /usr/lib/x86_64-linux-gnu

next /usr/local/ssl 

sudo rm -rf /usr/lib/ssl/* && sudo cp -r misc ct_log_list.cnf ct_log_list.cnf.dist openssl.cnf.dist /usr/lib/ssl

Есть дистрибутив который еще пока может собрать openssl и qt4.8.7 взять и распаковать deb->data.tar.xz можно тут https://github.com/Griggorii/qt_4.8-1_amd64.deb этот дистрибутив является фактически золотой жилой за счет того что другие не могут и находится на стадии заморозки крупные компании могут обратиться по покупке на griggorii@gmail.com строить и собирать всякие карты и графы на qt самое то внешний вид очень качественный , я получил такой дистрибутив как ранее говорил методом смешивания ранее такие возможности были , на данный момент это единственный возможно даже в мире дистрибутив который что то устаревшее хоть как то может собрать по причине того что некоторые старые dev пакеты уже почти не найти.
