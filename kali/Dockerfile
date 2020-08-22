FROM kalilinux/kali-rolling

RUN apt-get update
# clean up
RUN apt-get upgrade -y

# https://tools.kali.org/kali-metapackages
# RUN apt-get -y install kali-tools-reverse-engineering
# RUN apt-get -y install kali-tools-default
# RUN apt-get -y install kali-tools-top10

# if you want to use 'john'. (for nahammcon - warmup)
# RUN apt-get -y install kali-tools-headless


RUN apt-get -y install \
    git \
    gdb \
    ncat \
    pngcheck \
    python3-pip \
    g++-multilib \
    curl \
    hexedit \
    python3-venv \
    libssl-dev
# RUN apt-get clean && rm -rf /var/cache/apt/archives/* /var/lib/apt/lists/*

# https://linux.die.net/man/1/hexedit

RUN python3 -m pip install --upgrade pip
RUN python3 -m pip install --upgrade git+https://github.com/Gallopsled/pwntools.git@dev
