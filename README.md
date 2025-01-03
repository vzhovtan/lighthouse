### Lighthouse

Lighthouse is initially internal project to build ome kind of knowledge database integrated with 
exisiting infra. MongoDB was the infra-provied data store solution.
It has been modified over time to use standalone external KV storage s DB and Redis selected.
Redis runs as Docker container.

DB file is:
* `lhv4db.json` 
which is complete DB taken from MongoDB, converted to redis-like format and saved in JSON format.

Python apps are starting Redis, taking the local file `lhv4db.json` and starting backend service for API. 
There is no front-end, the backend intended to be used as REST API server.