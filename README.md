# api-todo-1

API example with 1 service with secure key authentication only. (no oAuth. Example is coming).

- Install mfw-cli if not installed yet.
  ```sh
  # npm install @microservice-framework/mfw-cli -g
  ```

- Clone this repo
  ```sh
  # git clone https://github.com/microservice-framework/api-todo-example.git
  Cloning into 'api-todo-example'...
  remote: Counting objects: 9, done.
  remote: Compressing objects: 100% (8/8), done.
  remote: Total 9 (delta 1), reused 5 (delta 1), pack-reused 0
  Unpacking objects: 100% (9/9), done.
  # cd api-todo-example
  ```
  Application folder is a bundle for all services.
  
- Install all services that a part of this bundle
  ```sh
  # mfw setup
	-	downloading microservice-router
	-	downloading example-todo
	-	copiyng example-todo to /Volumes/DATA/gor/test-mfw/api-todo-example/services/example-todo
	-	updating dependencies for example-todo
	-	copiyng microservice-router to /Volumes/DATA/gor/test-mfw/api-todo-example/services/microservice-router
	-	updating dependencies for microservice-router
	[ok]	/Volumes/DATA/gor/test-mfw/api-todo-example/services created.
	[ok]	/Volumes/DATA/gor/test-mfw/api-todo-example/logs created.
	[ok]	/Volumes/DATA/gor/test-mfw/api-todo-example/pids created.
	[ok]	/Volumes/DATA/gor/test-mfw/api-todo-example/configs created.
	[ok]	@microservice-framework/microservice-router updated.
	[ok]	github:microservice-framework/example-todo updated.
	[war]	/Volumes/DATA/gor/test-mfw/api-todo-example already exists.
	[war]	.gitignore already exists  ```

- start all service
  ```sh
  # mfw start all
	-	starting example-todo:start
	-	starting microservice-router:start-admin
	-	starting microservice-router:start-proxy
	[ok]	example-todo:start started
	[ok]	microservice-router:start-admin started
	[ok]	microservice-router:start-proxy started
	[war]	failed to read .env file. Creating default one.
  ```

- open [Example App Page](http://microservice-frame.work/api-todo-example/)
  This page will connect your local API.