## Lighthouse V3

Lighthouse is developed by Cisco CX engineers for engineers providing useful commands and support links to help in troubleshooting.


Lighthouse is internal project and has been created with idea to use Cisco internal REST API back-end aka BDB as a backend and JS as frontend on CSOne, which is ticket handling system in CX. V1 and V2 were created purely with JS and all information has been saved in .txt files.

BDB (Big Data Broker) is internal REST API backend to run custom Python and JS scripts and using MongoDB as database. Current version of Lighthouse utilizes MongoDB and saves data in different collections for different platforms. Each entry in DB represents particular feature as a key and contains troubleshooting information as value in JSON format.

Lighthouse backend built with Python using API to BDB for ingesting data into MongoDB or retrieving the data from database.

There are two frontends are created with JS. Admin one includes functions to update DB, get usage statistics and so on.

This one built with:

* `bdb_add_update_final.html`
* `bdb_admin_final.html`
* `bdb_get_stats_final.html`
* `bdb_guide_final.html`
* `bdb_index_final.html`
* `bdb_user_view_final.html`

Second frontend designed to run in Salesforce CSOne app using Greasemonkey and/or Tampermonkey:

* `lighthouse_v3_frontend_final.js`

Python backendis:

* `lighthouse_v3_backend.py`

There is an additional backends file created to collect statistics of Lighthouse usage and save it in MongoDB:

* `lighthouse_v3_statistics_v2.0.py`
