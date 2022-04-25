# Shirt_Inventory_Tracker

# Project Overview
Legarza Sports is an organization that hosts various youth sports programs, the largest of which is our camp programs. The purpose of this project was to develop a document that automates calculations of the total number of shirts a camp site used and the total cost based on region, program type, shirt size, and shirt color. This project helped to save over 100+ hours and $28,000 in labor hours, costs, and losses due to data inefficiencies and inaccuracies.

# Business Objectives
1.) Consolidate the collection and analysis of camper shirt unit totals and cost data into a single document that every region can access and update.

2.) Analyze camper shirt unit totals and costs based on region, program type, shirt size, and color

3.) Use analyses of shirt totals to make data-driven decisions on what type of shirts and how many to buy


## Inventory Document Features
### Shirt Tracker Tab
<img width="656" alt="Screen Shot 2022-04-24 at 6 07 43 PM" src="https://user-images.githubusercontent.com/102498189/165005227-b74d8295-2dc4-455a-a9ce-76beead56d5d.png">
-Column A specifies the date that a program coordinator pulled shirts for a specified camp. This information is used to help filter regional calculations in the "Regional Totals" tab.

-Column B specifies the region that shirts are being pulled for and includes a data validation drop down menu to ensure that regional inputs are restricted and uniform in format.

-Column C specifies the program type for shirts being pulled and includes a data validation drop down menu to ensure that program inputs are restricted to those the company offers and are uniform in format.

-Column D specifies the shirt size for shirts being pulled and includes a data validation drop down menu to ensure consistent formating for shirt size selections.

-Column E specifies the shirt color for shirts being pulled and includes a data validation drop down menu to ensure that only colors provided by the company are selected.

-Column F specifies how many shirts were taken from the company's warehouse to a camp site for a particular shirt given the program type, size, and color.

-Column G specifies how many shirts were returned to the company's warehouse from a camp site after a camp was conducted given the program type, size, and color.

-Column H automatically calculates how many shirts were used based on a given program type, size, and color by subtracting the total returned from the total taken.

### Regional Totals Tab
<img width="1142" alt="Screen Shot 2022-04-24 at 6 24 18 PM" src="https://user-images.githubusercontent.com/102498189/165006140-b7aa682a-3e05-4ff7-ad78-caecd51017de.png">
Tables are created in order to show the total number of shirts used based on the overarching program of the shirt which is then subdivided into sizes and then the colors offered in each size. The "Total Used" Column within each shirt size table utilizes a SUMIFS function that calculates the total number of shirts used based on a few conditions that are met in the "Shirt Tracker" tab:

-A specified region in a data valdiated dropdown menu in cell B1

-The program matches the name of the program in the program banner of each table (i.e. "Basketball", "All-Sports", etc.)

-The shirt size matches the shirt size at the top left of each sub table

-The shirt color matches the shirt color to the left of the "Total Used" column

### Shirt Inventory Charts Tab
<img width="588" alt="Screen Shot 2022-04-24 at 6 37 44 PM" src="https://user-images.githubusercontent.com/102498189/165006986-5aca9bb1-4f40-41d7-bd3b-9b5fb820542e.png">
Utilized data from the "Shirt Tracker" tab to create informative pivot tables and pivot charts to be utilized in the "Dashboard" tab.

### Dashboard Tab
<img width="876" alt="Screen Shot 2022-04-24 at 6 39 28 PM" src="https://user-images.githubusercontent.com/102498189/165007096-a6b42893-580f-4eb2-b76f-88014b2b8aa5.png">
Utilized pivot charts from the "Shirt Inventory Charts" tab to visualize shirt usage by program, color, and size that can be filtered based on region.
