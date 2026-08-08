---
title: "CellsHelper"
linktitle: "CellsHelper"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Provides helper functions."
type: docs
weight: 460
url: /nodejs/aspose.cells/cellshelper/
---

## CellsHelper class

Provides helper functions.

## Methods

| Name | Description |
| --- | --- |
| [getAltStartPath()](./getaltstartpath/) | Gets or sets the alternate startup path, which is referred to by some external formula references. |
| [getCustomImplementationFactory()](./getcustomimplementationfactory/) | Gets or sets the factory for creating instances with special implementation. |
| [getDPI()](./getdpi/) | Gets the DPI of the machine. |
| [getLibraryPath()](./getlibrarypath/) | Gets or sets the library path which is referred to by some external formula references. |
| [getSignificantDigits()](./getsignificantdigits/) | Gets and sets the number of significant digits. The default value is 17. Only could be 15 or 17 now. |
| [getSignificantDigitsType()](./getsignificantdigitstype/) | The value of the property is SignificantDigitsType integer constant. |
| [getStartupPath()](./getstartuppath/) | Gets or sets the startup path, which is referred to by some external formula references. |
| [isCloudPlatform()](./iscloudplatform/) | Please set this property True when running on a cloud platform, such as: Azure, AWSLambda, etc, |
| [setAltStartPath()](./setaltstartpath/) | Gets or sets the alternate startup path, which is referred to by some external formula references. |
| [setCloudPlatform()](./setcloudplatform/) | Please set this property True when running on a cloud platform, such as: Azure, AWSLambda, etc, |
| [setCustomImplementationFactory()](./setcustomimplementationfactory/) | Gets or sets the factory for creating instances with special implementation. |
| [setDPI()](./setdpi/) | Gets the DPI of the machine. |
| [setLibraryPath()](./setlibrarypath/) | Gets or sets the library path which is referred to by some external formula references. |
| [setSignificantDigits()](./setsignificantdigits/) | Gets and sets the number of significant digits. The default value is 17. Only could be 15 or 17 now. |
| [setSignificantDigitsType()](./setsignificantdigitstype/) | The value of the property is SignificantDigitsType integer constant. |
| [setStartupPath()](./setstartuppath/) | Gets or sets the startup path, which is referred to by some external formula references. |
| [addAddInFunction(function, minCountOfParameters, maxCountOfParameters, paramersType, functionValueType)](./addaddinfunction/) *(static)* | Add addin function. NOTE: This member is now obsolete. Instead, please use WorksheetCollection.RegisterAddInFunction() m |
| [cellIndexToName(row, column)](./cellindextoname/) *(static)* | Gets cell name according to its row and column indexes. |
| [cellNameToIndex(cellName)](./cellnametoindex/) *(static)* | Gets the cell row and column indexes according to its name. |
| [columnIndexToName(column)](./columnindextoname/) *(static)* | Gets column name according to column index. |
| [columnNameToIndex(columnName)](./columnnametoindex/) *(static)* | Gets column index according to column name. |
| [convertA1FormulaToR1C1(formula, row, column)](./converta1formulator1c1/) *(static)* | Converts A1 formula of the cell to the r1c1 formula. NOTE: This member is now obsolete. Instead, please use Worksheet.Co |
| [convertR1C1FormulaToA1(r1c1Formula, row, column)](./convertr1c1formulatoa1/) *(static)* | Converts the r1c1 formula of the cell to A1 formula. NOTE: This member is now obsolete. Instead, please use Worksheet.Co |
| [createSafeSheetName(nameProposal)](./createsafesheetname/) *(static)* | Checks given sheet name and create a valid one when needed. If given sheet name conforms to the rules of excel sheet nam |
| [createSafeSheetName(nameProposal, replaceChar)](./createsafesheetname-1/) *(static)* | Checks given sheet name and create a valid one when needed. If given sheet name conforms to the rules of excel sheet nam |
| [getCacheFolder()](./getcachefolder/) *(static)* |  |
| [getDateTimeFromDouble(doubleValue, date1904)](./getdatetimefromdouble/) *(static)* | Convert the double value to the date time value. |
| [getDoubleFromDateTime(dateTime, date1904)](./getdoublefromdatetime/) *(static)* | Convert the date time to double value. |
| [getTextWidth(text, font, scaling)](./gettextwidth/) *(static)* | Get width of text in unit of points. |
| [getUsedColors(workbook)](./getusedcolors/) *(static)* | Gets all used colors in the workbook. |
| [getVersion()](./getversion/) *(static)* | Get the release version. |
| [mergeFiles(files, cachedFile, destFile)](./mergefiles/) *(static)* | Merges some large xls files to a xls file. This method only supports merging data, style and formulas to the new file. T |
| [needQuoteInFormula(sheetName)](./needquoteinformula/) *(static)* | Indicates whether the name of the sheet should be enclosed in single quotes |
| [rowIndexToName(row)](./rowindextoname/) *(static)* | Gets row name according to row index. |
| [rowNameToIndex(rowName)](./rownametoindex/) *(static)* | Gets row index according to row name. |
| [setCacheFolder()](./setcachefolder/) *(static)* |  |
