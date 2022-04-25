
Data Validation Approach Document
Background:
The purpose of data validation is to ensure a certain level of quality of the final data. Data validation focuses on the quality dimensions related to the ‘structure of the data’, that are accuracy, comparability, coherence, clarity and accessibility.
Definitions:
1.	Accuracy: The general definition of accuracy refers to the measurement of the difference between the ‘target parameter’ and the ‘estimated parameter’.
2.	Coherence and comparability: The general definition of coherence and comparability is that data should be consistent internally, over time and comparable between units within the same organization across regions and countries.
3.	Clarity and accessibility: ‘Accessibility and clarity’ is a quality dimension checked in a data validation process; it is related to the IT formal checks that are performed in order to be able to read without any misunderstanding the data.
Data Validation Process comprises of: 
1.	Validation levels and validation rules:
a)	It is desirable to be able to judge to what extent a data set has been validated (validation level). The validation levels are:
i.	Valid. Lev. 0: consistency with the expected IT structural requirements 
ii.	Valid. Lev. 1: consistency within the data set 
iii.	Valid. Lev. 2: consistency with other data sets within the same domain and within the same data source 
iv.	Valid lev. 3: consistency within the same domain between different data sources 
v.	Valid lev. 4: consistency between separate domains in the same data provider 
vi.	Valid. Lev 5: consistency with data of other data providers.

Graphical representation of validation levels: 



b)	Validation rules are based on various considerations:
i.	Automated versus manual; 
ii.	Objective versus subjective/expert opinion; 
iii.	Structural validation versus content validation; 
iv.	Set being validated: in-field, in-record, cross-record, cross-data set, etc.;
v.	Place in the statistical process: input, throughput, output; 
vi.	Type of validation rule: equality, inequality, logical rule;
Validation rules distinguishes rules to ensure technical integrity of the data file and rules for logical/statistical consistency validation.
Rules to ensure technical integrity of a data file 
•	formal validity of entries (valid data type, field length, characters, numerical range) 
•	presence of an entry
•	no duplicate units
•	all the values in a field of one data set are contained in a field of another data set (for instance contained in a code list): “code list check”
•	each record has a valid number of related records (in a hierarchical file structure): “Cardinality check”
		Rule to ensure logical validation and consistency:
•	Range checks: bounds fixed vs bounds depending on entries in other fields


Data Validation Process Steps:
The data validation process consists of five significant steps.
1)	Detail Plan
It is the most critical step, to create the proper roadmap for data validation. It deals with the overall expectation if there is an issue in source data, then how to resolve that issue? It deals in defining the number of iterations, required during data validation.
2)	Validate the Database
This is responsible for ensuring that all the applicable data is present from source to sink. This step is responsible for determining the number of records, size of data, comparison of source and target based on the data field.
3)	Data Completeness 
	This is to check whether the data is complete or not.

4)	Validate Data Formatting
The main focus is that the data clearly understood in the target system, the end-users should clearly understand data whether it is meeting the business expectation or not. It includes:
•	A data type check confirms that the data entered has the correct data type.
•	A code check ensures that a field is selected from a valid list of values or follows certain formatting rules.
•	A range check will verify whether input data falls within a predefined range.
•	Many data types follow a certain predefined format. A common use case is date columns that are stored in a fixed format like “YYYY-MM-DD” or “DD-MM-YYYY.” A data validation procedure that ensures dates are in the proper format helps maintain consistency across data and through time.
•	A consistency check is a type of logical check that confirms the data’s been entered in a logically consistent way. An example is checking if the subsequent event date is after the preceding event dat.
•	Some data like IDs or e-mail addresses are unique by nature. A database should likely have unique entries on these fields. A uniqueness check ensures that an item is not entered multiple times into a database.

5)	Sampling
Before testing on the large set of data, it is necessary to do sampling. It is essential to do testing on the small amount of data and check if the sample data meets the business requirement, if yes then only proceed with a large set of data. It will also decrease the error rate for data and increase the quality and accuracy of the data.
