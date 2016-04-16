## promise-sqlite3

Forked from `chenqing/co-sqlite3`, removing extraneous stuff.

### Installing

```
npm install promise-sqlite3
```

### Usage

```
const sqlite3 = require('promise-sqlite3');


sqlite3('test.db').then(function(db){
    db.get('SELECT * FROM testtable WHERE id < ? ORDER BY ID DESC ' ,[50])
      .then(function(row) {
        console.log(row);
      });
});
```
