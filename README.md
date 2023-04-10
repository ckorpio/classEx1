# classEx1
To do in class: File ops in Node.js

This exercise can be run from Codespaces or it can be deployed anywhere on the cloud.

Things to note:

1. The file "exercise1.js" contains a listener which allows the script to interact with a user via a browser. It also contains a couple of routes that demonstrate a few basic things:
  1.1: A default GET route "app.get('/',..." which will provide a basic default response.
  
  1.2: An "app.get('/api/say/:name',..." route which will respond to a apscific request "/api/say" and will use a parameter passed as part of the route, e.g.
 "/api/say/Cris".
 
  1.3: An "app.get('/wfile',..." route which demonstrates how one can access a local file for writing data (submitted as a query string of key-value pairs typical of a GET request) into a local file on the server.
  
  1.4: An example route "app.post('/post/users', function(req, res) {..." which demonstrates the communication of data via a POST request. This request is assumed to come from submitting some form whose handler is this URI endpoint. So if the URL of the app is say, https://server.com/blah/blah/exercise1.js (or whatever URI the app is deployed to), then the form handler would be something like this: https://server.com/blah/blah/exercise1.js/post/users so that the form posts to the above endpoint.
  
2. In the same repository there is also a form "post.html" which posts data to the above route "app.get('/wfile',...". What that form does can also be done with Postman (without importing anything from Github). But if you find Postman confusing you can just use that form where you make sure the "action" attribute is set properly for your URI.

The file "mydata.txt" is just a file that supports the file operations provided as example in "exercise1.js". The "package.json" acts as a sort of "registry" that records build parameters and dependencies required for building and deploying the app.

In order to run this example, you can download the form to your local computer and deploy the app in Codespaces (or wherever else you like). Then when you have a URI for accessing your app via a browser, you can edit the local form to put that URI in the action part of the form, load it on a browser, enter inputs and submit them to the post endpoint of "exercise1.js". Other than this edit of the form, no other editing is needed to run this exercise.
