FROM ubuntu:16.04

RUN apt-get -y -qq update && apt-get -qq -y install \
    python3-pip \
    python3-pytest python3-crypto python3-twisted python3-requests python3-yaml
RUN pip3 install --quiet bravado==9.2.2 tornado pymongo==3.6.1 pytest-ordering==0.5 flask

RUN mkdir -p /testing
ENTRYPOINT ["bash", "/testing/run.sh"]
