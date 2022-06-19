# Polynomial approximation
Automatic polynomial approximation for n given points in 2D

## About math
App uses simple least squares methods to plot polynomial regression curve from given dataset

## Input options
User can input data either from .xslx file or manually
### Importing data from excel
Importing data have strict rules for successfully import given data. 
- Vars has to be in cells A1 and B1
- values for **x-coordinates** is vertically in columnn A starting from A2
- values for **y-coordinates** is vertically in columnn B starting from B2

Exapmle:

![image](https://user-images.githubusercontent.com/53153263/157262109-8e722c7b-f638-45e1-8c16-0bc2365bef91.png)

## Navigation

![image](https://user-images.githubusercontent.com/53153263/157262789-3c115e30-a449-4e32-8910-a6b0168a23af.png)

### 1. Function controller
- Is controlling user navigation into the database of saved function
- For first function is defaultly set name to be "Function 1" but it's editable
- For every new function is defaultly set name to be "new function" but it's also editable
- **Save function** stores function in database
- after saving is enabled button **Next** that switch to next function
- **Previous** button switch to previous function
### 2. Show options
- First group **"Show"** controlls ploting 
- Available options are: show approximation curve and pionts from dataset; Show only points; Show only approximation curve
- **"Functions"** group controlls ploting of functions
- Available options are: show only current function; Show current function (don't have to be stored in database) and all stored function
- Show options are global for all functions in database. That means that user cannot show one function with option "only points" and rest of them with option "only curve".
### 3. Database
- Box, that lists all function in database
### 4. Export
- Export current function to Excel
### 5. Data controller
- **Import data** button let user import data from Excel file (read "Importing data from excel" above for more information)
- **Number of points** spinner let user set set number of points of dataset; It's autoupdated when importing data
- Table contains dataset for plotting
- Number of table rows is controlled by number of points spinner
- User can edit data even from imported file
- **Degree of polynomial** sets polynomial regression degree: currently available is 1 (linear regression), 2, 3, 4, 5, exponential
- **Clear** Delete all data from table
- **Refresh points** manual override if plot is badly rendered
### 6. Axes
- Show functions according to dataset and show options
### 7. Prompt
- Used for reporting current app status
