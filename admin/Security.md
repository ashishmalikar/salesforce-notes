## Salesforce security model

Salesforc security models, lets you specify the access to the user for certain type of data.
With Salesforce security model one can set which type of data can be accessible by which group of user
also which records can be accessible by which user.

### Different Level of Data Security Access

#### Organization Level Security
For your whole org, you can maintain a list of authorized users, locations, login hours.

#### Object Level Security
Access to object-level data is the simplest thing we can set. By setting Object level security 
one can restrict certain group of user to have access to read, create, edit and delete data.

#### Field Level Security
With Field level security we can restrict access to the certain field.

#### Record Level Security
For object user can have permission but then we can restrict access to records i.e. user can see which data or not.
You can manage record level security in four ways:
- Organization-wide Defaults
- Role Hierarchies
- Sharing Rules
- Manual Sharing