FROM debian
LABEL maintainer 'Vanessa <vxreis@gmail.com>'

ARG TESTE_VAR=teste
ENV TESTE_VAR=${TESTE_VAR}

# docker image build --build-arg TESTE_VAR=mudou -t ex-build-arg .
# docker container run --rm ex-build-arg bash -c "echo $TESTE_VAR"