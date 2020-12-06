# Data :bar_chart: Generator Application/Utility In Python
This Application is for generating any kind of dummy/random data in csv,json,xml format.

## Benifits
- This Application is really useful for those who want to play with data without touching the actual/production data.
- This Application or utility helpful in generating any kind of dummy data like csv,json,xml.
- We can prepare test data set using this application, which helpful in development/testing phase.
- This application is modularize you can extend as per your need.

## Configuration of Application :white_check_mark:
In resource folder there is one configuation file(input_info.json).
This file having two main key:
 * [*data_info*] : This is having all fields/columns  and its value related information need to be generated.
 * [*meta_info*] : This is having informations as following:
              1. No. of rows
              2. data generation location.
              3. file format in which data need to be generate.

## Sample Configuation Example
### For String Field
```bash
		      {
			"var_name": "emp_name", //This field is for column name
			"var_type": "str", //This is for defining data type like String.
			"var_constraint": {
				"prefix": "Mr.", //This field is for if you required any prefix in String.
				"suffix": "*",  //This field is for if you required any sufix in String.
				"min_len": 3, //This field is for String min length.
				"max_len": 10, //This field is for String max length.
				"allow_null": true, //This field is for any null value.
				"default": [] //Configure when you only want specific value in generation of data instead of above.
			}
```

### For Integer Field
```bash
		      {
			"var_name": "emp_id", //This field is for column name
			"var_type": "int", //This is for defining data type like Integer
			"var_constraint": {
				"start_range": 1, //This field is for Starting value.
				"incremental_by": 1, //This field is for increment by value.
				"end_range": 50000,//This field is for end of value.
				"default": [1,2,3] //Configure when you only want specific random value in generation of data instead of above.
			}
```

### For Boolean Field
```bash
		     {
			"var_name": "emp_active", //This field is for column name
			"var_type": "bool", //This is for defining data type like Boolean
			"var_constraint": {
				"default": [true] //Configure when you only want specific value in generation of data instead of above.
		     }
```

### For Date/DateTime Field
```bash
		      {
			"var_name": "emp_last_update", //This field is for column name
			"var_type": "datetime", //This is for defining data type like datetime
			"var_constraint": {//Date will be generated in between of start and end datetime range specify below
				"start_date_time": "11/01/2017 00:00:00",
				"end_date_time": "11/10/2019 00:00:00",
				"date_time_format": "%d/%m/%Y %H:%M:%S", // For Date Format
				"default": [] //Configure when you only want specific value in generation of data instead of above.
			}
```

 [sample configuration file refrence!](https://github.com/kapiljain14/Data-Generator-Python/blob/master/resource/input_info.json)
 
 ## For Code Setup
- This project having requirment.txt, which is having all the required liberaries.
- You can use any ide like pycharm or directly configure the requirment.txt file.

## For Code Execution
- First make sure about all requiremnty libraries and python3 installation.
- Configure for the data in resource folder needs tobe setup before perior run.
- In data_gneration module run data_gen_execute.py file for data generation.

## Author✍
[![Linkedin](https://i.stack.imgur.com/gVE0j.png) Kapil Jain](https://www.linkedin.com/in/kapiljain14/)



## Contact
Please write to

:e-mail:
kapiljain14@hotmail.com

 
 

