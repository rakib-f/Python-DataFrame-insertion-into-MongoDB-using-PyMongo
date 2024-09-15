### Python-DataFrame-insertion-into-MongoDB-using-PyMongo
This repository demonstrates how to insert data from a Pandas DataFrame into a MongoDB collection using PyMongo, the Python MongoDB driver. This exercise is useful for developers who want to work with MongoDB databases while using data manipulation capabilities of Pandas.

To run this code, you'll need the following libraries:
- pandas: To create and manage DataFrames.
- pymongo: To interact with MongoDB from Python.

Install these dependencies using the following command:
pip install pandas pymongo

You will also need a local or cloud MongoDB instance. Make sure MongoDB is running on your system.

The code connects to a MongoDB instance using MongoClient. After loading the csv file into a DataFrame using pandas, it converts the DataFrame into a list of dictionaries using to_dict('records'), and then inserts the list of documents into the MongoDB collection using the insert_many() method.
Here, MongoClient uses your MongoDB instance that is running on your machine. You can get the info by executing <mongosh> on the command prompt. Use your database name and the collection name that you want to insert your data into.
