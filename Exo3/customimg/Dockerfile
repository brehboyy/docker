FROM ubuntu:precise

# Install Armagetron
RUN \
    apt-get update && \
    apt-get install -y python-software-properties && \
    add-apt-repository ppa:armagetronad-dev && \
    apt-get update && \
    apt-get install -y armagetronad-dedicated && \
    service armagetronad-dedicated stop

CMD /usr/games/armagetronad-dedicated

EXPOSE 4534/tcp
