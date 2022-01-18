# nota_bene_sqlite3_centos
Nota Bene concernant l'utilisation du module sqlite3 sur centos

Ne pas installer sqlite3 via pip install

# Procédure

yum install -y gcc make sqlite-devel zlib-devel libffi-devel openssl-devel
cd Python-3.7.5
sudo ./configure --enable-optimizations --enable-loadable-sqlite-extensions 
sudo make 
sudo make altinstall

# Source

https://github.com/mylar3/mylar3/issues/238
