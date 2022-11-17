# UFO-Sightings

## Overview

This project is built to display UFO sightings data collection as a table using JavaScript. Javascript allows users to filter data to find specific information. Additionally, an article about UFO sightings and the data/table are be gathered on an HTML page. 

### The table

A **data.js** file was provided containing a lot of information about UFOs, including the date there were spotted, the city, state, country and etc.
Using this information a new **app.js** file is created to build a table. Initially, the data information is integrated to the new file and the body of the table is selected using **d3** library:

<img width="276" alt="Screen Shot 2022-11-17 at 2 18 37 PM" src="https://user-images.githubusercontent.com/111609994/202572280-8d835a2b-a7cc-4b6c-8708-5de5c6202888.png">

This part of code uses standard javascript function to create a canvas to later populate it with the given data. Using ***forEach** the code loops through each object in the data array, appends each row to the HTML table, then adds each value from the object into a **cell**.

<img width="353" alt="Screen Shot 2022-11-17 at 2 18 46 PM" src="https://user-images.githubusercontent.com/111609994/202572311-5c1e4cb7-d631-4703-bd28-cea67b989d42.png">

### HTML

In the meantime, it's important to keep track of the **html** file where all of this data will be gathered and displayed eventually.

Using a shortcut autofill the html file is populated with default starter code and BootstrapCDN is linked alongside with **style.css** which is used later to style the page:

<img width="738" alt="Screen Shot 2022-11-17 at 2 23 56 PM" src="https://user-images.githubusercontent.com/111609994/202573002-44de9292-c4f4-42ac-93ce-d4a81fdc9bc6.png">

Headers and paragraphs in the html's body are inserted by using **div class="container-fluid"**:

<img width="788" alt="Screen Shot 2022-11-17 at 2 27 41 PM" src="https://user-images.githubusercontent.com/111609994/202573538-06abe33e-53c0-4874-af5f-6c30b0949820.png">

In a separate **container-fluid** list items are inserted to allow users to filter the table according to their preferences. These list items will include **date, city, state, country and shape**:

<img width="831" alt="Screen Shot 2022-11-17 at 2 29 33 PM" src="https://user-images.githubusercontent.com/111609994/202573931-0af5494e-3dbb-49b5-98ac-509bc47262a2.png">

It's essential to provide all the sources the html file will use to load and display the table:

<img width="658" alt="Screen Shot 2022-11-17 at 2 31 06 PM" src="https://user-images.githubusercontent.com/111609994/202574126-41d5a448-2e32-46d4-8c45-fe43e71439c1.png">

### Return to javascript

In the **app.js** code several functions are built to filter the table.
The **updateFilters** function is built to filter the table based on the input from the users. In addition, an ***if-else*** statement is used to make sure
**filters** exist and a value was entered in order to update the table on the page. If a value is not entered, the table will clear from the filters variable.

<img width="539" alt="Screen Shot 2022-11-17 at 2 34 08 PM" src="https://user-images.githubusercontent.com/111609994/202574756-4c8b36b8-4ce0-4a9d-a309-d65eb812cb2b.png">

Finnaly, **function filterTable()** was inserted to hold the updated table data based on the user input and to rebuild the table with the filtered data by deploying **buildTable(filteredData)**.

### Drawback

One of the drawbacks of this webpage is the lack of flexibility of user inputs. The user must familiarize themselves with the data before filtering it since an incorrect input in the search bars will return nothing. Additionally, we can assume that another drawback is that the users won't be notified if their input is incorrect. For example, if **middleburg** was misspelled ***middle burg***, the table will display nothing and won't notify the user to maybe check the input.

### Additional Steps

I believe **if-else** statements could be deployed to check for incorrect inputs: if the input is incorrect, a message will let the user know. Additionally, correct versions could be offered to the user. 

The data is based on USA. No other countries are used in this data. The country filter could be removed alongside with the column. The users should be informed initially that this data is about USA. It won't trick the users to look for other countries.


