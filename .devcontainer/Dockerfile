FROM ubuntu:18.04
RUN apt-get update \
    && apt-get install -y --no-install-recommends mysql-client \
    && rm -rf /var/lib/apt/lists/* \
    && apt-get -y update \
    && apt-get -y upgrade \
    && apt-get install -y sqlite3 libsqlite3-dev
ENTRYPOINT ["sqlite"]