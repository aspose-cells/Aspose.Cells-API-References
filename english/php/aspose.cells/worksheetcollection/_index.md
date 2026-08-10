---
title: "WorksheetCollection Class"
linktitle: "WorksheetCollection"
articleTitle: "WorksheetCollection"
second_title: "Aspose.Cells for PHP via Java"
description: "Encapsulates a collection of Worksheet objects."
type: docs
weight: 7610
url: /php/aspose.cells/worksheetcollection/
---

## WorksheetCollection class

Encapsulates a collection of Worksheet objects.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [WebExtensionTaskPanes](#webextensiontaskpanes) | WebExtensionTaskPaneCollection | Gets the list of task panes. |
| [WebExtensions](#webextensions) | WebExtensionCollection | Gets the list of task panes. |
| [ThreadedCommentAuthors](#threadedcommentauthors) | ThreadedCommentAuthorCollection | Gets the list of threaded comment authors. |
| [IsRefreshAllConnections](#isrefreshallconnections) | boolean | Indicates whether refresh all connections on opening file in MS Excel. |
| [Names](#names) | NameCollection | Gets the collection of all the Name objects in the spreadsheet. |
| [ActiveSheetName](#activesheetname) | String | Represents the name of active worksheet when the spreadsheet is opened. |
| [ActiveSheetIndex](#activesheetindex) | Number | Represents the index of active worksheet when the spreadsheet is opened. Sheet index is zero based. |
| [Dxfs](#dxfs) | DxfCollection | Gets the master differential formatting records. |
| [XmlMaps](#xmlmaps) | XmlMapCollection | Gets and sets the XML maps in the workbook. |
| [BuiltInDocumentProperties](#builtindocumentproperties) | BuiltInDocumentPropertyCollection | Returns a DocumentProperty collection that represents all the built-in document properties of the spreadsheet. A new pro |
| [CustomDocumentProperties](#customdocumentproperties) | CustomDocumentPropertyCollection | Returns a DocumentProperty collection that represents all the custom document properties of the spreadsheet. |
| [OleSize](#olesize) | Object | Gets and Sets displayed size when Workbook file is used as an Ole object. Null means no ole size setting. |
| [ExternalLinks](#externallinks) | ExternalLinkCollection | Represents external links in a workbook. |
| [PivotCaches](#pivotcaches) | PivotCacheCollection |  |
| [TableStyles](#tablestyles) | TableStyleCollection | Gets TableStyles object. |
| [RevisionLogs](#revisionlogs) | RevisionLogCollection | Represents revision logs. |
| [SensitivityLabels](#sensitivitylabels) | SensitivityLabelCollection |  |
| [Count](#count) | Number |  |
| [Item (int)](#itemint) | Worksheet | Gets the Worksheet element at the specified index. |
| [Item (java.lang.String)](#itemjavalangstring) | Worksheet | Gets the Worksheet element with the specified name. |

## Methods

| Name | Description |
| --- | --- |
| [setOleSize](#setolesize) | Sets displayed size when Workbook file is used as an Ole object.

This method is generally used to adjust display size i |
| [clearPivottables](#clearpivottables) | Clears pivot tables from the spreadsheet. |
| [refreshAll](#refreshall) | Refresh all pivot tables and charts with pivot source. |
| [refreshPivotTables](#refreshpivottables) | Refreshes all the PivotTables in the Excel file. |
| [createRange](#createrange) | Creates a Range object from an address of the range. |
| [createUnionRange](#createunionrange) | Creates a Range object from an address of the range. |
| [getSheetByCodeName](#getsheetbycodename) | Gets the worksheet by the code name. |
| [sortNames](#sortnames) | Sorts the defined names.

If you create a large amount of named ranges in the Excel file, please call this method after  |
| [insert](#insert) | Insert a worksheet. |
| [add](#add) | Adds a worksheet to the collection. |
| [swapSheet](#swapsheet) | Swaps the two sheets. |
| [registerAddInFunction](#registeraddinfunction) | Adds addin function into the workbook |
| [removeAt](#removeat) | Removes the element at a specified name. |
| [clear](#clear) | Clear all worksheets.

A workbook must contains a worksheet. |
| [addCopy](#addcopy) | Adds a worksheet to the collection and copies data from an existed worksheet. |
| [getRangeByName](#getrangebyname) | Gets Range object by pre-defined name. |
| [getNamedRanges](#getnamedranges) | Gets all pre-defined named ranges in the spreadsheet. |
| [getNamedRangesAndTables](#getnamedrangesandtables) | Gets all pre-defined named ranges in the spreadsheet. |
| [iterator](#iterator) |  |
| [get](#get) | Reserved for internal use. |
| [contains](#contains) | Reserved for internal use. |
| [indexOf](#indexof) | Reserved for internal use. |

### WorksheetCollection.WebExtensionTaskPanes property {#webextensiontaskpanes}

Gets the list of task panes.

**Type:** WebExtensionTaskPaneCollection

### WorksheetCollection.WebExtensions property {#webextensions}

Gets the list of task panes.

**Type:** WebExtensionCollection

### WorksheetCollection.ThreadedCommentAuthors property {#threadedcommentauthors}

Gets the list of threaded comment authors.

**Type:** ThreadedCommentAuthorCollection

### WorksheetCollection.IsRefreshAllConnections property {#isrefreshallconnections}

Indicates whether refresh all connections on opening file in MS Excel.

**Type:** boolean

### WorksheetCollection.Names property {#names}

Gets the collection of all the Name objects in the spreadsheet.

**Type:** NameCollection

### WorksheetCollection.ActiveSheetName property {#activesheetname}

Represents the name of active worksheet when the spreadsheet is opened.

**Type:** String

### WorksheetCollection.ActiveSheetIndex property {#activesheetindex}

Represents the index of active worksheet when the spreadsheet is opened. Sheet index is zero based.

**Type:** Number

### WorksheetCollection.Dxfs property {#dxfs}

Gets the master differential formatting records.

**Type:** DxfCollection

### WorksheetCollection.XmlMaps property {#xmlmaps}

Gets and sets the XML maps in the workbook.

**Type:** XmlMapCollection

### WorksheetCollection.BuiltInDocumentProperties property {#builtindocumentproperties}

Returns a DocumentProperty collection that represents all the built-in document properties of the spreadsheet. A new property cannot be added to built-in document properties list. You can only get a built-in property and change its value. The following is the built-in properties name list: Title Subject Author Keywords Comments Template Last Author Revision Number Application Name Last Print Date Creation Date Last Save Time Total Editing Time Number of Pages Number of Words Number of Characters Security Category Format Manager Company Number of Bytes Number of Lines Number of Paragraphs Number of Slides Number of Notes Number of Hidden Slides Number of Multimedia Clips

**Type:** BuiltInDocumentPropertyCollection

### WorksheetCollection.CustomDocumentProperties property {#customdocumentproperties}

Returns a DocumentProperty collection that represents all the custom document properties of the spreadsheet.

**Type:** CustomDocumentPropertyCollection

### WorksheetCollection.OleSize property {#olesize}

Gets and Sets displayed size when Workbook file is used as an Ole object. Null means no ole size setting.

**Type:** Object

### WorksheetCollection.ExternalLinks property {#externallinks}

Represents external links in a workbook.

**Type:** ExternalLinkCollection

### WorksheetCollection.PivotCaches property {#pivotcaches}

**Type:** PivotCacheCollection

### WorksheetCollection.TableStyles property {#tablestyles}

Gets TableStyles object.

**Type:** TableStyleCollection

### WorksheetCollection.RevisionLogs property {#revisionlogs}

Represents revision logs.

**Type:** RevisionLogCollection

### WorksheetCollection.SensitivityLabels property {#sensitivitylabels}

**Type:** SensitivityLabelCollection

### WorksheetCollection.Count property {#count}

**Type:** Number

### WorksheetCollection.Item (int) property {#itemint}

Gets the Worksheet element at the specified index.

**Type:** Worksheet

### WorksheetCollection.Item (java.lang.String) property {#itemjavalangstring}

Gets the Worksheet element with the specified name.

**Type:** Worksheet

### setOleSize(startRow, endRow, startColumn, endColumn) {#setolesize}

Sets displayed size when Workbook file is used as an Ole object.

This method is generally used to adjust display size in ppt file or doc file.

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Number | Start row index. |
| endRow | Number | End row index. |
| startColumn | Number | Start column index. |
| endColumn | Number | End column index. |

### clearPivottables() {#clearpivottables}

Clears pivot tables from the spreadsheet.

### refreshAll() {#refreshall}

Refresh all pivot tables and charts with pivot source.

### refreshPivotTables() (1 of 2) {#refreshpivottables}

Refreshes all the PivotTables in the Excel file.

---

### refreshPivotTables(option) (2 of 2) {#refreshpivottables-1}

Refreshes all the PivotTables in the Excel file.

| Parameter | Type | Description |
| --- | --- | --- |
| option | PivotTableRefreshOption | The option for refreshing data source of the pivot tables. |

### createRange(address, sheetIndex) {#createrange}

Creates a Range object from an address of the range.

| Parameter | Type | Description |
| --- | --- | --- |
| address | String | The address of the range. |
| sheetIndex | Number | The sheet index. |

**Returns:** A Range object

### createUnionRange(address, sheetIndex) {#createunionrange}

Creates a Range object from an address of the range.

| Parameter | Type | Description |
| --- | --- | --- |
| address | String | The address of the range. |
| sheetIndex | Number | The sheet index. |

**Returns:** A Range object

### getSheetByCodeName(codeName) {#getsheetbycodename}

Gets the worksheet by the code name.

| Parameter | Type | Description |
| --- | --- | --- |
| codeName | String | Worksheet code name. |

**Returns:** The element with the specified code name.

### sortNames() {#sortnames}

Sorts the defined names.

If you create a large amount of named ranges in the Excel file, please call this method after all named ranges are created and before saving

### insert(index, sheetType) (1 of 2) {#insert}

Insert a worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The sheet index |
| sheetType | Number | A SheetType value. The sheet type. |

**Returns:** Returns an inserted worksheet.

---

### insert(index, sheetType, sheetName) (2 of 2) {#insert-1}

Insert a worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The sheet index |
| sheetType | Number | A SheetType value. The sheet type. |
| sheetName | String | The sheet name. |

**Returns:** Returns an inserted worksheet.

### add(type) (1 of 4) {#add}

Adds a worksheet to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | A SheetType value. Worksheet type. |

**Returns:** Worksheet object index.

**Example:**

```php
$workbook = new cells\Workbook();
$workbook->getWorksheets()->add(cells\SheetType::CHART);
$cells = $workbook->getWorksheets()->get(0)->getCells();
$cells->get("c2")->putValue(5000);
$cells->get("c3")->putValue(3000);
$cells->get("c4")->putValue(4000);
$cells->get("c5")->putValue(5000);
$cells->get("c6")->putValue(6000);
$charts = $workbook->getWorksheets()->get(1)->getCharts();
$chartIndex = $charts->add(cells\ChartType::COLUMN, 10, 10, 20, 20);
$chart = $charts->get($chartIndex);
$chart->getNSeries()->add("Sheet1!C2:C6", true);
```

---

### add() (2 of 4) {#add-1}

Adds a worksheet to the collection.

**Returns:** Worksheet object index.

---

### add(sheetName) (3 of 4) {#add-2}

Adds a worksheet to the collection.

| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | String | Worksheet name |

**Returns:** Worksheet object.

---

### add(value) (4 of 4) {#add-3}

Reserved for internal use.

### swapSheet(sheetIndex1, sheetIndex2) {#swapsheet}

Swaps the two sheets.

| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex1 | Number | The first worksheet. |
| sheetIndex2 | Number | The second worksheet. |

### registerAddInFunction(addInFile, functionName, lib) (1 of 2) {#registeraddinfunction}

Adds addin function into the workbook

| Parameter | Type | Description |
| --- | --- | --- |
| addInFile | String | the file contains the addin functions |
| functionName | String | the addin function name |
| lib | boolean | whether the given addin file is in the directory or sub-directory of Workbook Add-In library. This flag takes effect and makes difference when given addInFile is of relative path: true denotes the path is relative to Add-In library and false denotes the path is relative to this Workbook. |

**Returns:** ID of the data which contains given addin function

---

### registerAddInFunction(id, functionName) (2 of 2) {#registeraddinfunction-1}

Adds addin function into the workbook

| Parameter | Type | Description |
| --- | --- | --- |
| id | Number | ID of the data which contains addin functions, can be got by the first call of registerAddInFunction(java.lang.String, java.lang.String, boolean) for the same addin file. |
| functionName | String | the addin function name |

**Returns:** URL of the addin file which contains addin functions

### removeAt(name) (1 of 2) {#removeat}

Removes the element at a specified name.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the element to remove. |

---

### removeAt(index) (2 of 2) {#removeat-1}

Removes the element at a specified index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The index value of the element to remove. |

### clear() {#clear}

Clear all worksheets.

A workbook must contains a worksheet.

### addCopy(sheetName) (1 of 3) {#addcopy}

Adds a worksheet to the collection and copies data from an existed worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | String | Name of source worksheet. |

**Returns:** Worksheet object index.

---

### addCopy(sheetIndex) (2 of 3) {#addcopy-1}

Adds a worksheet to the collection and copies data from an existed worksheet.

| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | Number | Index of source worksheet. |

**Returns:** Worksheet object index.

---

### addCopy(source, destSheetNames) (3 of 3) {#addcopy-2}

Copy a group of worksheets.

| Parameter | Type | Description |
| --- | --- | --- |
| source | Worksheet[] | The source worksheets. |
| destSheetNames | String[] | The names of the copied sheets. |

### getRangeByName(rangeName) (1 of 2) {#getrangebyname}

Gets Range object by pre-defined name.

| Parameter | Type | Description |
| --- | --- | --- |
| rangeName | String | Name of range. |

**Returns:** Range object. Returns null if the named range does not exist.

---

### getRangeByName(rangeName, currentSheetIndex, includeTable) (2 of 2) {#getrangebyname-1}

Gets Range by pre-defined name or table's name

| Parameter | Type | Description |
| --- | --- | --- |
| rangeName | String | Name of range or table's name. |
| currentSheetIndex | Number | The sheet index. -1 represents global . |
| includeTable | boolean | Indicates whether checking all tables. |

### getNamedRanges() {#getnamedranges}

Gets all pre-defined named ranges in the spreadsheet.

**Returns:** An array of Range objects. If the defined Name's reference is external or has multiple ranges, no Range object will be returned for this Name. Returns null if the named range does not exist.

### getNamedRangesAndTables() {#getnamedrangesandtables}

Gets all pre-defined named ranges in the spreadsheet.

**Returns:** An array of Range objects. Returns null if the named range does not exist.

### iterator() {#iterator}

### get(index) {#get}

Reserved for internal use.

### contains(value) {#contains}

Reserved for internal use.

### indexOf(value) {#indexof}

Reserved for internal use.
