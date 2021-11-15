FROM alpine
RUN apk add --update ansible
RUN mkdir workdir
WORKDIR /workdir
COPY inventory.yml /workdir
COPY docker-playbook.yml /workdir
COPY entrypoint.sh /workdir
CMD ["/workdir/entrypoint.sh"]