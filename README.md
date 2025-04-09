Area(areaID (PK), areaName, areaLocation)

An area can have many experiences. 

Experience(experienceID (PK), experienceName, experienceCapacity)

Each experience type has an identifier and name. 

(WE) Experience Type (typeID, name)

Every experience has an experience type. 
Many experiences can occur in the same venue. 


Ticket Class (ticketID, className, ticketDescription, price)

Each ticket class is valid for many experiences.


Member(memberID (PK), givenName, surname, emailAddress, dateOfBirth)

If it is a member’s birthday month, their ticket price is reduced. 

Each entry into a member’s purchase history is uniquely identified by the purchase date. The purchase history also stores the points gained.
When a member purchases a ticket, an entry is created into their purchase history and their purchase date is recorded. 
Each role type has an identifier, a description, and a basic pay rate.

Role Type(typeID (PK), ticketDescription, basicPayRayte)

Each seniority level has an identifier, level description, additional pay loading (%).
Each personnel has an identifier, given name, surname, mobile number, email address, and date of birth, and a record of their employment status. 
Each personnel can have many role allocations - these are made up of the role type and seniority level. 
A personnel can have a supervisor, who is another personnel. 
No personnel can have duplicate role allocations
A roster is kept based on a personnel’s role allocation. Each entry is recorded and contains a date, start time, and the duration (hours). 
Each personnel on the roster has an assigned experience. 
Each recommended visit has an identifier, title, description, recommended age group, and thrill level stored.
A recommended visit program can hold many experiences. 
An experience can be part of various recommended visit programs, but does not have to be. 
Each maintenance task has an identifier, description, start date, status, and a staff contact. 
Each maintenance task seeks to repair issues present in one experience but many experiences can require maintenance. 
Personnel can be assigned to a maintenance task as a staff contact.
