VERSION=0.2
IMAGE_NAME=nginx-display-hostname
DOCKERHUB_USER=raghulmz

build:
	docker image build -t $(IMAGE_NAME):$(VERSION) .
tag: build
	docker tag $(IMAGE_NAME):$(VERSION) $(DOCKERHUB_USER)/$(IMAGE_NAME):$(VERSION)
	docker tag $(IMAGE_NAME):$(VERSION) $(DOCKERHUB_USER)/$(IMAGE_NAME):latest
push: tag
	docker push $(DOCKERHUB_USER)/$(IMAGE_NAME):$(VERSION)
run: build
	docker run -d -p 80:80 $(IMAGE_NAME):$(VERSION)