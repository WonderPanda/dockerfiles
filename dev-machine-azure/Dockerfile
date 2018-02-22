FROM coderonin/dev-machine-base

RUN echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ xenial main" | \
   tee /etc/apt/sources.list.d/azure-cli.list

RUN apt-key adv --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893 && \
   apt -y install apt-transport-https && \
   apt-get update && apt -y install azure-cli