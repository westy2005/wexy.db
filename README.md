<br>

## Yüklemek İçin
```npm
npm install  wexy.db
```

# Uyarı || Warning
- Node sürümü 14 gereklidir.
- Node version 14 is required

## Nasıl Kullanılır? || how to use?
# TypeScript
```typescript
import db from "wexy.db"
```
# JS
```javascript
const { Database } = require("wexy.db");
const  db  = new Database("myDatabase");

// Data set | get
db.set("data1", 1);
db.get("data1");
db.fetch("data1");

// Data exists

db.has("data1");
db.exists("data2");

// Get all data

db.all(5); || db.all();
db.fetchAll(5); || db.fetchAll();

// To JSON

db.toJson(5); || db.toJson();

// Delete data

db.delete("key");
db.deleteAll();

// Get data type

db.type("data1"); // ---> number

// DB Array methods
db.push("array1", 10);
db.pull("array1", 10);
db.arrayHasValue("array1", 10);
db.valueArray();
db.keyArray();

// DB Math metods

db.math("data1","*", 3);
db.add("data1", 10);
db.substr("data1", 5);

// DB Finding methods

db.includes("da");
db.startsWith("da");
db.findAndDelete((key,value) => {
    return key.includes("data");
});

// Infos
console.log(db.size);
console.log(db.totalDBSize);
console.log(Database.DBCollection);


// Destroy DB
db.destroy();
```
## Bana ulaşabileceğiniz yerler. || Bugs report
[Discord](https://discord.gg/PXUDXBew)
