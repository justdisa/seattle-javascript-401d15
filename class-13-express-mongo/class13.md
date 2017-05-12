![cf](http://i.imgur.com/7v5ASc8.png) 13: Mongo and Express
=====================================

## Daily Plan
* Lightning Talks

* Notes:
  * We're writing a lot of code! You'll want to start considering a boiler plate, but don't use it yet!
  * Join me in Lovelace at 11:45a for Adam and Scott to release a quick review of upcoming project week and meet your team.


* Persistence Layer
* Mongo -setup
* Mongoose -setup


## Mongo Resources
* Read [Little MongoDB Book]

## MongoDB
  * **Overview**
    * **MongoDB** is a document based (noSQL) database
    * data is stored as a document with a series of key/value pairs
    * the data structure used to define a **MongoDB** document is referred to as `BSON` (Binary JSON)
    * you can install **MongoDB** through npm by running `npm install mongodb`
    * **MongoDB** runs as a daemon process and has an included shell client for easy database access
      * **start the MongoDB process:** `mongod`
      * **start the MongoDB shell:** `mongo`

## Mongoose
  * **Overview**
    * **Mongoose** provides us with a schema based solution for modeling our application data
    * it provides us with helper methods, validation, queries, and logic hooks to speed up the dev process
    * basic usage:
    ``` javascript
      const mongoose = require('mongoose');
      mongoose.connect(process.env.MONGODB_URI);

      var Note = mongoose.model('Note', { name: String });

      var note = new Note({ name: 'test note' });
      note.save(function(err) {
        if (err) return err;
        console.log('new note created!');
      });
    ```

## Mongo Shell Commands
  * **Commands**
    * `show dbs` - show a list of available databases
    * `use dbname` - switch to a new database
    * `show collections` - show a list of collections from the current database
    * `db.collection.find()` - show all documents in the collection
    * `db.collection.insert({ <data> })` - insert a new document into the collection
    * `db.collection.save()` - insert a new document or update an existing document in the collection

<!-- links -->
[Little MongoDB Book]: http://openmymind.net/2011/3/28/The-Little-MongoDB-Book/

#NOTES#

Going to build a very simple server, routes, and model, and skip over the controller. We will need to apply the whole mongo installation to the project. He will do a shorthand implementation. We will not be able to use the starter code directly.

Need Dirs
+ controller
+ routes
  - routes/notes.js
  1. Function that takes a router when called
    - module.exports = function(router) {
      router.get()
      router.get() => {

      }
      router.post()
      router.put()
      router.delete()
    }
  2.
  3.
  4.
+ server.js
+ models
  - model/note.js
    1. Up until now, we've set up our model as a constructor function
    2. import Mongoose and give it an alias to cut down on typing
    3. const noteItem = Schema({
        note: {type: String, required: true},
        details: {type: String, max: 1048},
        date: {type: Date, default: date.now} //implied required: false
      })
    4. Mongoose and Mongo will take care of the ID for you. We do not need to define the ID.
    5. module.exports = mongoose.mode('note', noteItem) //naming it note and passing in the schema
+ etc
