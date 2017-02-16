# aws-ec2-price
REST API for searching price of AWS EC2 instance

Installation 
------------
	go get -u github.com/odg0318/aws-ec2-price

This package requires some dependancies:
* `gin-gonic/gin<https://github.com/gin-gonic/gin>`
* `urfave/cli<https://github.com/urfave/cli>`

Run 
---
	aws-ec2-price --port=[PORT]

Default port is 8080.

Run with Docker
---------------
	make docker-build
	docker run --rm -p 8080:8080 aws-ec2-price:latest 

APIs
----
* GET /ec2/regions/:region/instance_types/:instance_type
