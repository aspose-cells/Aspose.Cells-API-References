##WorksheetCollection
Encapsulates a collection of Worksheet..worksheet objects.
## WorksheetCollection class
Encapsulates a collection of [Worksheet](../worksheet/) objects.
```javascript
class WorksheetCollection;
```
### Example
```javascript
const { Workbook } = require("aspose.cells.node");
var workbook = new Workbook();
var sheets = workbook.worksheets;
//Add a worksheet
sheets.add();
//Change the name of a worksheet
sheets.get(0).name = "First Sheet";
//Set the active sheet to the second worksheet
sheets.activeSheetIndex = 1;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [webExtensionTaskPanes](#webExtensionTaskPanes--)| WebExtensionTaskPaneCollection | Readonly. Gets the list of task panes. |
| [webExtensions](#webExtensions--)| WebExtensionCollection | Readonly. Gets the list of task panes. |
| [threadedCommentAuthors](#threadedCommentAuthors--)| ThreadedCommentAuthorCollection | Readonly. Gets the list of threaded comment authors. |
| [isRefreshAllConnections](#isRefreshAllConnections--)| boolean | Indicates whether refresh all connections on opening file in MS Excel. |
| [names](#names--)| NameCollection | Readonly. Gets the collection of all the Name objects in the spreadsheet. |
| [activeSheetName](#activeSheetName--)| string | Represents the name of active worksheet when the spreadsheet is opened. |
| [activeSheetIndex](#activeSheetIndex--)| number | Represents the index of active worksheet when the spreadsheet is opened. |
| [dxfs](#dxfs--)| DxfCollection | Readonly. Gets the master differential formatting records. |
| [xmlMaps](#xmlMaps--)| XmlMapCollection | Gets and sets the XML maps in the workbook. |
| [builtInDocumentProperties](#builtInDocumentProperties--)| BuiltInDocumentPropertyCollection | Readonly. Returns a [DocumentProperty](../documentproperty/) collection that represents all the built-in document properties of the spreadsheet. |
| [customDocumentProperties](#customDocumentProperties--)| CustomDocumentPropertyCollection | Readonly. Returns a [DocumentProperty](../documentproperty/) collection that represents all the custom document properties of the spreadsheet. |
| [oleSize](#oleSize--)| Object | Gets and Sets displayed size when Workbook file is used as an Ole object. |
| [externalLinks](#externalLinks--)| ExternalLinkCollection | Readonly. Represents external links in a workbook. |
| [tableStyles](#tableStyles--)| TableStyleCollection | Readonly. Gets [TableStyles](../tablestyles/) object. |
| [revisionLogs](#revisionLogs--)| RevisionLogCollection | Readonly. Represents revision logs. |
| [sensitivityLabels](#sensitivityLabels--)| SensitivityLabelCollection | Readonly. Represents all sensitivity labels. |
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [Worksheet](../worksheet/) element at the specified index. |
| [get(string)](#get-string-)| Gets the [Worksheet](../worksheet/) element with the specified name. |
| [getWebExtensionTaskPanes()](#getWebExtensionTaskPanes--)| <b>@deprecated.</b> Please use the 'webExtensionTaskPanes' property instead. Gets the list of task panes. |
| [getWebExtensions()](#getWebExtensions--)| <b>@deprecated.</b> Please use the 'webExtensions' property instead. Gets the list of task panes. |
| [getThreadedCommentAuthors()](#getThreadedCommentAuthors--)| <b>@deprecated.</b> Please use the 'threadedCommentAuthors' property instead. Gets the list of threaded comment authors. |
| [isRefreshAllConnections()](#isRefreshAllConnections--)| <b>@deprecated.</b> Please use the 'isRefreshAllConnections' property instead. Indicates whether refresh all connections on opening file in MS Excel. |
| [setIsRefreshAllConnections(boolean)](#setIsRefreshAllConnections-boolean-)| <b>@deprecated.</b> Please use the 'isRefreshAllConnections' property instead. Indicates whether refresh all connections on opening file in MS Excel. |
| [getNames()](#getNames--)| <b>@deprecated.</b> Please use the 'names' property instead. Gets the collection of all the Name objects in the spreadsheet. |
| [getActiveSheetName()](#getActiveSheetName--)| <b>@deprecated.</b> Please use the 'activeSheetName' property instead. Represents the name of active worksheet when the spreadsheet is opened. |
| [setActiveSheetName(string)](#setActiveSheetName-string-)| <b>@deprecated.</b> Please use the 'activeSheetName' property instead. Represents the name of active worksheet when the spreadsheet is opened. |
| [getActiveSheetIndex()](#getActiveSheetIndex--)| <b>@deprecated.</b> Please use the 'activeSheetIndex' property instead. Represents the index of active worksheet when the spreadsheet is opened. |
| [setActiveSheetIndex(number)](#setActiveSheetIndex-number-)| <b>@deprecated.</b> Please use the 'activeSheetIndex' property instead. Represents the index of active worksheet when the spreadsheet is opened. |
| [getDxfs()](#getDxfs--)| <b>@deprecated.</b> Please use the 'dxfs' property instead. Gets the master differential formatting records. |
| [getXmlMaps()](#getXmlMaps--)| <b>@deprecated.</b> Please use the 'xmlMaps' property instead. Gets and sets the XML maps in the workbook. |
| [setXmlMaps(XmlMapCollection)](#setXmlMaps-xmlmapcollection-)| <b>@deprecated.</b> Please use the 'xmlMaps' property instead. Gets and sets the XML maps in the workbook. |
| [getBuiltInDocumentProperties()](#getBuiltInDocumentProperties--)| <b>@deprecated.</b> Please use the 'builtInDocumentProperties' property instead. Returns a [DocumentProperty](../documentproperty/) collection that represents all the built-in document properties of the spreadsheet. |
| [getCustomDocumentProperties()](#getCustomDocumentProperties--)| <b>@deprecated.</b> Please use the 'customDocumentProperties' property instead. Returns a [DocumentProperty](../documentproperty/) collection that represents all the custom document properties of the spreadsheet. |
| [getOleSize()](#getOleSize--)| <b>@deprecated.</b> Please use the 'oleSize' property instead. Gets and Sets displayed size when Workbook file is used as an Ole object. |
| [setOleSize(Object)](#setOleSize-object-)| <b>@deprecated.</b> Please use the 'oleSize' property instead. Gets and Sets displayed size when Workbook file is used as an Ole object. |
| [getExternalLinks()](#getExternalLinks--)| <b>@deprecated.</b> Please use the 'externalLinks' property instead. Represents external links in a workbook. |
| [getTableStyles()](#getTableStyles--)| <b>@deprecated.</b> Please use the 'tableStyles' property instead. Gets [TableStyles](../tablestyles/) object. |
| [getRevisionLogs()](#getRevisionLogs--)| <b>@deprecated.</b> Please use the 'revisionLogs' property instead. Represents revision logs. |
| [getSensitivityLabels()](#getSensitivityLabels--)| <b>@deprecated.</b> Please use the 'sensitivityLabels' property instead. Represents all sensitivity labels. |
| [createRange(string, number)](#createRange-string-number-)| Creates a [Range](../range/) object from an address of the range. |
| [createUnionRange(string, number)](#createUnionRange-string-number-)| Creates a [Range](../range/) object from an address of the range. |
| [getSheetByCodeName(string)](#getSheetByCodeName-string-)| Gets the worksheet by the code name. |
| [sortNames()](#sortNames--)| Sorts the defined names. |
| [insert(number, SheetType)](#insert-number-sheettype-)| Insert a worksheet. |
| [insert(number, SheetType, string)](#insert-number-sheettype-string-)| Insert a worksheet. |
| [add(SheetType)](#add-sheettype-)| Adds a worksheet to the collection. |
| [add()](#add--)| Adds a worksheet to the collection. |
| [add(string)](#add-string-)| Adds a worksheet to the collection. |
| [swapSheet(number, number)](#swapSheet-number-number-)| Swaps the two sheets. |
| [registerAddInFunction(string, string, boolean)](#registerAddInFunction-string-string-boolean-)| Adds addin function into the workbook |
| [registerAddInFunction(number, string)](#registerAddInFunction-number-string-)| Adds addin function into the workbook |
| [removeAt(string)](#removeAt-string-)| Removes the element at a specified name. |
| [removeAt(number)](#removeAt-number-)| Removes the element at a specified index. |
| [clear()](#clear--)| Clear all worksheets. |
| [addCopy(string)](#addCopy-string-)| Adds a worksheet to the collection and copies data from an existed worksheet. |
| [addCopy(number)](#addCopy-number-)| Adds a worksheet to the collection and copies data from an existed worksheet. |
| [addCopy(Worksheet[], string[])](#addCopy-worksheetarray-stringarray-)| Copy a group of worksheets. |
| [getRangeByName(string)](#getRangeByName-string-)| Gets Range object by pre-defined name. |
| [getRangeByName(string, number, boolean)](#getRangeByName-string-number-boolean-)| Gets [Range](../range/) by pre-defined name or table's name |
| [getNamedRanges()](#getNamedRanges--)| Gets all pre-defined named ranges in the spreadsheet. |
| [getNamedRangesAndTables()](#getNamedRangesAndTables--)| Gets all pre-defined named ranges in the spreadsheet. |
| [setOleSize(number, number, number, number)](#setOleSize-number-number-number-number-)| Sets displayed size when Workbook file is used as an Ole object. |
| [clearPivottables()](#clearPivottables--)| Clears pivot tables from the spreadsheet. |
| [refreshAll()](#refreshAll--)| Refresh all pivot tables and charts with pivot source. |
| [refreshAllAsync()](#refreshAllAsync--)| Refresh all pivot tables and charts with pivot source. |
| [refreshPivotTables()](#refreshPivotTables--)| Refreshes all the PivotTables in the Excel file. |
| [refreshPivotTables(PivotTableRefreshOption)](#refreshPivotTables-pivottablerefreshoption-)| Refreshes all the PivotTables in the Excel file. |
| [refreshPivotTablesAsync()](#refreshPivotTablesAsync--)| Refreshes all the PivotTables in the Excel file. |
| [refreshPivotTablesAsync(PivotTableRefreshOption)](#refreshPivotTablesAsync-pivottablerefreshoption-)| Refreshes all the PivotTables in the Excel file. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### webExtensionTaskPanes {#webExtensionTaskPanes--}
Readonly. Gets the list of task panes.
```javascript
webExtensionTaskPanes : WebExtensionTaskPaneCollection;
```
### webExtensions {#webExtensions--}
Readonly. Gets the list of task panes.
```javascript
webExtensions : WebExtensionCollection;
```
### threadedCommentAuthors {#threadedCommentAuthors--}
Readonly. Gets the list of threaded comment authors.
```javascript
threadedCommentAuthors : ThreadedCommentAuthorCollection;
```
### isRefreshAllConnections {#isRefreshAllConnections--}
Indicates whether refresh all connections on opening file in MS Excel.
```javascript
isRefreshAllConnections : boolean;
```
### names {#names--}
Readonly. Gets the collection of all the Name objects in the spreadsheet.
```javascript
names : NameCollection;
```
### activeSheetName {#activeSheetName--}
Represents the name of active worksheet when the spreadsheet is opened.
```javascript
activeSheetName : string;
```
### activeSheetIndex {#activeSheetIndex--}
Represents the index of active worksheet when the spreadsheet is opened.
```javascript
activeSheetIndex : number;
```
**Remarks**
Sheet index is zero based.
### dxfs {#dxfs--}
Readonly. Gets the master differential formatting records.
```javascript
dxfs : DxfCollection;
```
### xmlMaps {#xmlMaps--}
Gets and sets the XML maps in the workbook.
```javascript
xmlMaps : XmlMapCollection;
```
### builtInDocumentProperties {#builtInDocumentProperties--}
Readonly. Returns a [DocumentProperty](../documentproperty/) collection that represents all the built-in document properties of the spreadsheet.
```javascript
builtInDocumentProperties : BuiltInDocumentPropertyCollection;
```
**Remarks**
A new property cannot be added to built-in document properties list. You can only get a built-in property and change its value. The following is the built-in properties name list: <p>Title</p> <p>Subject</p> <p>Author</p> <p>Keywords</p> <p>Comments</p> <p>Template</p> <p>Last Author</p> <p>Revision Number</p> <p>Application Name</p> <p>Last Print Date</p> <p>Creation Date</p> <p>Last Save Time</p> <p>Total Editing Time</p> <p>Number of Pages</p> <p>Number of Words</p> <p>Number of Characters</p> <p>Security</p> <p>Category</p> <p>Format</p> <p>Manager</p> <p>Company</p> <p>Number of Bytes</p> <p>Number of Lines</p> <p>Number of Paragraphs</p> <p>Number of Slides</p> <p>Number of Notes</p> <p>Number of Hidden Slides</p> <p>Number of Multimedia Clips
**Example**
```javascript
const { Workbook } = require("aspose.cells.node");
var workbook = new Workbook();
var doc = workbook.worksheets.builtInDocumentProperties.get("Author");
doc.value = "John Smith";
```
### customDocumentProperties {#customDocumentProperties--}
Readonly. Returns a [DocumentProperty](../documentproperty/) collection that represents all the custom document properties of the spreadsheet.
```javascript
customDocumentProperties : CustomDocumentPropertyCollection;
```
**Example**
```javascript
const { Workbook } = require("aspose.cells.node");
var excel = new Workbook();
excel.worksheets.customDocumentProperties.add("Checked by", "Jane");
```
### oleSize {#oleSize--}
Gets and Sets displayed size when Workbook file is used as an Ole object.
```javascript
oleSize : Object;
```
**Remarks**
Null means no ole size setting.
### externalLinks {#externalLinks--}
Readonly. Represents external links in a workbook.
```javascript
externalLinks : ExternalLinkCollection;
```
### tableStyles {#tableStyles--}
Readonly. Gets [TableStyles](../tablestyles/) object.
```javascript
tableStyles : TableStyleCollection;
```
### revisionLogs {#revisionLogs--}
Readonly. Represents revision logs.
```javascript
revisionLogs : RevisionLogCollection;
```
### sensitivityLabels {#sensitivityLabels--}
Readonly. Represents all sensitivity labels.
```javascript
sensitivityLabels : SensitivityLabelCollection;
```
### get(number) {#get-number-}
Gets the [Worksheet](../worksheet/) element at the specified index.
```javascript
get(index: number) : Worksheet;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The zero based index of the element. |
**Returns**
The element at the specified index.
### get(string) {#get-string-}
Gets the [Worksheet](../worksheet/) element with the specified name.
```javascript
get(sheetName: string) : Worksheet;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | string | Worksheet name |
**Returns**
The element with the specified name.
### getWebExtensionTaskPanes() {#getWebExtensionTaskPanes--}
```javascript
getWebExtensionTaskPanes() : WebExtensionTaskPaneCollection;
```
**Returns**
[WebExtensionTaskPaneCollection](../webextensiontaskpanecollection/)
### getWebExtensions() {#getWebExtensions--}
```javascript
getWebExtensions() : WebExtensionCollection;
```
**Returns**
[WebExtensionCollection](../webextensioncollection/)
### getThreadedCommentAuthors() {#getThreadedCommentAuthors--}
```javascript
getThreadedCommentAuthors() : ThreadedCommentAuthorCollection;
```
**Returns**
[ThreadedCommentAuthorCollection](../threadedcommentauthorcollection/)
### isRefreshAllConnections() {#isRefreshAllConnections--}
```javascript
isRefreshAllConnections() : boolean;
```
### setIsRefreshAllConnections(boolean) {#setIsRefreshAllConnections-boolean-}
```javascript
setIsRefreshAllConnections(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getNames() {#getNames--}
```javascript
getNames() : NameCollection;
```
**Returns**
[NameCollection](../namecollection/)
### getActiveSheetName() {#getActiveSheetName--}
```javascript
getActiveSheetName() : string;
```
### setActiveSheetName(string) {#setActiveSheetName-string-}
```javascript
setActiveSheetName(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getActiveSheetIndex() {#getActiveSheetIndex--}
```javascript
getActiveSheetIndex() : number;
```
**Remarks**
Sheet index is zero based.
### setActiveSheetIndex(number) {#setActiveSheetIndex-number-}
```javascript
setActiveSheetIndex(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
Sheet index is zero based.
### getDxfs() {#getDxfs--}
```javascript
getDxfs() : DxfCollection;
```
**Returns**
[DxfCollection](../dxfcollection/)
### getXmlMaps() {#getXmlMaps--}
```javascript
getXmlMaps() : XmlMapCollection;
```
**Returns**
[XmlMapCollection](../xmlmapcollection/)
### setXmlMaps(XmlMapCollection) {#setXmlMaps-xmlmapcollection-}
```javascript
setXmlMaps(value: XmlMapCollection) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [XmlMapCollection](../xmlmapcollection/) | The value to set. |
### getBuiltInDocumentProperties() {#getBuiltInDocumentProperties--}
```javascript
getBuiltInDocumentProperties() : BuiltInDocumentPropertyCollection;
```
**Returns**
[BuiltInDocumentPropertyCollection](../builtindocumentpropertycollection/)
**Remarks**
A new property cannot be added to built-in document properties list. You can only get a built-in property and change its value. The following is the built-in properties name list: <p>Title</p> <p>Subject</p> <p>Author</p> <p>Keywords</p> <p>Comments</p> <p>Template</p> <p>Last Author</p> <p>Revision Number</p> <p>Application Name</p> <p>Last Print Date</p> <p>Creation Date</p> <p>Last Save Time</p> <p>Total Editing Time</p> <p>Number of Pages</p> <p>Number of Words</p> <p>Number of Characters</p> <p>Security</p> <p>Category</p> <p>Format</p> <p>Manager</p> <p>Company</p> <p>Number of Bytes</p> <p>Number of Lines</p> <p>Number of Paragraphs</p> <p>Number of Slides</p> <p>Number of Notes</p> <p>Number of Hidden Slides</p> <p>Number of Multimedia Clips
### getCustomDocumentProperties() {#getCustomDocumentProperties--}
```javascript
getCustomDocumentProperties() : CustomDocumentPropertyCollection;
```
**Returns**
[CustomDocumentPropertyCollection](../customdocumentpropertycollection/)
### getOleSize() {#getOleSize--}
```javascript
getOleSize() : Object;
```
**Remarks**
Null means no ole size setting.
### setOleSize(Object) {#setOleSize-object-}
```javascript
setOleSize(value: Object) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Object | The value to set. |
**Remarks**
Null means no ole size setting.
### getExternalLinks() {#getExternalLinks--}
```javascript
getExternalLinks() : ExternalLinkCollection;
```
**Returns**
[ExternalLinkCollection](../externallinkcollection/)
### getTableStyles() {#getTableStyles--}
```javascript
getTableStyles() : TableStyleCollection;
```
**Returns**
[TableStyleCollection](../tablestylecollection/)
### getRevisionLogs() {#getRevisionLogs--}
```javascript
getRevisionLogs() : RevisionLogCollection;
```
**Returns**
[RevisionLogCollection](../revisionlogcollection/)
### getSensitivityLabels() {#getSensitivityLabels--}
```javascript
getSensitivityLabels() : SensitivityLabelCollection;
```
**Returns**
[SensitivityLabelCollection](../sensitivitylabelcollection/)
### createRange(string, number) {#createRange-string-number-}
Creates a [Range](../range/) object from an address of the range.
```javascript
createRange(address: string, sheetIndex: number) : Range;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| address | string | The address of the range. |
| sheetIndex | number | The sheet index. |
**Returns**
A [Range](../range/) object
### createUnionRange(string, number) {#createUnionRange-string-number-}
Creates a [Range](../range/) object from an address of the range.
```javascript
createUnionRange(address: string, sheetIndex: number) : UnionRange;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| address | string | The address of the range. |
| sheetIndex | number | The sheet index. |
**Returns**
A [Range](../range/) object
### getSheetByCodeName(string) {#getSheetByCodeName-string-}
Gets the worksheet by the code name.
```javascript
getSheetByCodeName(codeName: string) : Worksheet;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| codeName | string | Worksheet code name. |
**Returns**
The element with the specified code name.
### sortNames() {#sortNames--}
Sorts the defined names.
```javascript
sortNames() : void;
```
**Remarks**
If you create a large amount of named ranges in the Excel file, please call this method after all named ranges are created and before saving
### insert(number, SheetType) {#insert-number-sheettype-}
Insert a worksheet.
```javascript
insert(index: number, sheetType: SheetType) : Worksheet;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The sheet index |
| sheetType | [SheetType](../sheettype/) | The sheet type. |
**Returns**
Returns an inserted worksheet.
### insert(number, SheetType, string) {#insert-number-sheettype-string-}
Insert a worksheet.
```javascript
insert(index: number, sheetType: SheetType, sheetName: string) : Worksheet;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The sheet index |
| sheetType | [SheetType](../sheettype/) | The sheet type. |
| sheetName | string | The sheet name. |
**Returns**
Returns an inserted worksheet.
### add(SheetType) {#add-sheettype-}
Adds a worksheet to the collection.
```javascript
add(type: SheetType) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [SheetType](../sheettype/) | Worksheet type. |
**Returns**
[Worksheet](../worksheet/) object index.
**Example**
```javascript
const { Workbook, SheetType, ChartType } = require("aspose.cells.node");
var workbook = new Workbook();
workbook.worksheets.add(SheetType.Chart);
var cells = workbook.worksheets.get(0).cells;
cells.get("c2").putValue(5000);
cells.get("c3").putValue(3000);
cells.get("c4").putValue(4000);
cells.get("c5").putValue(5000);
cells.get("c6").putValue(6000);
var charts = workbook.worksheets.get(1).charts;
var chartIndex = charts.add(ChartType.Column, 10, 10, 20, 20);
var chart = charts.get(chartIndex);
chart.nSeries.add("Sheet1!C2:C6", true);
```
### add() {#add--}
Adds a worksheet to the collection.
```javascript
add() : number;
```
**Returns**
[Worksheet](../worksheet/) object index.
### add(string) {#add-string-}
Adds a worksheet to the collection.
```javascript
add(sheetName: string) : Worksheet;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | string | Worksheet name |
**Returns**
[Worksheet](../worksheet/) object.
### swapSheet(number, number) {#swapSheet-number-number-}
Swaps the two sheets.
```javascript
swapSheet(sheetIndex1: number, sheetIndex2: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex1 | number | The first worksheet. |
| sheetIndex2 | number | The second worksheet. |
### registerAddInFunction(string, string, boolean) {#registerAddInFunction-string-string-boolean-}
Adds addin function into the workbook
```javascript
registerAddInFunction(addInFile: string, functionName: string, lib: boolean) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| addInFile | string | the file contains the addin functions |
| functionName | string | the addin function name |
| lib | boolean | whether the given addin file is in the directory or sub-directory of Workbook Add-In library.         /// This flag takes effect and makes difference when given addInFile is of relative path:         /// true denotes the path is relative to Add-In library and false denotes the path is relative to this Workbook. |
**Returns**
ID of the data which contains given addin function
### registerAddInFunction(number, string) {#registerAddInFunction-number-string-}
Adds addin function into the workbook
```javascript
registerAddInFunction(id: number, functionName: string) : string;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| id | number | ID of the data which contains addin functions,         /// can be got by the first call of [RegisterAddInFunction(string, string, bool)](../registeraddinfunction(string, string, bool)/) for the same addin file. |
| functionName | string | the addin function name |
**Returns**
URL of the addin file which contains addin functions
### removeAt(string) {#removeAt-string-}
Removes the element at a specified name.
```javascript
removeAt(name: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The name of the element to remove. |
### removeAt(number) {#removeAt-number-}
Removes the element at a specified index.
```javascript
removeAt(index: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index value of the element to remove. |
### clear() {#clear--}
Clear all worksheets.
```javascript
clear() : void;
```
**Remarks**
A workbook must contains a worksheet.
### addCopy(string) {#addCopy-string-}
Adds a worksheet to the collection and copies data from an existed worksheet.
```javascript
addCopy(sheetName: string) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | string | Name of source worksheet. |
**Returns**
[Worksheet](../worksheet/) object index.
### addCopy(number) {#addCopy-number-}
Adds a worksheet to the collection and copies data from an existed worksheet.
```javascript
addCopy(sheetIndex: number) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | number | Index of source worksheet. |
**Returns**
[Worksheet](../worksheet/) object index.
### addCopy(Worksheet[], string[]) {#addCopy-worksheetarray-stringarray-}
Copy a group of worksheets.
```javascript
addCopy(source: Worksheet[], destSheetNames: string[]) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | [Worksheet](../worksheet/)[] | The source worksheets. |
| destSheetNames | string[] | The names of the copied sheets. |
### getRangeByName(string) {#getRangeByName-string-}
Gets Range object by pre-defined name.
```javascript
getRangeByName(rangeName: string) : Range;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rangeName | string | Name of range. |
**Returns**
Range object.<p></p>Returns null if the named range does not exist.
### getRangeByName(string, number, boolean) {#getRangeByName-string-number-boolean-}
Gets [Range](../range/) by pre-defined name or table's name
```javascript
getRangeByName(rangeName: string, currentSheetIndex: number, includeTable: boolean) : Range;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rangeName | string | Name of range or table's name. |
| currentSheetIndex | number | The sheet index. -1 represents global . |
| includeTable | boolean | Indicates whether checking all tables. |
**Returns**
[Range](../range/)
### getNamedRanges() {#getNamedRanges--}
Gets all pre-defined named ranges in the spreadsheet.
```javascript
getNamedRanges() : Range[];
```
**Returns**
An array of Range objects. If the defined Name's reference is external or has multiple ranges, no Range object will be returned for this Name. <p></p>Returns null if the named range does not exist.
### getNamedRangesAndTables() {#getNamedRangesAndTables--}
Gets all pre-defined named ranges in the spreadsheet.
```javascript
getNamedRangesAndTables() : Range[];
```
**Returns**
An array of Range objects.<p></p>Returns null if the named range does not exist.
### setOleSize(number, number, number, number) {#setOleSize-number-number-number-number-}
Sets displayed size when Workbook file is used as an Ole object.
```javascript
setOleSize(startRow: number, endRow: number, startColumn: number, endColumn: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | number | Start row index. |
| endRow | number | End row index. |
| startColumn | number | Start column index. |
| endColumn | number | End column index. |
**Remarks**
This method is generally used to adjust display size in ppt file or doc file.
### clearPivottables() {#clearPivottables--}
Clears pivot tables from the spreadsheet.
```javascript
clearPivottables() : void;
```
### refreshAll() {#refreshAll--}
Refresh all pivot tables and charts with pivot source.
```javascript
refreshAll() : void;
```
### refreshAllAsync() {#refreshAllAsync--}
Refresh all pivot tables and charts with pivot source.
```javascript
refreshAllAsync() : Promise<void>;
```
**Returns**
[Promise<void>](../promise<void>/)
### refreshPivotTables() {#refreshPivotTables--}
Refreshes all the PivotTables in the Excel file.
```javascript
refreshPivotTables() : void;
```
### refreshPivotTables(PivotTableRefreshOption) {#refreshPivotTables-pivottablerefreshoption-}
Refreshes all the PivotTables in the Excel file.
```javascript
refreshPivotTables(option: PivotTableRefreshOption) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../pivottablerefreshoption/) | The option for refreshing data source of the pivot tables. |
### refreshPivotTablesAsync() {#refreshPivotTablesAsync--}
Refreshes all the PivotTables in the Excel file.
```javascript
refreshPivotTablesAsync() : Promise<void>;
```
**Returns**
[Promise<void>](../promise<void>/)
### refreshPivotTablesAsync(PivotTableRefreshOption) {#refreshPivotTablesAsync-pivottablerefreshoption-}
Refreshes all the PivotTables in the Excel file.
```javascript
refreshPivotTablesAsync(option: PivotTableRefreshOption) : Promise<boolean>;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../pivottablerefreshoption/) | The option for refreshing data source of the pivot tables. |
**Returns**
[Promise<boolean>](../promise<boolean>/)
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
