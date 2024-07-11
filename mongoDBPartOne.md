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


