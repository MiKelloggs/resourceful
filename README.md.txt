**Resource:** Glass management database

ID | Beginning Year | Ending Year | Make | Model | Part Number | Special Notes | Cost | Quantity in Stock
---|---|----|----|----|----|----|----|----
Integer | Integer | Integer | Varchar | Varchar | Varchar | Varchar | Integer | Integer
ID | The first year of vehicle that the windshield will fit | The last year it will | Vehicle Make | Vehicle Model | Part Number of Glass| Special Notes: (Heated, Rain Sensor etc...) | Price of the windshield from warehouse | Amount of units in stock


**CREATE TABLE** *glassdb* (

**id** INTEGER PRIMARY KEY,

**yearstart** VARCHAR(255),

**yearend** VARCHAR(255),

**make** VARCHAR(255),

**model** VARCHAR(255),

**partnumber** VARCHAR(255),

**location** VARCHAR(255),

**cost** INTEGER,

**stock** INTEGER);


*  **GET** - View Current Stock - "*/windshields*" -
* Search by Part Number - "/windshields/windshield" - GET



Method | Path | Name
---|---|----
GET | /windshields | View Current Stock
GET | /windshields/windshield | Search by Part Number
POST | /windshields/windshield | Create New Entry
PUT | /windshields/windshield | Modify Current Stock
DELETE | /windshields/windshield | Delete by Part Number