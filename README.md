# docker-ocserv

ocserv

## Use:

Get the docker image:

	docker pull ilanyu/ocserv

Start an ocserv instance:

	docker run --restart=always --name ocserv --privileged -p 4443:4443 -p 4443:4443/udp -e "TZ=Asia/Chongqing" -d ilanyu/ocserv

Add user:

	docker exec -ti ocserv ocpasswd -c /etc/ocserv/ocpasswd

Delete user:

	docker exec -ti ocserv ocpasswd -c /etc/ocserv/ocpasswd -d test

