FROM debian:latest

COPY . /debdir
RUN dpkg -i /debdir/*.deb; apt-get install -y -f

CMD ["bash"]
ENTRYPOINT ["proxysql", "-f", "-D", "/var/lib/proxysql"]
