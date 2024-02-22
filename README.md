### Lighthouse

Lighthouse uses Redis as key-value store for the DB. Redis run as Docker container.

DB file is:

* `lhv4db.json` 

which is complete DB taken from MongoDB, converted to redis-like format and saved in JSON format.

Python apps are starting Redis, taking the local file `lhv4db.json` and starting backend service for API. There is no front-end, the backend intended to be used as REST API server