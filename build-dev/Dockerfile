FROM python:3.9
LABEL maintainer 'Vanessa <vxreis@gmail.com>'

RUN useradd www && \
    mkdir /app && \
    mkdir /log && \
    chown www /log

USER www
VOLUME /log
WORKDIR /app
EXPOSE 8000 

ENTRYPOINT [ "/usr/local/bin/python" ]
CMD [ "run.py" ]

# docker image build -t ex-build-dev .
# docker container run -it -v C:/learning-docker/build-dev:/app -p 80:8000 --name python-server ex-build-dev

# Com outro container consigo acessar o log
# docker container run -it --volumes-from=python-server estudo cat log/http-server.log