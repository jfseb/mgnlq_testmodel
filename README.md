# mgnlq_testmodel

test model data
for the mongo db based nlq processing

contains
  1. Mongoose schema  <modelname>.mongooseschema.json
  2. Model documents (which are effectively model data loaded into mongoose)  <modelname>.doc.json
  3. <modelname>.data.json


Filename              |   | comment
----------------------|---|------------
model.json            |   |
<modelname>.doc.json  | Model Documents | data effectively loaded into mongodb  "models" collection
<modelname>.mongooseschema.json |
<modelname>.data.json |   |



## How to use

The data can be uploaded into a mongodb  ("testdb")
via  [mgnlq_model](https://github.com/jfseb/mgnlq_model)

```npm run load_data```

this module is used as reference data in many projects

an alternative source and target name can be specified via:

var mongoConnectionString = process.env.MONGO_DBURL || 'mongodb://localhost/testdb';
var modelPath = process.env.MGNLQ_MODELPATH  || 'node_modules/mgnlq_testmodel/testmodel/';


# history

0.0.5 uri_rank, uri