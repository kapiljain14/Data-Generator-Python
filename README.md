# Data Generator Application/Utility In Python
This Application is for generating any kind of dummy/random data in csv,json,xml format.

## Benifits
- This Application is really useful for those who want to play with data without touching the actual/production data.
- This Application or utility helpful in generating any kind of data like csv,json,xml.
- We can prepare test data set using this application, which helpful in development/testing phase.
- This application is modularize you can extend as per your need.

## Configuration of Application
In resource folder there is one configuation file(input_info.json).
This file having two main key:
1. data_info: This is having all fields/columns  and its value related information need to be generated.
2. meta_info: This is having informations as following:
              1. No. of rows
              2. data generation location.
              3. file format in which data need to be generate.

## Sample Configuation Example
### For String Field
```bash
		      {
			"var_name": "emp_name", //This field is for column name
			"var_type": "str", //This is for defining data type like String
			"var_constraint": {
				"prefix": "Mr.", //This field is for if you required any prefix in String
				"suffix": "*",  //This field is for if you required any sufix in String
				"min_len": 3, //This field is for String min length
				"max_len": 10, //This field is for String max length
				"allow_null": true, //This field is for any null value.
				"default": [] //Configure when you only want specific value in generation of data instead of above
			}
```




