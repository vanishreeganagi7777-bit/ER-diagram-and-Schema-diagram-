### Company Data Storage Requirements

TECHIMPACKT:

The company is organized into branches. Each branch has a unique number, a name, and a particular employee who manages it.

The company makes it’s money by selling to clients. Each client has a name and a unique number to identify it.

The foundation of the company is it’s employees. Each employee has a name, birthday, sex, salary and a unique number.

An employee can work for one branch at a time, and each branch will be managed by one of the employees that work there. We’ll also want to keep track of when the current manager started as manager.

An employee can act as a supervisor for other employees at the branch, an employee may also act as the supervisor for employees at other branches. An employee can have at most one supervisor.

A branch may handle a number of clients, with each client having a name and a unique number to identify it. A single client may only be handled by one branch at a time.

Employees can work with clients controlled by their branch to sell them stuff. If nescessary multiple employees can work with the same client. We’ll want to keep track of how many dollars worth of stuff each employee sells to each client they work with.

Many branches will need to work with suppliers to buy inventory. For each supplier we’ll keep track of their name and the type of product they’re selling the branch. A single supplier may supply products to multiple branches.

## ER Diagram:
<img width="1167" height="726" alt="ER diagram" src="https://github.com/user-attachments/assets/c6e6b57f-ee9b-4418-825b-d378581e1e6f" />



## Schema Diagram:
<img width="1619" height="971" alt="schema diagrams" src="https://github.com/user-attachments/assets/82786100-b0c6-4e59-8a64-a9727f0571db" />



## Algorithm:
Algorithm

## Step1: 
	Mapping of Regular Entity Types:
				For each regular entity type create a relation(table) that includes all the simple attributes of the regular entity. 
## Step2:
	Mapping of Weak Entity Types:
				For each weak entity type create a relation (table) that includes all simple attributes of the weak entity.
## Step3:
	Mapping of Binary Relationship Types:
				Include one side of the relationship as a foreign key in the other favor total participation.


## Step4:
	Mapping of Binary(1-N) Relationship Types:
				For each weak entity type create a relation (table) that includes all simple attributes of the weak entity.


## Step5:
	Mapping of Binary(M-N) Relationship Types:
				Create a new relation (table) who's primary key is a combination of both entities primary key's . Also include any relationship attributes.


