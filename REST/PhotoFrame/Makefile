build:
	docker build -t photoframe .

start: stop build
	docker run -p 8080:8080 -d photoframe

stop:
	docker ps | grep photoframe | cut -d' ' -f1 | xargs docker kill