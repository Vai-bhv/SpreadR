# SpreadR


Purpose

This code is for creating an interactive spreadsheet web application. It allows users to create multiple sheets, add, edit, and delete cells in those sheets. It also supports formulas, cell formatting, and other basic spreadsheet functionality.


Packages Used

This code does not use any external packages.



Code Structure

The code is structured as follows:


Variables

activeSheetColor: a variable that stores the color code of the active sheet.
sheetsFolderCont: a variable that stores the reference to the DOM element that contains all the sheet folders.
addSheetBtn: a variable that stores the reference to the DOM element of the add sheet button.


Event Listeners

addSheetBtn: an event listener that listens for a click on the add sheet button. It creates a new sheet, updates the database, updates the UI, and sets the newly created sheet as active.


Functions

createSheetDB(): a function that creates a two-dimensional array representing the database of the sheet. It creates an empty cell object for each cell in the sheet and pushes it to the sheet database.

createGraphComponentMatrix(): a function that creates a two-dimensional array representing the dependency matrix of the sheet. It creates an empty array for each cell in the sheet and pushes it to the graph component matrix.
handleSheetActiveness(sheet): a function that listens for a click event on the sheet and sets the clicked sheet as active. It updates the sheet database, the UI, and the properties of the sheet.

handleSheetUI(sheet): a function that updates the UI to reflect the active sheet. It sets the background color of the active sheet to activeSheetColor and sets the background color of all other sheets to transparent.

handleSheetProperties(): a function that sets the properties of all cells in the sheet to their default values. It clicks on each cell in the sheet to trigger the event listener that sets the default properties of the cell.

handleSheetDB(sheetIdx): a function that sets the sheet database and graph component matrix to the corresponding sheet indexed by sheetIdx.
handleSheetRemoval(sheet): a function that listens for a right-click event on a sheet and removes it permanently. It updates the database, the UI, and sets the active sheet to the first sheet.

handleSheetUIRemoval(sheet): a function that removes a sheet from the UI. It updates the sheet IDs and sets the background color of the first sheet to activeSheetColor.


Conclusion

This code provides a basic structure for creating an interactive spreadsheet web application. It allows users to create and manage multiple sheets and perform basic spreadsheet operations.
