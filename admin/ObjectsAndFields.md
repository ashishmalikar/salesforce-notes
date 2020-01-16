## Fields and Objects in Salesforce

### What is Object in salesforce?
Object can be consider as a database table, to store organizations data.
Object can be of two types: 
 - Standard Object 
 	Standard objects are those objects which are provided by salesforce platform pre build.
 - Custom Object 
 	Custom objects are those created by user	

### How many types of relationships are there in salesforce?
Salesforce object relationship types are as given below:
	- Lookup Relationship
	- Master-Detail Relationship
	- Many-to-many (Junction Object)
	- Hierarchy

#### Master-Detail relationship
In Master-Detail relationship objects are closely tied to each other such that master record(Parent) takes control over certain behavious of detail record(Child).
In Matser-Detail relationship, if we delete Mater record child record will also get deleted.

### Lookup Relationship
Unlike Master-detail, in lookup relationship parent object does not get control over child object, even the parent is get deleted child object will be still there.

### Many-to-Many Relationship
Many-to-Many relationship can be established between two different kinds ob objects. To create Many-to-Many relationship Juntion Object can be used.
Junction object is simply object on which Look-up or master detail of two different object get created and act as a link between two objects.

