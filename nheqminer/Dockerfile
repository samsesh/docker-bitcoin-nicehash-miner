FROM andersonpids/bitcoin-nicehash-miner:base
LABEL maintainer="apds.anderson@gmail.com"

RUN git clone -b Linux https://github.com/nicehash/nheqminer.git --depth=1

RUN cd nheqminer/cpu_xenoncat/Linux/asm/ \
    && sh assemble.sh \
    && cd ../../../Linux_cmake/nheqminer_cpu \
    && cmake . \
    && make -j $(nproc)
