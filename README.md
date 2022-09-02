# Team_8

## Machine Learning Model - Final Project 2021

## Predicting Housing Prices

* In our final project, our team used Machine Learning Linear Regression as a Data Science and Analytics housing pricing prediction. We hypothesize that the more bedrooms a property has the higher the sale price. The housing data was chosen from Kaggle due the the numerous variables associated with every property that have an effect on the sale price.

## Team Members - Roles
 * Krystle West - Machine Learning Tool Creation Manager (Triangle)
 * Arielle Colasanto- Framework Creation Manager (Circle)
 * Vincent Vinci - Information Manager (Square)
 
 * Meetings every Tuesday and Thursday
 
## Storyboard

[Google Slidesand Storyboard](https://docs.google.com/presentation/d/1wvPNxExDlCJhe1lzaHfo_akHufj1xvtRC4TSMN_8q5g/edit#slide=id.g138bc1f89a1_0_0)

## Resources and DataSets:

* Data Source: `House Prices` were obtained from [Kaggle - Housing Data](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data)
* Software: `Python 3.9`, `Visual Studio Code`, `Anaconda 4.13`, `Jupyter Notebook`, and `Pandas` 

## Data Approach

## SQLite Advantages
While there are a few specific use cases for SQLite, we'll be focusing on how it can be beneficial to you and where you might get the most value from it. The main advantages are:

1. **It's local.** One of the core advantages of SQLite is that it allows you to create databases locally on your computer to support testing and easy prototyping. This is beneficial, because if you want to test something out and you need a database, it's not always the most convenient to set up a SQL database server just to try something out.
2. **There's an app for that.** Another advantage of SQLite databases are that they can be used on a mobile phone app. Most mobile phone games will use an SQLite database to store certain information about you or your players statistics. While we won't be creating a mobile app in this module, it's still helpful to understand the full context.

## SQLite Disadvantages
SQLite also has a couple of disadvantages, however. They are:

1. **It's local.** If you've used a MYSQL database before, you might have noticed that you can have multiple users access the database. With SQLite, there are no users. SQL is local: stored on one computer or phone. So, only that computer or phone will have access.
2. **There are fewer security features:** one other disadvantage to be aware of is that SQLite doesn't have as many security features as a traditional SQL database. While it's not something specifically to be concerned with for this module, just keep that in mind as you create other databases later on.

Good work with SQLite! Now let's move on to SQLAlchemy.

## SQLAlchemy ORM
One of the primary features of SQLAlchemy is the **Object Relational Mapper**, which is commonly referred to as ORM. ORM allows you to create classes in your code that can be mapped to specific tables in a given database. This allows us to create a special type of system called a **decoupled system**.

To understand ORMs and decoupled systems, consider the following scenario. Suppose you are cleaning out the garage, and you find a bunch of wires or ropes that are all knotted together. We would call this a **tightly coupled system:** all of the different ropes are connected to each other, so if we go to grab just one, the whole mess comes along with it. What the ORM does for us is untangle—or decouple—all of those ropes, so we can use just one of them at a time. When we pick one up, we won't pick up the whole knot; or, if one element breaks, it doesn't affect any of the other cords.

Generally speaking, the less coupling in our code, the better. If there are a bunch of relationships between all of your coding components and one of them breaks, everything breaks.

The ORM helps us keep our systems decoupled. We'll get into more specific details about how we can keep our code decoupled, but for now, just remember that your references will be to classes in your code instead of specific tables in the database, and that we'll be able to influence each class independently.

## SQLAlchemy Create Engine
Another really great feature of SQLAlchemy is the `create engine` function. This function's primary purpose is to set up the ability to query a SQLite database. After all, data just sitting in a database that we can't access does us no good.

In order to connect to our SQLite database, we need to use the `create_engine()` function. This function doesn't actually connect to our database; it just prepares the database file to be connected to later on.

This function will typically have one parameter, which is the location of the SQLite database file. Try this function by adding the following line to your code.

````Python
engine = create_engine("sqlite:///********")
````

We've got our engine created—good work! Next we're going to reflect our existing database into a new model with the `automap_base()` function. Reflecting a database into a new model essentially means to transfer the contents of the database into a different structure of data. 

## SQLAlchemy Automap Base
**Automap Base** creates a base class for an automap schema in SQLAlchemy. Basically, it sets up a foundation for us to build on in SQLAlchemy, and by adding it to our code, it will help the rest of our code to function properly.

In order for your code to function properly, you will need to add this line to your code:


````Python
Base = automap_base()
````
### Data Structure

### Data Exploration 

### Data Analysis

[Google Slides](https://docs.google.com/presentation/d/1wvPNxExDlCJhe1lzaHfo_akHufj1xvtRC4TSMN_8q5g/edit#slide=id.g138bc1f89a1_0_0)
