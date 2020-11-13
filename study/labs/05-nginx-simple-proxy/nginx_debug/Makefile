IMAGE=tbutzer/nginx_debug

build:
	sudo docker build --tag $(IMAGE) .

publish: ## Send this image to docker hub!
	sudo docker login -u tbutzer
	sudo docker push $(IMAGE)

