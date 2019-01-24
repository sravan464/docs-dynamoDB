# docs-dynamoDB (wwh (why,what,how))



##### In Dynamo DB we can't create multiple databses in one region, thats why we set the region while using aws-sdk
but we can create multiple tables using (createtable) function
### datatypes in dynamodb

  #### scalar types (only one value)
  ------------
  string,
  number,
  boolean, 
  binary -> blobs of binary data (ex: compressed data, encrypted text,images etc),
  null -> unknown or undefined state
  
  #### set types (set of scalar values)
  ------------ 
  all the elements/attributes in 1 set should be same , these are unordered collections and not empty values allowed 
  ex: set of numbers , set of strings
  
  #### document types (complex structure with nested attributes)
  ------------
  we can nest up to 32 levels deep
  ex: list and map
  
  list -> ordered collection of values , can have multiple data types
  map  -> unordered collectoin of values(key-value pairs) , ideal for storing JSON documents
  
  
#### size  
 any item in the dynamodb is limited to 400kb (here item is object/row(document in mongodb) in the table), each attribute(property/key-value pair) must be under 2kb
 we cannot store empty value in dynamodb (must be atleast 1 character)
