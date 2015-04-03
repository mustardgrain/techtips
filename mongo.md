Pretty-Printing
---------------

Add the following line to your `$HOME/.mongorc.js` file to enable pretty print globally by default:

```
DBQuery.prototype._prettyShell = true
```

Searching in Mongo
---------------

To search for a substring in a particular field run the following in the Mongo shell:

```
db.xxxxxx.findOne({"field" : {$regex : ".*string.*"}});
```