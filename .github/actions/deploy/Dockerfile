FROM alpine
RUN apk add --update ansible
RUN mkdir -p /github/workspace
WORKDIR /github/workspace
COPY inventory.yml /github/workspace/
COPY docker-playbook.yml /github/workspace/
COPY id_rsa-encrypted /github/workspace/
COPY entrypoint.sh /github/workspace/
RUN chmod +x /github/workspace//entrypoint.sh
CMD ["/github/workspace//entrypoint.sh"]