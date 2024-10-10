# RMA-Selector

## About the Project
This project is an application I created in my professional career to assist to help speed up the work flow of coworkers who performed manual data entry; specifically when entering a failure mode for a product. The software being used for data entry only had one single text field/dropdown box and thus every failure reason across all products would be displayed, thus adding time and difficulty to quick selection of the right reason. A simpler solution would be to allow selection of product, filter for unique parent failure categories for that product, and then futher filter for associated child reason root causes with the selected parent reason.

The goal was to allow a user to select a local CSV file, and then have 3 dropdown selection boxes where each chosen value would filter the options available in the next one(s). When the third and final dropdown value was selected, the User could click the "Copy Reason to Clipboard" button to automatically have the chosen value ready for pasting.

## Getting Started
This code uses [Python](https://www.python.org/) with the following packages:
- [pandas]([https://numpy.org/](https://pandas.pydata.org/))
- [os](https://docs.python.org/3/library/os.html)
- [tkinter](https://docs.python.org/3/library/tkinter.html)

## Usage
The application is a simple interface designed for ease of use. 

![RMA Selector Interface](https://github.com/user-attachments/assets/29ac99b9-6eea-4564-a897-5c1cb6ff3163)

Below is an example of a sample csv containing product, parent reason, and child reason data.

### ...

In order to use the Analyzer application, perform the following steps:
1. Click the *Select CSV* button to open a file dialog and choose the csv to use.
2. Open the *Product Category* dropdown and select the correct product.
3. Open the *Parent Reason* dropdown and select the correct parent reason.
4. Open the *Child Reason* dropdown and select the correct child reason.
5. Click *Copy RMA Reason to Clipboard* button to copy the selected child reason to the clipboard for pasting elsewhere.
