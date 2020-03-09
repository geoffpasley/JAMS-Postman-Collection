# JAMS-Postman-Collection
 Postman Collection for the JAMS REST API

<h2>Usage</h2>
Create an environment with the following variables and populate those variables:
<ul>
  <li><b>username</b></li>
  <li><b>password</b></li>
  <li><b>url</b> (ex. http://YOUR_URL_NAME)</li>
  <li><b>access_token</b>  (LEAVE BLANK)</li>
</ul>

The JAMS REST API relies on a token to process requests. Nearly all requests in these collections depend on the access_token variable. To populate this variable do the following:
<ul>
 <li>Expand the <b>Authentication</b> collection.</li>
 <li>Send the <b>POST api/authentication/login</b> request.</li>
 <li>You should receive a response like this 
   <code>
   {
      "access_token": "RANDOM_TOCKEN_VALUE",
      "expires_in": "43199"
   }
   </code></li>
 <li>Verify the <b>access_token</b> environment variable was successfully populated.</li>
