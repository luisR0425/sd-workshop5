FROM alpine
MAINTAINER luis.rosales@correo.icesi.edu.co

RUN apk update && \
  apk add python &&  \
  apk add wget

RUN wget https://bootstrap.pypa.io/get-pip.py -P /tmp && \
  python /tmp/get-pip.py && \
  pip install flask


ADD sources /tmp

CMD ["/usr/bin/python","/tmp/greedy.py"]
