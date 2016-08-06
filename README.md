# Core-Data
![1](https://cloud.githubusercontent.com/assets/19565981/17454394/4c96358e-5bb1-11e6-92e0-375a36ec87eb.png)

## Core Data
* In April 2005, Apple realesed Mac OSX version 10.4, which was the first to support the **Core Data** framework.
* Core Data is the framework that allow developers store(or retrieve) data in database in object oriented way.
* Core Data is an **ORM(Object Relational Model)** which creates a layer between database and UI.
* Core Data just work with the ORM and let ORM handles the backend.
* It speed up the process of interaction as we don't have to write queries.
* For save or retrieval of large data, programmers recomended to use core dat beacause of it's abilities to handle the less processing speed of iphone.

There are four main camponent of Core Data.
## Componenets of Core Data

![2](https://cloud.githubusercontent.com/assets/19565981/17454397/6481f836-5bb1-11e6-8868-3ac25c7eb774.png)

### Persistent Object Store:
* SQLite is default persisitent store in Core Data.
* Persistent store object store allow developer to setup different stores of different format like Binary, Custom, XML (OSX only) SQLite.

![3](https://cloud.githubusercontent.com/assets/19565981/17454401/84adcdba-5bb1-11e6-8ef4-42c4baada279.png)

### Persistent Store Co-ordinator:
* As it name indicates, **NSPersistentStoreCoordinator** object persist data to task.
* It is partly responsible to manage different Persisitent Object Stores.
* It handles mapping between Object Model and Persisitent store.

### Managed Object Model:
* Managed Object Model defines the data structure.
* It contains information about the entities of the object graph, what attributes they have and how they relate to each other.
* In XCode, The Managed Object Model is defined in project navigator with the extension **.xcdatamodeld**.
* We can use Visual Editor to define the Entities, their attributes as well as relationships.

### Managed Object Context:
* Managed Object Context is heart of Core Data.
* It manages all Data Objects and their relationships.
* Whenever we need to fetch and save objects in persistent store, Our application talk with **Managed Object Context** first.


Basically, our apllication talk with **Persistent Store** using **Managed Object Context** & we manipulate data using **Managed Object**.

#### Managed object:
- Managed Object represent single entity i.e. a row at table in data.
	* e.g. If we want info about employee whose Employee Id is EMP0067 then this single instance could be retrieve as **Managed Object**.
- Managed Objects are instances of **NSManagedObject** or a subclass of it.


## Core Data Implementation

First create a new Xcode project with template **Single View Application**, At the next screen, enter the name of the project and don’t forget to select the options **Use Core Data** as shown.

![coredata1](https://cloud.githubusercontent.com/assets/19565981/17454405/a0bd5494-5bb1-11e6-97fb-590a93212251.png)

Now go to file with extension .xcdatamodeld i.e. **Managed Object Model(Data model of Core Data)** in project navigator. Open the Data Model by clicking. It will open in Data Model Insepcter as shown below.

![coredata2](https://cloud.githubusercontent.com/assets/19565981/17454409/c1f25218-5bb1-11e6-9045-bc81b1f4647a.png)

Here we can define entities, their attributes and maintain relation between two entities(if more two entities present in Data Model).To create an entity, click the + button in the bottom-left of the editor view and name the entity.

![coredata3](https://cloud.githubusercontent.com/assets/19565981/17454413/f67e4096-5bb1-11e6-8bc8-6f1d5a3c4c57.png)

Once you create a new entity, Click on the + button in the Attributes section to add attributes. Give name to attribute and set the datatype.
### To be continued...
