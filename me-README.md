-------------
Pre-requisite
-------------
1. setup docker
2. Install pre-requisites, can refer here https://github.com/crosstool-ng/crosstool-ng/blob/master/testing/docker/ubuntu22.04/Dockerfile
3. In case the link not working
apt-get install -y gcc g++ gperf bison flex texinfo help2man make libncurses5-dev \
    python3-dev autoconf automake libtool libtool-bin gawk wget bzip2 xz-utils unzip \
    patch libstdc++6 rsync git meson ninja-build

-------------
build crosstool
-------------
1. git clone
2. run `./bootstrap`
3. `./configure --enable-local`
4. `make`
5. Then, an executable `./ct-ng` should be created
6. `./ct-ng help` to get list of help

