How to:

1) Install Nodejs and Mongodb on your system.
2) Run "npm install" on root directory.
3) Run "node server.js" on root directory.
4) Test locally the app by entering "localhost:3001/musicians" on any browser.
5) Test updates locally with, ie:

curl -i -X PUT -H 'Content-Type: application/json' -d '{"band": "BBQ Brawlers"}' http://localhost:3001/musicians/535fe13ac688500000c2b28b

Where "band" is the field to update, "BBQ Brawlers" is the value to update, and 535fe13ac688500000c2b28b is the id of the document to update.

6) Test add locally with, ie:

curl -i -X POST -H 'Content-Type: application/json' -d '{"name": "Joe", "band": "Abita Boys", "instrument":"voice"}' http://localhost:3001/musicians

7) Test delete locally with, ie:

curl -i -X DELETE http://localhost:3001/musicians/535feac1cc539500000a209f
