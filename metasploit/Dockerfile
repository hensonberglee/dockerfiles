FROM r.j3ss.co/kalilinux
LABEL maintainer "Christian Koep <christian.koep@fom-net.de>"

RUN apt-get update && apt-get upgrade -y && apt-get install -y \
    metasploit-framework \
    --no-install-recommends \
    && rm -rf /var/lib/apt/lists/*

COPY start.sh /start.sh

ENTRYPOINT [ "/start.sh" ]
