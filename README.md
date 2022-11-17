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




