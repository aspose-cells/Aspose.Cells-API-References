---
title: "WorksheetCollection"
linktitle: "WorksheetCollection"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Encapsulates a collection of Worksheet objects."
type: docs
weight: 4740
url: /nodejs/aspose.cells/worksheetcollection/
---

## WorksheetCollection class

Encapsulates a collection of Worksheet objects.

## Methods

| Name | Description |
| --- | --- |
| [add(type)](#add) | Adds a worksheet to the collection. |
| [add()](#add-1) | Adds a worksheet to the collection. |
| [add(sheetName)](#add-2) | Adds a worksheet to the collection. |
| [add()](#add-3) | Reserved for internal use. |
| [addCopy(sheetName)](#addcopy) | Adds a worksheet to the collection and copies data from an existed worksheet. |
| [addCopy(sheetIndex)](#addcopy-1) | Adds a worksheet to the collection and copies data from an existed worksheet. |
| [addCopy(source, destSheetNames)](#addcopy-2) | Copy a group of worksheets. |
| [clear()](#clear) | Clear all worksheets. A workbook must contains a worksheet. |
| [clearPivottables()](#clearpivottables) | Clears pivot tables from the spreadsheet. |
| [contains()](#contains) | Reserved for internal use. |
| [createRange(address, sheetIndex)](#createrange) | Creates a Range object from an address of the range. |
| [createUnionRange(address, sheetIndex)](#createunionrange) | Creates a Range object from an address of the range. |
| [get(index)](#get) | Gets the Worksheet element at the specified index. |
| [get(sheetName)](#get-1) | Gets the Worksheet element with the specified name. |
| [get()](#get-2) | Reserved for internal use. |
| [getActiveSheetIndex()](#getactivesheetindex) | Represents the index of active worksheet when the spreadsheet is opened. Sheet index is zero based. |
| [getActiveSheetName()](#getactivesheetname) | Represents the name of active worksheet when the spreadsheet is opened. |
| [getBuiltInDocumentProperties()](#getbuiltindocumentproperties) | Returns a DocumentProperty collection that represents all the built-in document properties of the spreadsheet. A new pro |
| [getCount()](#getcount) |  |
| [getCustomDocumentProperties()](#getcustomdocumentproperties) | Returns a DocumentProperty collection that represents all the custom document properties of the spreadsheet. |
| [getDxfs()](#getdxfs) | Gets the master differential formatting records. |
| [getExternalLinks()](#getexternallinks) | Represents external links in a workbook. |
| [getNamedRanges()](#getnamedranges) | Gets all pre-defined named ranges in the spreadsheet. |
| [getNamedRangesAndTables()](#getnamedrangesandtables) | Gets all pre-defined named ranges in the spreadsheet. |
| [getNames()](#getnames) | Gets the collection of all the Name objects in the spreadsheet. |
| [getOleSize()](#getolesize) | Gets and Sets displayed size when Workbook file is used as an Ole object. Null means no ole size setting. |
| [getPivotCaches()](#getpivotcaches) |  |
| [getRangeByName(rangeName)](#getrangebyname) | Gets Range object by pre-defined name. |
| [getRangeByName(rangeName, currentSheetIndex, includeTable)](#getrangebyname-1) | Gets Range by pre-defined name or table's name |
| [getRevisionLogs()](#getrevisionlogs) | Represents revision logs. |
| [getSensitivityLabels()](#getsensitivitylabels) |  |
| [getSheetByCodeName(codeName)](#getsheetbycodename) | Gets the worksheet by the code name. |
| [getTableStyles()](#gettablestyles) | Gets TableStyles object. |
| [getThreadedCommentAuthors()](#getthreadedcommentauthors) | Gets the list of threaded comment authors. |
| [getWebExtensionTaskPanes()](#getwebextensiontaskpanes) | Gets the list of task panes. |
| [getWebExtensions()](#getwebextensions) | Gets the list of task panes. |
| [getXmlMaps()](#getxmlmaps) | Gets and sets the XML maps in the workbook. |
| [indexOf()](#indexof) | Reserved for internal use. |
| [insert(index, sheetType)](#insert) | Insert a worksheet. |
| [insert(index, sheetType, sheetName)](#insert-1) | Insert a worksheet. |
| [isRefreshAllConnections()](#isrefreshallconnections) | Indicates whether refresh all connections on opening file in MS Excel. |
| [iterator()](#iterator) |  |
| [refreshAll()](#refreshall) | Refresh all pivot tables and charts with pivot source. |
| [refreshPivotTables()](#refreshpivottables) | Refreshes all the PivotTables in the Excel file. |
| [refreshPivotTables(option)](#refreshpivottables-1) | Refreshes all the PivotTables in the Excel file. |
| [registerAddInFunction(addInFile, functionName, lib)](#registeraddinfunction) | Adds addin function into the workbook |
| [registerAddInFunction(id, functionName)](#registeraddinfunction-1) | Adds addin function into the workbook |
| [removeAt(name)](#removeat) | Removes the element at a specified name. |
| [removeAt(index)](#removeat-1) | Removes the element at a specified index. |
| [setActiveSheetIndex()](#setactivesheetindex) | Represents the index of active worksheet when the spreadsheet is opened. Sheet index is zero based. |
| [setActiveSheetName()](#setactivesheetname) | Represents the name of active worksheet when the spreadsheet is opened. |
| [setOleSize()](#setolesize) | Gets and Sets displayed size when Workbook file is used as an Ole object. Null means no ole size setting. |
| [setOleSize(startRow, endRow, startColumn, endColumn)](#setolesize-1) | Sets displayed size when Workbook file is used as an Ole object. This method is generally used to adjust display size in |
| [setRefreshAllConnections()](#setrefreshallconnections) | Indicates whether refresh all connections on opening file in MS Excel. |
| [setXmlMaps()](#setxmlmaps) | Gets and sets the XML maps in the workbook. |
| [sortNames()](#sortnames) | Sorts the defined names. If you create a large amount of named ranges in the Excel file, please call this method after a |
| [swapSheet(sheetIndex1, sheetIndex2)](#swapsheet) | Swaps the two sheets. |

### add(type) {#add}

Adds a worksheet to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | SheetType |

**Returns:** Number — `Number` Worksheet object index.

**Example:**

```js
var workbook = new aspose.cells.Workbook();
workbook.getWorksheets().add(aspose.cells.SheetType.CHART);
var cells = workbook.getWorksheets().get(0).getCells();
cells.get("c2").putValue(5000);
cells.get("c3").putValue(3000);
cells.get("c4").putValue(4000);
cells.get("c5").putValue(5000);
cells.get("c6").putValue(6000);
var charts = workbook.getWorksheets().get(1).getCharts();
var chartIndex = charts.add(aspose.cells.ChartType.COLUMN, 10, 10, 20, 20);
var chart = charts.get(chartIndex);
chart.getNSeries().add("Sheet1!C2:C6", true);
```

### add() {#add-1}

Adds a worksheet to the collection.

**Returns:** Number — `Number` Worksheet object index.

### add(sheetName) {#add-2}

Adds a worksheet to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | String | Worksheet name |

**Returns:** Worksheet — `Worksheet` Worksheet object.

### add() {#add-3}

Reserved for internal use.

### addCopy(sheetName) {#addcopy}

Adds a worksheet to the collection and copies data from an existed worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | String | Name of source worksheet. |

**Returns:** Number — `Number` Worksheet object index.

### addCopy(sheetIndex) {#addcopy-1}

Adds a worksheet to the collection and copies data from an existed worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | Number | Index of source worksheet. |

**Returns:** Number — `Number` Worksheet object index.

### addCopy(source, destSheetNames) {#addcopy-2}

Copy a group of worksheets.

| Parameter | Type | Description |
| --- | --- | --- |
| source | Array ofWorksheet | The source worksheets. |
| destSheetNames | Array of String | The names of the copied sheets. |

### clear() {#clear}

Clear all worksheets. A workbook must contains a worksheet.

### clearPivottables() {#clearpivottables}

Clears pivot tables from the spreadsheet.

### contains() {#contains}

Reserved for internal use.

### createRange(address, sheetIndex) {#createrange}

Creates a Range object from an address of the range.

| Parameter | Type | Description |
| --- | --- | --- |
| address | String | The address of the range. |
| sheetIndex | Number | The sheet index. |

**Returns:** Range — `Range` A Range object

### createUnionRange(address, sheetIndex) {#createunionrange}

Creates a Range object from an address of the range.

| Parameter | Type | Description |
| --- | --- | --- |
| address | String | The address of the range. |
| sheetIndex | Number | The sheet index. |

**Returns:** UnionRange — `UnionRange` A Range object

### get(index) {#get}

Gets the Worksheet element at the specified index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The zero based index of the element. |

**Returns:** Worksheet — `Worksheet` The element at the specified index.

### get(sheetName) {#get-1}

Gets the Worksheet element with the specified name.

| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | String | Worksheet name |

**Returns:** Worksheet — `Worksheet` The element with the specified name.

### get() {#get-2}

Reserved for internal use.

### getActiveSheetIndex() {#getactivesheetindex}

Represents the index of active worksheet when the spreadsheet is opened. Sheet index is zero based.

### getActiveSheetName() {#getactivesheetname}

Represents the name of active worksheet when the spreadsheet is opened.

### getBuiltInDocumentProperties() {#getbuiltindocumentproperties}

Returns a DocumentProperty collection that represents all the built-in document properties of the spreadsheet. A new property cannot be added to built-in document properties list. You can only get a built-in property and change its value. The following is the built-in properties name list: TitleSubjectAuthorKeywordsCommentsTemplateLast AuthorRevision NumberApplication NameLast Print DateCreation DateLast Save TimeTotal Editing TimeNumber of PagesNumber of WordsNumber of CharactersSecurityCategoryFormatManagerCompanyNumber of BytesNumber of LinesNumber of ParagraphsNumber of SlidesNumber of NotesNumber of Hidden SlidesNumber of Multimedia Clips

**Example:**

```js
var doc = workbook.getWorksheets().getBuiltInDocumentProperties().get("Author");
doc.setValue("John Smith");
```

### getCount() {#getcount}

### getCustomDocumentProperties() {#getcustomdocumentproperties}

Returns a DocumentProperty collection that represents all the custom document properties of the spreadsheet.

**Example:**

```js
excel.getWorksheets().getCustomDocumentProperties().add("Checked by", "Jane");
```

### getDxfs() {#getdxfs}

Gets the master differential formatting records.

### getExternalLinks() {#getexternallinks}

Represents external links in a workbook.

### getNamedRanges() {#getnamedranges}

Gets all pre-defined named ranges in the spreadsheet.

**Returns:** Array ofRange — `Array ofRange` An array of Range objects. If the defined Name's reference is external or has multiple ranges, no Range object will be returned for this Name. Returns null if the named range does not exist.

### getNamedRangesAndTables() {#getnamedrangesandtables}

Gets all pre-defined named ranges in the spreadsheet.

**Returns:** Array ofRange — `Array ofRange` An array of Range objects.Returns null if the named range does not exist.

### getNames() {#getnames}

Gets the collection of all the Name objects in the spreadsheet.

### getOleSize() {#getolesize}

Gets and Sets displayed size when Workbook file is used as an Ole object. Null means no ole size setting.

### getPivotCaches() {#getpivotcaches}

### getRangeByName(rangeName) {#getrangebyname}

Gets Range object by pre-defined name.

| Parameter | Type | Description |
| --- | --- | --- |
| rangeName | String | Name of range. |

**Returns:** Range — `Range` Range object.Returns null if the named range does not exist.

### getRangeByName(rangeName, currentSheetIndex, includeTable) {#getrangebyname-1}

Gets Range by pre-defined name or table's name

| Parameter | Type | Description |
| --- | --- | --- |
| rangeName | String | Name of range or table's name. |
| currentSheetIndex | Number | The sheet index. -1 represents global . |
| includeTable | boolean | Indicates whether checking all tables. |

**Returns:** Range — `Range`

### getRevisionLogs() {#getrevisionlogs}

Represents revision logs.

### getSensitivityLabels() {#getsensitivitylabels}

### getSheetByCodeName(codeName) {#getsheetbycodename}

Gets the worksheet by the code name.

| Parameter | Type | Description |
| --- | --- | --- |
| codeName | String | Worksheet code name. |

**Returns:** Worksheet — `Worksheet` The element with the specified code name.

### getTableStyles() {#gettablestyles}

Gets TableStyles object.

### getThreadedCommentAuthors() {#getthreadedcommentauthors}

Gets the list of threaded comment authors.

### getWebExtensionTaskPanes() {#getwebextensiontaskpanes}

Gets the list of task panes.

### getWebExtensions() {#getwebextensions}

Gets the list of task panes.

### getXmlMaps() {#getxmlmaps}

Gets and sets the XML maps in the workbook.

### indexOf() {#indexof}

Reserved for internal use.

### insert(index, sheetType) {#insert}

Insert a worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The sheet index |
| sheetType | Number | SheetType |

**Returns:** Worksheet — `Worksheet` Returns an inserted worksheet.

### insert(index, sheetType, sheetName) {#insert-1}

Insert a worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The sheet index |
| sheetType | Number | SheetType |
| sheetName | String | The sheet name. |

**Returns:** Worksheet — `Worksheet` Returns an inserted worksheet.

### isRefreshAllConnections() {#isrefreshallconnections}

Indicates whether refresh all connections on opening file in MS Excel.

### iterator() {#iterator}

### refreshAll() {#refreshall}

Refresh all pivot tables and charts with pivot source.

### refreshPivotTables() {#refreshpivottables}

Refreshes all the PivotTables in the Excel file.

### refreshPivotTables(option) {#refreshpivottables-1}

Refreshes all the PivotTables in the Excel file.

| Parameter | Type | Description |
| --- | --- | --- |
| option | PivotTableRefreshOption | The option for refreshing data source of the pivot tables. |

### registerAddInFunction(addInFile, functionName, lib) {#registeraddinfunction}

Adds addin function into the workbook

| Parameter | Type | Description |
| --- | --- | --- |
| addInFile | String | the file contains the addin functions |
| functionName | String | the addin function name |
| lib | boolean | whether the given addin file is in the directory or sub-directory of Workbook Add-In library. This flag takes effect and makes difference when given addInFile is of relative path: true denotes the path is relative to Add-In library and false denotes the path is relative to this Workbook. |

**Returns:** Number — `Number` ID of the data which contains given addin function

### registerAddInFunction(id, functionName) {#registeraddinfunction-1}

Adds addin function into the workbook

| Parameter | Type | Description |
| --- | --- | --- |
| id | Number | ID of the data which contains addin functions, can be got by the first call of |
| functionName | String | the addin function name |

**Returns:** String — `String` URL of the addin file which contains addin functions

### removeAt(name) {#removeat}

Removes the element at a specified name.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the element to remove. |

### removeAt(index) {#removeat-1}

Removes the element at a specified index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The index value of the element to remove. |

### setActiveSheetIndex() {#setactivesheetindex}

Represents the index of active worksheet when the spreadsheet is opened. Sheet index is zero based.

### setActiveSheetName() {#setactivesheetname}

Represents the name of active worksheet when the spreadsheet is opened.

### setOleSize() {#setolesize}

Gets and Sets displayed size when Workbook file is used as an Ole object. Null means no ole size setting.

### setOleSize(startRow, endRow, startColumn, endColumn) {#setolesize-1}

Sets displayed size when Workbook file is used as an Ole object. This method is generally used to adjust display size in ppt file or doc file.

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Number | Start row index. |
| endRow | Number | End row index. |
| startColumn | Number | Start column index. |
| endColumn | Number | End column index. |

### setRefreshAllConnections() {#setrefreshallconnections}

Indicates whether refresh all connections on opening file in MS Excel.

### setXmlMaps() {#setxmlmaps}

Gets and sets the XML maps in the workbook.

### sortNames() {#sortnames}

Sorts the defined names. If you create a large amount of named ranges in the Excel file, please call this method after all named ranges are created and before saving

### swapSheet(sheetIndex1, sheetIndex2) {#swapsheet}

Swaps the two sheets.

| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex1 | Number | The first worksheet. |
| sheetIndex2 | Number | The second worksheet. |
