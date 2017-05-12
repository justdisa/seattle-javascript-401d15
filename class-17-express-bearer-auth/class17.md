![cf](http://i.imgur.com/7v5ASc8.png) 17: Bearer Auth
=====================================

## JSON Web Token Resources
* Read [JSON Web Tokens]

## Bearer Auth
  * **Overview**
    * using standard HTTP, we can use *bearer* auth tokens to access protected resources
    * this token is accessible on the `req.headers.authorization` property and can be split by the term **`Bearer `** to grab the associated token (much like we did with `Basic ` auth yesterday)
    * in our application, this token will used to provide a user with permissions to access specific routes of our choice (ex: `POST: /api/gallery` and `GET: /api/gallery/:id`)

  * **JWT (JSON Web Tokens)**
    * a **JWT** is the standard for securely transmitting information between parties as a JSON object
    * this information is secured through a digital signature
    * we'll be "signing" our **JWT's** through the use of an `APP_SECRET` that we will configure as part of our environment variables

    * **Benefits:**
      * **authentication** - once a user has logged in, each new request will include the JWT - allowing the user to access routes that are permitted with that token
      * **general information exchange** - JWT's are excellent at securely transmitting data between parties - this is often configured using a series of public/private key pairs

## CFGram Visualization
  ![visualization](https://s3-us-west-2.amazonaws.com/s.cdpn.io/154088/cfgram.png)

<!-- links -->
[JSON Web Tokens]: https://scotch.io/tutorials/authenticate-a-node-js-api-with-json-web-tokens


# 17: Bearer Auth

## JSON Web Token Resources

+ Read (https://scotch.io/tutorials/authenticate-a-node-js-api-with-json-web-tokens "JSON Web Tokens")
### Bearer Auth

+ #### Overview
  - using standard HTTP, we can use bearer auth tokens to access protected resources. this token is accessible on the req.headers.authorization property and can be split by the term Bearer to grab the associated token (much like we did with Basic auth yesterday)

  - in our application, this token will used to provide a user with permissions to access specific routes of our choice (ex: POST: /api/gallery and GET: /api/gallery/:id) JWT (JSON Web Tokens)

  - a JWT is the standard for securely transmitting information between parties as a JSON object

  - this information is secured through a digital signature

  - we'll be "signing" our JWT's through the use of an APP_SECRET that we will configure as part of our environment variables

+ #### Benefits:

  + authentication - once a user has logged in, each new request will include the JWT - allowing the user to access routes that are permitted with that token
  + general information exchange - JWT's are excellent at securely transmitting data between parties - this is often configured using a series of public/private key pairs


![CFGram Visualization](https://camo.githubusercontent.com/aa5d50880d556194f8e4e7316cf9184fae0b6cc0/68747470733a2f2f73332d75732d776573742d322e616d617a6f6e6177732e636f6d2f732e6364706e2e696f2f3135343038382f63666772616d2e706e67)

#Notes#

Node has its own native promise library, but bluebird's is better so we require it. We bind that to mongoose. It doesn't have its own promise library, but...
There's no possible way for me to take notes while this is on my screen. Here's where I need to make a resolution to go back and watch these videos later.

I'm a little frustrated.

`req.user._id`
the `_id comes from the schema`


a .env file is a plain text file for us to store our environment variables in.
