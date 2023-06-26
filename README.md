# CS340

## Module Seven: Project Two
### Allen White



## README

### Changelog:
* Date updated: 6.25.2023 by Allen White (Dash description and screenshots)
* Date updated: 6.4.2023 by Allen White (additional screenshots and functionality)
* Date updated: 5.28.2023 by Allen White (initial commit and description)s
## Background
### Intent – 
This product was developed for Grazioso Salvare by Allen White to allow for easy, intuitive filtering of datasets for animal records.

### Current state – 
The product allows for interaction with the data through a series of filters and interactive visualizations as described below.


## Dashboard Functionality
### Initial State
Description: The application provides an intuitive user interface to select and filter data from the Austin Animal Center Outcomes dataset. Users can select the type of animal to view (limited to cat, dog, or all), view metrics broken down in a pie chart for the current subset of data, see the geographic location for pickup of a single animal, as well as read quick, easy data about the selected animal.

 
![image](https://github.com/Whiteaw2/CS340/assets/20048527/59c52cb0-2ec9-4097-a0e0-f3ddd4e6e39c)


## Animal Type: Dropdown options
Description: Once the ‘Animal Type’ dropdown is selected, the potential large filtering options are seen and can be easily clicked.

 ![image](https://github.com/Whiteaw2/CS340/assets/20048527/a1f6b7c7-3707-4974-8769-f1e9f32e0fdb)


## Animal Type: Cat
Description: Once the animal type of cat is selected, the database is filtered to show only felines. The geolocation chart shows the first animal in the list, but the user can easily click to select a different animal using the radio buttons to the left of the listed animals. The pie chart is updated to reflect the breeds of all cats, and hovering shows the count for each breed. In the future it will be important to handle the small errors such as slight spelling variations which can lead to bloated data.

 ![image](https://github.com/Whiteaw2/CS340/assets/20048527/354e459f-025a-4e63-89cf-0071049d1089)


## Animal Type: Dog
Description: Once ‘Dog’ is selected, the table dynamically adjusts to reflect the filtered data and the geolocation maps reflect the first entry in the table. Also, once selected, the Search and Rescue Type option appears to allow for further filtering.

 ![image](https://github.com/Whiteaw2/CS340/assets/20048527/39495520-42dc-4c0b-badf-e30d094f1aa7)



## Animal Type: Dog
Search and Rescue Type: Mountain or Wilderness
Description: Once a selection is made to further filter the dog data by those who are relevant for various search and rescue types the table and all charts update.

 ![image](https://github.com/Whiteaw2/CS340/assets/20048527/9766e04f-3567-436c-a8ed-04bbbc6ebeb8)



## Animal Type: Dog
Search and Rescue Type: Water
Description: Once a selection is made to further filter the dog data by those who are relevant for various search and rescue types the table and all charts update.

 ![image](https://github.com/Whiteaw2/CS340/assets/20048527/5bea50f0-17df-45af-ae44-25b71678af79)



## Animal Type: Dog
Search and Rescue Type: Disaster Rescue or Individual Tracking
Description: Once a selection is made to further filter the dog data by those who are relevant for various search and rescue types the table and all charts update.

 ![image](https://github.com/Whiteaw2/CS340/assets/20048527/495b3cb1-2635-4f78-bfb3-4d2b8fa5afbf)




## Animal Type: Dog
Search and Rescue Type: Multi 
Description: Multiple Search and Rescue Types can be used to expand the data table search. All tables and charts update to reflect the newly filtered data. 

 ![image](https://github.com/Whiteaw2/CS340/assets/20048527/9ea3fd38-e882-43c8-8026-703074cf73aa)



## Reset
Description: To restore the page to its unfiltered state simply click on ‘Reset’

 ![image](https://github.com/Whiteaw2/CS340/assets/20048527/b6e777c7-6e76-4898-8cd4-ece465aca538)




## Tech Stack
The tools which were used to achieve the required functionality were composed of several core components, the backend, interface layer, and front-end. The backend was created using the NoSQL database MongoDB, which allows for fast, responsive, and secure access and modification to data relevant to the product. The interface layer was created using a custom-developed Mongo Shell Python interface script which provides the ability to Create, Read, Update, and Delete data as needed. This additional level of abstraction adds more responsive controls between the backend and front-end of the product. Lastly, the front-end was created using the Dash framework by Plotly, which is built on the React.js core for responsive, dynamic, front-end interface. The Dash framework generally adheres to the model-view-controller pattern which pertains to the data and interface between the front and backend, the view handles the rendering of the data into an interactable format, and the controller pattern gets and interprets actions from the user. Specifically, within this front-end, there are many traditional components of web design such as HTML div and stylings. The dynamic callback components of the Dash framework allow content and functionality to update based on specific actions performed by the user to provide an intuitive, responsive interaction using Python functions. 
Process
	At a high level, the product was produced by initially configuring and loading the database, after installing all dependencies. Creating the appropriate user account was an important step to ensure security for the product for the near and long term. Next, the interface layer was developed in Python which allowed for easy interaction with and modification of the dataset. This interface layer was developed and tested separately from the front-end to ensure that the core functionality was robust and responsive. Lastly, the front-end layout and functionality were developed and refined based on the client’s needs and considerations for user workflows. While developing the product, it was important to leverage external resources such as the Dash, Python, and Plotly resources, as well as online forums such as Stack Overflow to work through issues.  
Challenges
	During the development effort, it was important to have an understanding of new concepts related to several languages and frameworks. Syntactic errors in Python proved to be a significant issue as did HTML syntax and the interface between these and Dash. Often, it was important to transfer my working code into an IDE such as PyCharm to find errors in the Python syntax. Other issues required research and trialing solutions. While these were challenging at times, persistence, research, and iteration were ultimately the key to success.



## CRUD Python Mongo Interface
Background
Intent - This PyMongo CRUD interface for MongoDB was created as part of a project sponsored by the Grazioso Salvare project in partnership with the Austin Animal Center Outcomes to allow simple, flexible, and effective access through a GUI front-end to a non-relational database to identify rescue dogs who can be trained in various ways for search-and-rescue training based on breed information in existing datasets. The project is open source and encouraged to be used, modified, and shared as needed.
Current state – The project currently allows for dynamic Create, Read, Update, and Delete functionality through the adjustment of variables in a Jupyter Notebook running the “jupyterCallCRUD.py” script, calling the “CRUD.py” module. These rely on Mongosh and MongoDB to function.




## Getting Started
Prerequisites – To use the CRUD interface program, you will need to be running the following supporting programs. I have listed the current approved versions which have been tested, though you may be able to operate it successfully others. I have not offered an overview of the installation and configuration of some components, but intend to add those later as part of a more well-rounded documentation set.
Operating Systems
-	Ubuntu 22.04.2 LTS – release link
Programs, libraries, languages
-	Mongodb – v 6.0.5 – install link “Install on Debian”
-	Python v 3.9.12 – install link, beginner’s guide link
-	Jupyter Notebook – install link, beginner’s guide link
Basic Program Usage
To use the program in its current state: 
1.	Once the OS, environment, database, and collection, are properly configured on the machine (currently out of the scope of this documentation), you will need to launch the Jupyter notebook program. Note: MongoDB must be running through the ‘mongosh’ command before the program will work.
a.	Once in the Jupyter notebook program, navigate to the “jupyterCallCRUD.py” file, which will open a new tab to run and edit the program. (screenshot below)


![image](https://github.com/Whiteaw2/CS340/assets/20048527/7d631616-920f-4fdc-850a-8aa03ff32cd0)




Next, alter the commands that you would like to test functionality for. The text can be changed in the notebook and will dynamically make the correct calls to the mongoDB.


![image](https://github.com/Whiteaw2/CS340/assets/20048527/14f55fb3-fe5d-4ac1-893d-a885369ee965)


Note:
-	The database must have the required collection uploaded or created, as well as the appropriate user profiles configured, which is currently out of the scope of this documentation.
-	The two scripts must currently be housed in the same directory for the program to work
Following are screenshots of the importing of the dataset (CSV), user credentials, and operation of CRUD functionality. Commands will be very similar depending on your dataset and user credentials.



## 1.	Upload of Austin Animal Center Outcomes Dataset

 

![image](https://github.com/Whiteaw2/CS340/assets/20048527/3b30290d-a416-451f-8e0f-3ad9adff1e75)




## 2.	Create a user account in mongo shell to ensure user authentication to the database and collection.

 ![image](https://github.com/Whiteaw2/CS340/assets/20048527/19f00266-7816-48e0-bc0a-c3a1b811e6b9)



## 3. CRUD functionality that, when instantiated, provides the specified functionality.

Successful “Create” – shows state of happy path.
![image](https://github.com/Whiteaw2/CS340/assets/20048527/5131af5f-0eb1-499d-926f-82a786f94fe2)
 

## Failure “Create” – shows improper input error response state.
 ![image](https://github.com/Whiteaw2/CS340/assets/20048527/74bf0f49-9105-4f0d-aec5-0cf5382748e7)




## Successful “Read” – returns list of matching items in database. Note: the “readExactMatch” value sets a flag to match an exact string or any entry that contains that string. Example would be that “test” appears in “retestable”, but is not an exact match as it contains more letters.
 ![image](https://github.com/Whiteaw2/CS340/assets/20048527/97c371c0-d604-417e-ab25-8e17bcb387ba)




## Failure “Read” – improper input or no matching data.
 ![image](https://github.com/Whiteaw2/CS340/assets/20048527/551760a0-ebc3-4157-8d72-cc4014d2fab1)




## Successful “Update” – returns number of updated items.
 ![image](https://github.com/Whiteaw2/CS340/assets/20048527/1d65580b-1a18-40df-9bed-215207f65ec0)




## “Update” with no matching entries
 ![image](https://github.com/Whiteaw2/CS340/assets/20048527/add439dc-24d9-4d6b-97c3-9fcb82a703bb)




## Successful “Delete”
 ![image](https://github.com/Whiteaw2/CS340/assets/20048527/26865cba-07ea-4436-b299-ea4fa8992ed9)





## Failure “Delete”
 ![image](https://github.com/Whiteaw2/CS340/assets/20048527/4343c5fc-7bc2-4522-ac2e-7b8650dad3b0)



## Sources

_ _  Dash. Dash Leaflet. (n.d.). https://dash-leaflet-docs.onrender.com/ 

_ _ Dash Documentation & User Guide | Plotly. (n.d.). https://dash.plotly.com/

_ _ MongoDB. (n.d.). MongoDB: The Developer Data Platform. https://www.mongodb.com/

_ _ PEP 8 – Style Guide for Python Code | peps.python.org. (n.d.). https://peps.python.org/pep-0008/

_ _ PyCharm: the Python IDE for Professional Developers by JetBrains. (2021, June 2). JetBrains. https://www.jetbrains.com/pycharm/

_ _ Project Jupyter. (n.d.). Home. https://jupyter.org/

_ _ Stack Overflow - Where Developers Learn, Share, & Build Careers. (n.d.). Stack Overflow. https://stackoverflow.com/



