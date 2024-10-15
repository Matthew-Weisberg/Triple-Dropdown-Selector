# Triple-Dropdown-Selector

## About the Project
This project is an application I created in my professional career to assist to help speed up the work flow of coworkers who performed manual data entry; specifically when entering a failure mode for a product. The software being used for data entry only had one single text field/dropdown box and thus every failure reason across all products would be displayed, thus adding time and difficulty to quick selection of the right reason. A simpler solution would be to allow selection of product, filter for unique parent failure categories for that product, and then futher filter for associated child reason root causes with the selected parent reason.

The goal was to allow a user to select a local CSV file, and then have 3 dropdown selection boxes where each chosen value would filter the options available in the next one(s). When the third and final dropdown value was selected, the User could click the "Copy Reason to Clipboard" button to automatically have the chosen value ready for pasting.

## Getting Started
This code uses [Python](https://www.python.org/) with the following packages:
- [os](https://docs.python.org/3/library/os.html)
- [pandas](https://pandas.pydata.org/)
- [tkinter](https://docs.python.org/3/library/tkinter.html)

## Usage
The application is a simple interface designed for ease of use. 

![RMA Selector Interface](https://github.com/user-attachments/assets/29ac99b9-6eea-4564-a897-5c1cb6ff3163)

In order to use the Analyzer application, perform the following steps:
1. Click the *Select CSV* button to open a file dialog and choose the csv to use.
2. Open the *Product Category* dropdown and select the correct product.
3. Open the *Parent Reason* dropdown and select the correct parent reason.
4. Open the *Child Reason* dropdown and select the correct child reason.
5. Click *Copy RMA Reason to Clipboard* button to copy the selected child reason to the clipboard for pasting elsewhere.


### Sample Usage

Below is an example of a sample csv titled *failure_reasons.csv* containing product, parent reason, and child reason data.

|Product        |Parent Reason         |Child Reason             |
|---------------|----------------------|-------------------------|
|Blender        |Electrical Issue      |Power Cord Damage        |
|Blender        |Electrical Issue      |Internal Wiring Failure  |
|Blender        |Motor Issue           |Motor Burnout            |
|Blender        |Motor Issue           |Motor Stalling           |
|Blender        |Blade Issue           |Blade Dullness           |
|Blender        |Blade Issue           |Blade Dislodging         |
|Blender        |Overheating           |Motor Overload           |
|Blender        |Overheating           |Prolonged Use            |
|Toaster        |Electrical Issue      |Power Cord Damage        |
|Toaster        |Electrical Issue      |Short Circuit            |
|Toaster        |Heating Element Issue |Burned Heating Coil      |
|Toaster        |Heating Element Issue |Inconsistent Heating     | 
|Toaster        |Bread Ejection Failure|Spring Malfunction       |
|Toaster        |Bread Ejection Failure|Lever Jamming            |
|Toaster        |Overheating           |Thermostat Failure       |
|Toaster        |Overheating           |Prolonged Use            |
|Electric Kettle|Electrical Issue      |Power Cord Damage        |
|Electric Kettle|Electrical Issue      |Loose Connection         |
|Electric Kettle|Heating Issue         |Water Not Heating        |
|Electric Kettle|Heating Issue         |Inconsistent Heating     |
|Electric Kettle|Lid Mechanism Issue   |Lid Not Closing          |
|Electric Kettle|Lid Mechanism Issue   |Latch Failure            |
|Electric Kettle|Overheating           |Boiling Dry              |
|Electric Kettle|Overheating           |Internal Component Damage|

If I wanted to select the **Lever Jamming** reason for the Toaster, I would use the following dropdowns:

![1stDropdown](https://github.com/user-attachments/assets/d515b1e5-3c8c-4012-9ee1-18c290ad75b5)

![2ndDropdown](https://github.com/user-attachments/assets/98c09b18-d845-4b3a-89c2-db40e2571923)

![3rdDropdown](https://github.com/user-attachments/assets/9db78a2a-25a5-43d3-82f2-92f6d780354e)
