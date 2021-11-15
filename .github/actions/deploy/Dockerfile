FROM alpine
RUN apk add --update ansible
COPY inventory.yml /.
COPY docker-playbook.yml /.
COPY entrypoint.sh /.
ENTRYPOINT ["entrypoint.sh"]