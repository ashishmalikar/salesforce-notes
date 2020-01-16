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

#### Organization-wide Security
Organization-wide security(OWD) is the most baseline data access level. OWD restricts access to the data for most restricted user should have.
OWD used to restrict access. Then you grant access with other means like Shring Rules, Role hierarchies, Sales Teams, Account Teams, and so on.

#### Role Hierarchies
It give access for users higher in the hierarchy to all records owned by users below them in the hierarchy. 
Role hierarchies don’t have to match your organization chart exactly. 
Instead, each role in the hierarchy should represent a level of data access that a user or group of users needs.

#### Difference between a Role and Profile
Roles are one of the ways you can control access to records. They also impact reports (e.g. “My Teams” filter). Roles come into play if your security model (OWDs) are set to private.

Profiles help determine record privileges. Assuming the User can see the record, Profiles determine what the User can do, view or edit on that record. Profiles control other system privileges as well (mass email, export data, etc)

In simple words, Roles are one of the ways you can control access to records and Profiles determine what the User can do, view or edit on that record.

#### Sharing Rules
Sharing Rules are automatic exceptions to organization-wide defaults for particular groups of users, so they can get to records they don’t own or can’t normally see. Sharing rules, like role hierarchies, are only used to give additional users access to records. They can’t be stricter than your organization-wide default settings.

#### Manual sharing
It allows owners of particular records to share them with other users. Although manual sharing isn’t automated like org-wide sharing settings, role hierarchies, or sharing rules, it can be useful in some situations, such as when a recruiter going on vacation needs to temporarily assign ownership of a job application to someone else.

#### Profile
Each user has a single profile that controls which data and features that user has access to. A profile is a collection of settings and permissions. Profile settings determine which data the user can see, and permissions determine what the user can do with that data.
The settings in a user’s profile determine whether she can see a particular app, tab, field, or record type.
The permissions in a user’s profile determine whether she can create or edit records of a given type, run reports, and customize the app.
Profiles usually match up with a user’s job function (for example, system administrator, recruiter, or hiring manager), but you can have profiles for anything that makes sense for your Salesforce org. A profile can be assigned to many users, but a user can have only one profile at a time.

#### Standard profiles
Read Only
Standard User
Marketing User
Contract Manager
System Administrator
 

#### Permission Set?
A permission set is a collection of settings and permissions that give users access to various tools and functions. The settings and permissions in permission sets are also found in profiles, but permission sets extend users’ functional access without changing their profiles.
Permission sets make it easy to grant access to the various apps and custom objects in your org, and to take away access when it’s no longer needed.

Users can have only one profile, but they can have multiple permission sets.

#### “View all” and “Modify all” permission
View all and Modify all permissions are usually given to system administrator. When you grant “View All” or “Modify All” for an object on a profile or permission set, you grant any associated users access to all records of that object regardless of the sharing and security settings.

In essence, the “View All” and “Modify All” permissions ignore the sharing model, role hierarchy, and sharing rules that the “Create,” “Read,” “Edit,” and “Delete” permissions respect. Furthermore, “Modify All” also gives a user the ability to mass transfer, mass update, and mass delete records of that specific object, and approve such records even if the user is not a designated approver.

These tasks are typically reserved for administrators, but because “View All” and “Modify All” let us selectively override the system, responsibilities that are usually reserved for the administrator can be delegated to other users in a highly controlled fashion.
 

#### Is it possible to restrict permission for users using permission set
No, Permission Set always extends the permission. It does not restrict permission to users.
If a user does not have access to a specific record type, will they be able to see the records that have that record type?
Yes, Record type controls only visibility of record on UI but not its access to users. If user does not have access to record type then user will not be able to create records for that record type using UI. But user will we able to see records if they have appropriate permission to do so.
For more details about security questions for Salesforce admin interview questions, refer to my previous post Salesforce security interview questions