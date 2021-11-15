FROM alpine
RUN apk add --update ansible
RUN mkdir workdir
WORKDIR /workdir
COPY inventory.yml /workdir
COPY docker-playbook.yml /workdir
COPY entrypoint.sh /workdir
RUN chmod +x /workdir/entrypoint.sh
CMD ["/workdir/entrypoint.sh"]