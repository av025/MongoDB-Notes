# MongoDB "Non Relational Database"

MongoDB is a database management system so we can store data and allow computation on that data do databse management run queries on our data and secure our data.

### The Term Monog means Huge and humgoneous so MongoDB means Huge database or humgoneous database

## The Drwabacks of RDBMS which was overcome by Non-realtional MongoDB was :-

1. **Dynamic Schema**
2. **Huge data was not deal with RDBMS which make computation slower.**  
   3.**The data was only scalable when we can store that data in one machine.**

### In MongoDB we can store huge data and data was natively scalable and have flexible schema.

### MongoDb

#### 1. Document Oriented

#### 2. Stores data in the forms of collections and documents.

#### 3. Gained Popularity in mid 2000's

### Let's discuss how MongoDB Store Data in it.

#### How we stored data in RDBMS

In **RDBMS** we stored data in database and data was store in the form of Tables and **_2D Matrix Table_** where in 2D Matrix we have Rows and Columns and we store data in rows and whole single rows treated as entities.

#### How we stored data in MongoDB

In **MongoDB** here also we stored data in database and we store data in the form of **Collections** and data was repesent in the form of **documentations**.

### Let See Pictorial Representation form of RDBMS and MongoDB

```
              RDBMS                                                       MongoDB
    _______________________________                         ___________________________________
    |          Database            |                        |          Database               |
    |______________________________|                        |_________________________________|
    |   ________________________   |                        |  ____________________________   |
    |   |         Table         |  | <--------------------> |  |     Collection            |  |
    |   |_______________________|  |                        |  |___________________________|  |
    |   |  __________________   |  |                        |  |  ______________________   |  |
    |   |  | Data Stored in  |  |  | <------------------->  |  |  |  Data stored  in   |   |  |
    |   |  |_____Row________ |  |  |                        |  |  |__Documentation_____|   |  |
    |   |  |                 |  |  |                        |  |  |                    |   |  |
    |   |  | ______________  |  |  |                        |  |  |   ______________   |   |  |
    |   |  | | Fileds are  | |  |  | <------------------->  |  |  |  | Fileds are   |  |   |  |
    |   |  | | in the form | |  |  |                        |  |  |  |  saved as    |  |   |  |
    |   |  | | of colums   | |  |  |                        |  |  |  |  originally  |  |   |  |
    |   |  | |_____________| |  |  |                        |  |  |  |______________|  |   |  |
    |   |  |_________________|  |  |                        |  |  |____________________|   |  |
    |   |_______________________|  |                        |  |___________________________|  |
    |______________________________|                        |_________________________________|
```

### Documents Represent Data in MongoDB

Data was represent in the form of **JSON Structure** but originally it was stored in **BSON** which means **Binary Representation of Javascript Object Notation**  
**JSON Structure file was look like Javascript Object but totally it not fully javascript object**

#### In RDBMS our every Data has unique identity which was represent by primary keys similarly in MongoDB here also our data was also has unigue identity which was stored with `_id` which represent our data and stored uniquely.

### Example of JSON File

```json
{
  "_id": {
    "glossary": {
      "title": "example glossary",
      "GlossDiv": {
        "title": "S",
        "GlossList": {
          "GlossEntry": {
            "ID": "SGML",
            "SortAs": "SGML",
            "GlossTerm": "Standard Generalized Markup Language",
            "Acronym": "SGML",
            "Abbrev": "ISO 8879:1986",
            "GlossDef": {
              "para": "A meta-markup language, used to create markup languages such as DocBook.",
              "GlossSeeAlso": ["GML", "XML"]
            },
            "GlossSee": "markup"
          }
        }
      }
    }
  }
}
```

### Collection in MongoDB

Collection was also the same thing like we store our data in RDBMS which was **_table_**. let see example of collection

```css
Example of Collection
________________________________
| {                             |
|   "studentName":"Aayush Vyas" |
|    "studentRollNo.": 01       |
|    "studentClass" : "10th"    |
|  }                            |
|_______________________________|

________________________________
| {                             |
|   "studentName":"Rahul Sharma"|
|    "studentRollNo.": 01       |
|    "studentClass" : "10th"    |
|  }                            |
|_______________________________|

The Collection Of Students which we save in table
```

## Structure of MongoDB

### In our MongoDB Server { which we have when we install mongodb }

### -------> In this MongoDB we have Multiple Database like [Database] {d1 , d2 ,d3, .....}

### -------> Every Database have Multiple Collections like [Collections] {c1, c2, c3, .....}

### -------> In Every Collections we have multiple Documents

### -------> This documents are created with the help of JSON file

## Advantage of MongoDB

### 1. MongoDB give both features of SQL and NOSQL in it

#### We got RDBMS Features to like Tables , Authentication , Relationships and Non-Relational database features are Flexible Schema and scalable Database.

### 2. MongoDB was open source database

#### It was open source database which means it was free for to all not paid for all it comes in two version one was free version and second was supported version which was Paid version.

### 3. MongoDB was Horizontal scalabale

#### Let understand scalability with example

```latex
Case 1 :-
Let you create some website and write schema of that website database and that website deploy on the servers and have users also in the starting of month they have 1000 users on website and website database respond in less time of 10 milli-seconds than at that point we say our website was scalable.

Case 2 :-
Assume that after 6 months our website have user 8000 and if the database  will response now also in 10 milli-seconds or 20 milli-seconds than our website will be scalable if the responds take time upto 2 minutes or more than that than our website was not scalable.

In both case we understand that if the Load become greater than performance of the website was decrease than that website was not scalable or we say that when the load become more on database or data was increase in our database than queries-time was also increase in our database.

So that was Problem with RDBMS based Database management which solve by NO-SQL database which was Mongo DB
```

## How to Scale up things

let see the the method to scale-up the database

### Vertical Scaling

**Vertically scaling was one of the simplest Scaling method of our database but we can scale upto at one point also**  
Let understand vertical scaling with example

```
Assume that you have any dynamic website for which you take database which was 90% full and you known that in some couple of weeks or days that 10% storage of our database was also going to full so we have one option that we go to market and buy some storage to increase our database storage.

Assume that we have 500MB Storage which gona be full than we buy more 500MB storage from the market and place vertically
_________
|_500MB_|  ---> 500 MB
|_500MB_|  ---> 500 MB  = 1000 MB

After some Months this Storage was also gonna full so we buy 500 MB storage
_________
|_500MB_| ----> 500 MB
|_500MB_| ----> 500 MB
|_500MB_| ----> 500 MB = 1500 MB
So our performance was better but cost was also increase so it was costly but we can get benefit at only one points of vertical scaling because at one point the cost become costly but performance was not uptomark.
```

### `The Biggest Concern with Vertical Scaling was we store our all Data only in one Machine if the Machine was got failure so our all data was deleted or destroyed so it have only one point of failure.`

### To overcome Vertical Scaling Challenges we have Horizontal Scale to deal with all challenges.

### Horizontal Scale

Here in Horizontal scale we scale our Database horizontally here we use the concept `Cluster of Machines`.  
Let understand horizontal scaling with example

```
In horizontal Scaling we scale our Database by storing Data in multiple Machines over the network and create cluster of Machines like this :--
                                            _________
             -----------<------------------|__500MB__|-------------->--------------------
        _____|_____                                                                 ____|_____
        |__500MB__|                                                                 |__500MB__|
             |                                                                          |
             |                                                                          |
        _____|_____                                                                 ____|_____
        |__500MB__|                        ___________                              |__500MB_|
             |-------------->-------------|___500MB___|------------>-------------------|

It Solves the Database Scaling Problem because here we use multiple machine to store the data and for our needs we can use multiple machines if the data we use more number of machines or we our data was not that big than we use less machine and these machines are connected through Networks
```

### `MongoDB was also based on Horizontal Scale`

### 4. Data replication

In MonogoDB we can do data replication this is key point if our one machine was not working than on other machine the all data was present there so our data was never deleted.

### 5. Reliable

With the feature of Data replication our MongoDB become reliable.

### 6. Flexible Schema

In the MongoDB we can design Dynamic Schema or we can say flexible schema.

## Usecase of MongoDB

1. **Content Management System** or **"CMS"**
   The Content Management System are Blog Websites etc
2. **Product Data Management System**
   The Product Data Management System are like E-commerce Applications
3. **Operational Intelligence**
4. **Online Application**

### The Thumb-Rule to understand where we have to use MongoDB was

#### 1. Having Structured Data or Unstructured Data means flexible Schema or Fixed Schema we can use MongoDB

#### 2. Having Huge Data than we use MongoDB

#### 3. Want Good performance than also MongoDB is best because it was based on Horizontal Scaling

## Sharding of Data in MongoDB

### The MongoDB was based on Horizontal Scale in horizontal Scaling we scale our data by storing data in multiple Machines by connecting together over the network this was called as `Sharding in the term of MongoDB`.

Let understand Sharding with the help of Example

```
Let Assume you have 60 Thoushands users and you also have 60 thousands Data  which we do Sharding of 20 Thousands in each machine
_____________
|___________|
|___________|          _____________          _______________          ______________
|____60K____| ----->  |____20K_____| ----->   |____20K______| ----->   |_____20K_____| We distributed 60K users through Sharding
```

## Replica Sets in MongoDB

In MongoDB we can dp replication of data from one machine to another machine. mongoDB creates copy of our data in other machine if any system got fail or crash so our data was not destroyed.

```
We can do replication of data in MongoDB
_____________
|___________|
|___________|          ___Data-1___           ____Data-2____           _____Data-3____
|____60K____| ----->  |____20K_____| ----->   |____20K______| ----->   |_____20K_____| We can create replciation of our data
                    |  Copy of Data-3          Copy of Data-1           Copy of Data-2  |
                    |                                                                   |
                    |___________________________________________________________________|---> This machine are called Replica Datasets
If any Machine is down among three data was served from other machine and process was known as Replication of Data
```

### `With the feature of Sharding and Replica Sets the MongoDB becomes Highly Scalable`

## How mongoDB store Data in it

We store Data in the form of **Document** and this document are look like **JSON** but actually it was not json it was **`BSON`** means
**`Binary Representation of Javascript Object Notation`**

### Advantages of BSON Document Data :-

1. **This Document data was take less storage in database to store.**
2. **In the form of docuement and taking less storage so it has fast traversal**
3. **Due to Fast traversal the queries speed was also improve and faster that result good performance**
4. **JSON will support some number of Datatype like Strings , value only but BSON supports Huge number of Datatypes for data.**

### Limitation of BSON Document Data :-

**`We can store data in our BSON Document upto 16MB not above that and it was limitation of our MonogoDB`**

## Data Modeling in MongoDB

```
                                          Data Modeling in MongoDB
                             ------------------------|-----------------------------
                             |                                                    |
                         Entities                                               Relationship
```

#### We do two things in Data Modeling first was create Entities with the help of **`BSON Document`** and create relationship between Entieties `in MongoDB creating relationship was complex things`.

## Types of Relationships

#### 1. One to One Relationship.

#### 2. One to Many Relationship and we can mirror this relationship than another relationship was made which was Many to One Relationship.

#### 3. Many to Many Relationship.

#### 4. Many to Many Relationship.

### In MongoDB there was two ways to create relationship with entities.

### 1. Embeded Document

When we nested our Data into data than it was called as Embeded Document let understand with example :-

```json
User-data document
{
    "_id": <objectidOne>,
    "userName":"Aayush",
    "userLastName":"Vyas"

}
```

```json
user-contact document
{
    "userContactNumber":919644066282,
    "userHouseNumber":"Shri Nagar Extension",
    "userState":"Madhya-pradesh",
    "userCity": "Indore"
}
```

```json
user-education document
{
"userGradutate":true,
"userDegree":"B.Tech in Information Technology"
}
```

**`Now we can embeded or nested this user-contact and use-education in our user-data document this was Embeded Data`**

```json
{
    "_id": <objectidOne>,
    "userName":"Aayush",
    "userLastName":"Vyas",
    "contact": {
         "userContactNumber":919644066282,
         "userHouseNumber":"Shri Nagar Extension",
         "userState":"Madhya-pradesh",
         "userCity": "Indore"
    },
                
   "education" : {
         "userGradutate":true,
         "userDegree":"B.Tech in Information Technology"

   }
}
```
**`When one document inside one document which was also called nesting this was called Embeded Data`**

### 2. Reference Data 
We can give reference of documents in other documents this was the second way to create relationships in mongoDB let understand with example :- 

```json
User-data document
{
    "_id": <objectidOne>,
    "userName":"Aayush",
    "userLastName":"Vyas"

}
```

```json 
user-contact document
{   
    "_id" : <objectidTwo>
    "userContactNumber":919644066282,
    "userHouseNumber":"Shri Nagar Extension",
    "userState":"Madhya-pradesh",
    "userCity": "Indore"
}
```
```json
user-education document
{
  "_id":<objectidThree>
  "userGradutate":true,
   "userDegree":"B.Tech in Information Technology"
}
```
**``We can give reference of user-education and user-contact document in a user-data document``**  
```json
{
    "_id": <objectidOne>,
    "userName":"Aayush",
    "userLastName":"Vyas",
    "user-contact":<objectidTwo>,
    "user-education":<objectidThree>

}
// Here we give reference of other document in a document 
```
### Advantage of Embeded Data and Reference Data Relationship 
#### 1. Faster queries and good performance because data was stored in one big document file with this both method so all data was fetch from single query.
#### 2. Document type Stored data so easy to create.
#### 3. Easy to maintain Transcation.

### Challenges of Limitation of This Embeded Data and Reference Data Relationship are :- 
#### 1. Embeding of to much data can reach exceed of document storage capacity of BSON file we can store upto only 16MB of Data in BSON file.
#### 2. Whole Data was fetch from database or Excess of data loaded every time when we don't want that data so it was also called Eager loading and it lead to network overload and database overload.

### Solution to Overcome with this solution are :- 
#### 1. Create Small doucments so it was not exceed the maximum data-size of BSON File which was 16MB.
#### 2. Do Lazy loading means load only that data which we needed if after that the data more needed than use reference to load those data also.

### The Reference data was normalize data and embeded Data was De-Normalize data.

### The Solutions some more challenges are come which are :-- 
#### Which are queries are slower because our documents are in mulitple Small files so it take some miliseconds time to do computation because we run muliple query over the multiple documents.
#### Nowadays New Version of MongoDB have also feature to do transcation on multiple documents also but it was complicated.

# Practicle Part of MongoDB 

### To Use MongoDB Database we need two things to install first
- **MongoDB Installer to install mongoDB Database in our Machine.**
- **MongoDB Shell installer The MongoDB Shell (mongosh) is an interactive JavaScript shell used to interact with MongoDB instances. It provides a way to connect to your MongoDB database server, query and manipulate data, and perform administrative operations.** 

## Commands to use MongoDB Database 

### Invoke MongoDB Shell 
We have to invoke mongodb shell because it work as admistrator and we can interact with MongoDB instances and with the help of this **`mongosh`** it help to connect to your MongoDB database server , query and manipulate data and perform administrative operations.  
**`We use CMD "Command Prompt to Create MongoDB shell`**
```cmd
cmd: mongosh
``` 

### How to show all database in our mongodb 
The command to show all the database of our mongoDB was **`show databases ;`** or **`show dbs`**
```cmd
<test>: show databases;
<text>: show dbs;
```
### `We have to know that only those database was show who has data in it.` 

### How to switch to use other Database which was present in MongoDB
The command to switch to use other database was present in MongoDB was  
```cmd
<text>: use <database-name>;
```
### `We "use" command to switch to other databases in MongoDB`

### How we create new Database in mongoDB 
We again use **`use command`** to create new database in mongoDB  
```cmd
<text>: use <New-Database-Name>
``` 
### `To create New Database we use "use command" ` 

## Commands on Collection 

### What all the things we can do with collections
1. List all the collection.  **`READ`**
2. Create a new collection.  **`CREATE`**
3. Update the name of collection. **`UPDATE`**  
4. Remove the collection.   **`DELETE`**  

### 1. List all the Collections
We want to see all the collections in our Database of MongoDB Server, So we use this command  
```
<test>: show collections
```
### 2. Create a new Collection
For creating  new collection in current Database we use this command :-
```
<test>: db.createCollection("students");
``` 
### `The command was db.createCollection("students"); in which db was indicate to cureent directory database in our case which was test and after that command .createCollection("students") was help to create collection of students` 

### 3. Update the name of Collection 
To rename the name of collection we use this command :-   
```
<test> : db.currentName.renameCollection("New Name of Collection ");
```
### ` Let understand this command with example  in above example we create new collection which name was students so we write to change collection name like this "db.students.renameCollection("college_students") and here also db represent current database.`  

## `Both the command of create collection , rename collection will give output which was {ok : 1} which means succesfull` 

### 4. Remove the Collection 
We see two commands to delete collection from our Database first we deprecated command and than new command 

#### `Deprecated command `
```
<test> : db.nameOfCollection.removeCollection({ });
```
With the help of this we can delete or remove the collection of our Database one or more than one but now it was `deprecated`.

#### `There was another command to remove or collection let see that also `
```
<test> : db.nameOfCollection.drop( );
```
We can remove the collection with this `drop command` also. 

## Commands on Documents 

### What was the things we do from documents 
1. First was We can insert the Data. **`CREATE`**
2. Second was we can querey that data. **`READ`**
3. Third was we can update the data. **`UPDATE`**
4. Fourth was we can delete the data. **`DELETE`**  

### `We are create document data of "BSON" which look like JSON `

#### Lets create Data to insert in our new collection 
```json
var user = {
    "userName":"Aayush Vyas",
    "userIP":"27.0.0.0",
    "userLogInTime": "8:30PM"

}
``` 

#### We have to insert this user data in new created collection  for that we have shortcut command to do that.
```json
 userInformationDatabase> db.students.insertOne(user); // The Command to insert the data in our  collections

 // Output of above command to insert data and got insertedId
{
  acknowledged: true,
  insertedId: ObjectId('66901f13daffd4e57cc4e49b')
}
```
### `With the help of this command db.students.insertOne( ) we can insert the data.`

#### What if we want to insert multiple documents in our Collection.
```json
userInformationDatabase> db.students.insertMany([{userName:"Sheetal Armani", userIP:"127.0.0.1"},{userName:"Armaan Khan", userIP:"127.0.1.0",hobby:"Singing"}]); // The Command To insert many documents

// Output of inserted BSON Documents with it ObjectId
{
  acknowledged: true,
  insertedIds: {
    '0': ObjectId('66902206daffd4e57cc4e49c'),
    '1': ObjectId('66902206daffd4e57cc4e49d')
  }
}
```
### `In this command  db.students.insertMany([{ },{ } ,{ }])we enter the arrays of document to insert multiple BSON documnets`

### `Now we want to run query on our data or we say fetch "READ" the data from database`
To run query on our data we use this given command  :-
```json
test> db.students.find();  // The simplest query to run over our data to fetch information from Database

// Output of Query was.....
[
  {
    _id: ObjectId('669024a5daffd4e57cc4e49e'),
    userName: 'Aayush Vyas',
    userIP: '27.0.0.0',
    userLogInTime: '8:30PM'
  },
  {
    _id: ObjectId('669024d2daffd4e57cc4e49f'),
    userName: 'Sheetal Armani',
    userIP: '127.0.0.1'
  },
  {
    _id: ObjectId('669024d2daffd4e57cc4e4a0'),
    userName: 'Armaan Khan',
    userIP: '127.0.1.0',
    hobby: 'Singing'
  }
]
```
### We don't want whole data only want specific data from our Collections than we can add filter also to our query .....
To add filter option in our query we can pass specific key-pair value in json format inside the find( ) command query 
```json
test > db.students.find({userName:"Aayush Vyas"}) //Here we pass the specific key-pair value to add filter in it.

// The Output of the filter query was :-
students> db.students.find({userName:"Aayush Vyas"});
[
  {
    _id: ObjectId('669024a5daffd4e57cc4e49e'),
    userName: 'Aayush Vyas',
    userIP: '27.0.0.0',
    userLogInTime: '8:30PM'
  }
]
```

### How we Query Nested Documents let see with example 
**Creating Nested Documents**  
```json 
Creating userFullInformation document 

{
  userName: 'Aayush Vyas',
  userAge: 25,
  userAddress: {
    userHouseNumber: '315 Shri Nagar Extension Near Kalindi Park ',
    userCity: 'Indore',
    userState: 'Madhya Pradesh',
    userCountry: 'India'
  }
}
```
#### Let insert it in our collection students
```json
test > db.students.insertOne(); // Insert the BSON Document inside students collections 

// It returns with Objectid 
{
    _id: ObjectId('66902bacdaffd4e57cc4e4a1'),
    userName: 'Aayush Vyas',
    userAge: 25,
    userAddress: {
      userHouseNumber: '315 Shri Nagar Extension Near Kalindi Park ',
      userCity: 'Indore',
      userState: 'Madhya Pradesh',
      userCountry: 'India'
    }
  }
``` 

### Now we want to find query on the basis of userCity here also we want to add filter....
```json
test> db.students.find({"userAddress.userCity":"Indore"}); // Here we can again filter on the base of userCity

// The Output of the query was 
[
  {
    _id: ObjectId('66902bacdaffd4e57cc4e4a1'),
    userName: 'Aayush Vyas',
    userAge: 25,
    userAddress: {
      userHouseNumber: '315 Shri Nagar Extension Near Kalindi Park ',
      userCity: 'Indore',
      userState: 'Madhya Pradesh',
      userCountry: 'India'
    }
  }
]
``` 

## When we don't know the exact keyword we want to find in this scenario we use Regex or Regular Expression to do query search.

**Asume that we have to find the  keyword which Start from S and we forget the keyword so here we use Regex to find that Keyword**  
```json
test> db.students.find({userName:/S.*/}); // Here we use regular expression aka Regex that the keyword Start from S query on First Character S and return the fetch Data 

// The Fetch Data from our DB was 
[
  {
    _id: ObjectId('669024d2daffd4e57cc4e49f'),
    userName: 'Sheetal Armani',
    userIP: '127.0.0.1'
  }
]
```

### We can limit our Documents also if the Documents are more in the collections so our loading all data will not disturb efficency and performance also.
For limiting our documents to fetch the data we use this command :- 
```json 
test> db.students.find().limit(2); // So we limit our documents that only 2 documents are fetch from our DB
```

### We want that our BSON document was seen in formatted perfectly...
In previous version of MonogDB the our Documents are seen in one line not formatted properly so we use preety command for that but in new versions of MongoDB  they was defaulty formatted properly.
```
test> db.students.find().pretty();
``` 
### We want to Skip some documents in our collection 
Now if we want to skip our documents in our collection than we have to use skip command to skip the documents according to sequence number assume that we want to skip 1 numbers of documents so it skip one documents from our all documents of BSON file of our collections.

```json
test> db.students.find().skip(1); // Here we skip our documents by 1 

// The output was of skiping documents are :- 
[
  {
    _id: ObjectId('669024d2daffd4e57cc4e49f'),
    userName: 'Sheetal Armani',
    userIP: '127.0.0.1'
  },
  {
    _id: ObjectId('669024d2daffd4e57cc4e4a0'),
    userName: 'Armaan Khan',
    userIP: '127.0.1.0',
    hobby: 'Singing'
  },
  {
    _id: ObjectId('66902bacdaffd4e57cc4e4a1'),
    userName: 'Aayush Vyas',
    userAge: 25,
    userAddress: {
      userHouseNumber: '315 Shri Nagar Extension Near Kalindi Park ',
      userCity: 'Indore',
      userState: 'Madhya Pradesh',
      userCountry: 'India'
    }
  }
]
```

### We can sort our Documents in the Ascending and Descending Order on the particular fields
We can sort our documents in the Ascending and descending order on the particular fields let see command with the help of example
```json 
test > db.students.find().sort({userName:1}); // Here we use sort command on the basis of userName in our document and give them value 1 in sort method which means it sorted in Ascending order 

// Output was 
[
  {
    _id: ObjectId('669024a5daffd4e57cc4e49e'),
    userName: 'Aayush Vyas',
    userIP: '27.0.0.0',
    userLogInTime: '8:30PM'
  },
  {
    _id: ObjectId('66902bacdaffd4e57cc4e4a1'),
    userName: 'Aayush Vyas',
    userAge: 25,
    userAddress: {
      userHouseNumber: '315 Shri Nagar Extension Near Kalindi Park ',
      userCity: 'Indore',
      userState: 'Madhya Pradesh',
      userCountry: 'India'
    }
  },
  {
    _id: ObjectId('669024d2daffd4e57cc4e4a0'),
    userName: 'Armaan Khan',
    userIP: '127.0.1.0',
    hobby: 'Singing'
  },
  {
    _id: ObjectId('669024d2daffd4e57cc4e49f'),
    userName: 'Sheetal Armani',
    userIP: '127.0.0.1'
  }
]

// Now in Descending order we have to give -1 in sort method 
test > db.students.find().sort({userName:-1});

// Output was 
[
  {
    _id: ObjectId('669024d2daffd4e57cc4e49f'),
    userName: 'Sheetal Armani',
    userIP: '127.0.0.1'
  },
  {
    _id: ObjectId('669024d2daffd4e57cc4e4a0'),
    userName: 'Armaan Khan',
    userIP: '127.0.1.0',
    hobby: 'Singing'
  },
  {
    _id: ObjectId('669024a5daffd4e57cc4e49e'),
    userName: 'Aayush Vyas',
    userIP: '27.0.0.0',
    userLogInTime: '8:30PM'
  },
  {
    _id: ObjectId('66902bacdaffd4e57cc4e4a1'),
    userName: 'Aayush Vyas',
    userAge: 25,
    userAddress: {
      userHouseNumber: '315 Shri Nagar Extension Near Kalindi Park ',
      userCity: 'Indore',
      userState: 'Madhya Pradesh',
      userCountry: 'India'
    }
  }
]
```

### Now we want to count how much documents are in our collection than.... 
To find the count of documents in our collections than we use count query to find total document in our collection 
```json
test> db.students.find().count(); // With the help of this query we can find total number of document

// Output was 
4
``` 

### Now if we have same data in our DB multiple Time but we have to find only one desired data from our Database than ... 
Assume in our DB we have multiple same userName Data and we want the one particular data from our Database or we want only distinct data it means total number of different values regardless how many times it appears in the dataset than we use distinct command 

```json
test > db.students.distinct("userName"); // to find distinct data 
//It give array of distinct userName as a output
[ 'Aayush Vyas', 'Armaan Khan', 'Sheetal Armani' ]
```
### To Find Distinct Data from Nested Object was 
```json
test > db.collectionOfMessages.distinct("messages.comments"); // For Nested Object distinct Data we do this...
```

## Mathematical Operation on Our Database 
#### We can do mathematical operations query on our Database according to our needs  
#### let assume that we have collection which name was employeeRecords in which we have to find some data on the basis of Salary  

### Greater than 
```json 
// let see syntax first of greater than 
test > db.collection-name.find({ field : {$gt : 20000}});  // We create operator of greater than with the help of dollar sign "$"

// Example of our query 
employeeDatabase> db.employeeRecords.find({ salary : {$gt :20000}});
```
### Greater than equal 
```json
test> db.collection-name.find({filed : {$gte: 15000}}); // We create operator of greater than equal with the help of dollar sign "$"

// Example of our query 
employeeDatabase> db.employeeRecords.find({salary : {$gte : 15000}});
```
### Less than 
```json
// let see syntax first of less than 
test > db.collection-name.find({ field  : {$lt : 20000}}); // We create operator of less than with the help of dollar sign "$" 

// Example of our query 
employeeDatabase> db.employeeRecords.find({salary : {$lt : 20000}});
```
### less than equal 
```json 
// let see synatx first of less than eqaul 
test > db.collection-name.find({field :{$lte : 15000}}); // We create operator of less than equal with the help of dollar sign "$"

// Example of our query 
employeeDatabase> db.employeeRecords.find({salary : {$lte : 15000}});
```
### Not Equal to 
```json 
// let see syntax first of Not Equal to 
test > db.collection-name.find({field {$ne : 3000 / "In Some Operator String was also accepted"}});

// Example of our query 
employeeDatabase > db.employeeRecords.find({salary : {$ne: 20000}}); // So this query give salary of employeee which was not equal to 20 Thousands 
employeeDatabase > db.employeeRecords.find({userName : {$ne : "Armaan"}}); // So this query give userName which was not Armaan khan this not-equal query work on Strings.
```

### In Query 
**In Query will work as OR operator of programming language we can pass array of values from our field and it match with that it give data from our database.**  
```json 
// let see syntax first of In Query 
test > db.collection-name.find({field : {$in :[values of array]}});

// let assume we find the data of employee who's birth year lies in given value 
employeeDatabase> db.employeeRecords.find({dateOfBirth : {$in : [1995 , 1997 , 2001]}});
```

### All Query 
**All Query will work Like AND operator of programming language we can pass array of values from our field and if the value was match with that given field than only it give data from database otherwise not.**
```json 
// let see synatx first of All Query 
test > db.collection-name.find({ field : {$all :[values of array]}}) // If the values match it give data from our Data otherwise not...

// let assume here also we find the data of employee who's birth year was 1995 and 1999
employeeDatabase> db.employeeRecords.find({ dateOfBirth :{$all : [1995 , 1999]}});
```
### `We create mathematical operator through dollar sign "$"`

## Update Queries 
### Let see update queries how to update our data :- 

### updateOne Query 
With the help of this query we can update only one document of our collection.
```json
// let see syntax first 
test > db.collection-name.updateOne.({field: "value"}, {$set : {givenField: "new-value" or newField:"new-value"}});
// With the help of $set operator we can set new fileds or change the value of current filed

// Example 
employeeDatabase > db.employeeRecords.updateOne({employeeName:"Ayush Vyas"}, {$set : {employeeName:"Aayush Vyas"}}); 
// It change only first Value 
employeeDataBase > db.employeeRecords.updateOne({employeeName:"Aayush Vyas"}, {$set : {employeName:"Aayush Vyas"}});
// Create the new filed
``` 

### We have to do increment to our value 
For increment we use $inc operator  
```json
// let see synatx first
test > db.collection-name.updateOne.({field:"value"}, {$inc : {number : 1}});

// Example 
employeeDatabase > db.employeeRecords.updateOne({salary:2000}, {$inc: {salary : 5000}});
``` 

### Now in our document we have array and we have to push data in it than ......
For pushing data in array we use $push operator 
```json 
// let see syntax first 
test > db.collection-name.updateOne.({_idOfDocument:"id"}, {$push :{number : 6}}) // Here the syntax and example of push data in array of our database.
```

### If we want to update multiple Documents than we use this command 
```json
test > db.collection-name.update({field:"Value"}, {$set : {filed:"new-value"} or {new-filed:"new-value"}}, {upsert : true}); // We can update multiple Documents with this command
```

## Deletion Queries 
Now we see Deletion queries in our MonogoDB  

### When we have to delete only one document  or key-pair value from our document
To delete only one document or  key-pair value from our document
```json
test> db.collection-name.deleteOne( {
    // Here we have write which data we have to delete or search 
    "_id":"onject-id",
    // or key-pair value 
    "userName": "xyz"
})
```  

### If we want to delete multiple documents or key pair value than we use this coomand
```json
test> db.collection-name.deleteMany({filed-for-search-filter: {$in/all : [values in array]}});
```
