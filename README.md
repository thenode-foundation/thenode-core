# TheNode Core integration/staging repository


Quick installation of the TheNode daemon under linux.

Installation of libraries (using root user):

    add-apt-repository ppa:bitcoin/bitcoin -y
    apt-get update
    apt-get install -y build-essential libtool autotools-dev automake pkg-config libssl-dev libevent-dev bsdmainutils
    apt-get install -y libboost-system-dev libboost-filesystem-dev libboost-chrono-dev libboost-program-options-dev libboost-test-dev libboost-thread-dev
    apt-get install -y libdb4.8-dev libdb4.8++-dev

Cloning the repository and compiling (use any user with the sudo group):

    cd
    git clone https://github.com/thenode-foundation/TheNode-core.git
    cd thenode-core
    ./autogen.sh
    ./configure
    sudo make install
    cd src
    sudo strip thenoded
    sudo strip thenode-cli
    sudo strip thenode-tx
    cd ..

Running the daemon:

    thenoded 

Stopping the daemon:

    thenode-cli stop

Demon status:

    thenode-cli getinfo
    thenode-cli mnsync status



More information at [the-node.foundation](https://the-node.foundation)
