## Lighthouse V4

V4 is improvement of V3 with new frontend, modified DB schema and updated backend
It has been created to accommodate multiple platforms and technology as project is gaining popularity.

There are two frontends are created with JS. Admin one includes functions to update DB, get usage statistics and so on.
This one built with:

* `index.js`

which is main JS file and the entire JS code is split among different JS files to make maintenance easier:

* `index.html`

and

* `index.css`

Are for the admin frontend HTML file. The functionality of the admin frontend has not been changed comparing with V3, it is just updated view.

Second frontend designed to run in Salesforce Lightning platform and using Greasemonkey and Tampermonkey (Salesforce Lightning platform has been released and it is current default app for CX ticketing):

* `lbjb_lite_front_end.js`

Backend file is (the name has been changed to align with internalBDB requirements:

* `init.py`


There is complete DB file taken from MongoDB and saved in JSON format for local testing and further development.

* `lhv4_database.json`
