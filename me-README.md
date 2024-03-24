-------------
note
-------------
reason this branch is called `note-2`
i opened `note` and accidentally created pull request to the original repo
it seems cannot delete the pull request
i afraid making new branch called `note` will make the pull request at the original repo to re-appear again

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
7. If you encoutner problem where you cannot build as root, https://stackoverflow.com/a/53099177/10521815
8. in root, and in the current crosstool directory, run `chown user:user .`
9. `su user`
10. now build the crosstool

