# devops-services
3 services for to test devops

# Task 1:

Here we created a Dockerfile for each service and a `docker-compose.yaml file`
Clone the repo to the local and Run `docker-compose up -d --build` on the main directory to run the 3 containers.

Run these commands to test:
- `curl -X POST -H "Content-Type: application/json" -d '{"a": 5, "b": 3}' http://localhost:8081/add` 
- `curl -X POST -H "Content-Type: application/json" -d '{"a": 5, "b": 3}' http://localhost:8082/sub`
- `curl -X POST -H "Content-Type: application/json" -d '{"a": 7, "b": 2}' http://localhost:8083/add-sub`

# Task 2:
- `.github/workflows/node-version-bump.yml` is created to bump up the version of node.js in package.json file of every service on every push to master branch.
- To test it, just add a comment in any file and the version will be updated to next one.

