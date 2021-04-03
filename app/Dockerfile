FROM andersonpids/bitcoin-nicehash-miner:nheqminer as builder

FROM andersonpids/bitcoin-nicehash-miner:base
LABEL maintainer="apds.anderson@gmail.com"

WORKDIR /app/

COPY --from=builder /app/nheqminer/Linux_cmake/nheqminer_cpu/nheqminer_cpu .
COPY script/ .

CMD ["/bin/bash", "start.sh"]
