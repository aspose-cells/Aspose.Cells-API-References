##WorksheetCollection
Encapsulates a collection of  objects.
**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class WorksheetCollection extends CollectionBase
```
Encapsulates a collection of [Range.getWorksheet()](../../com.aspose.cells/range\#getWorksheet--) objects.
**Example**
```
Workbook workbook = new Workbook();
WorksheetCollection sheets = workbook.getWorksheets();
//Add a worksheet
sheets.add();
//Change the name of a worksheet
sheets.get(0).setName("First Sheet");
//Set the active sheet to the second worksheet
sheets.setActiveSheetIndex(1);
```
## Methods
| Method | Description |
| --- | --- |
| [add()](#add--) | Adds a worksheet to the collection. |
| [add(int type)](#add-int-) | Adds a worksheet to the collection. |
| [add(Object o)](#add-java.lang.Object-) | Adds an item to the CollectionBase instance. |
| [add(String sheetName)](#add-java.lang.String-) | Adds a worksheet to the collection. |
| [addCopy(Worksheet[] source, String[] destSheetNames)](#addCopy-com.aspose.cells.Worksheet---java.lang.String---) | Copy a group of worksheets. |
| [addCopy(int sheetIndex)](#addCopy-int-) | Adds a worksheet to the collection and copies data from an existed worksheet. |
| [addCopy(String sheetName)](#addCopy-java.lang.String-) | Adds a worksheet to the collection and copies data from an existed worksheet. |
| [clear()](#clear--) | Clear all worksheets. |
| [clearPivottables()](#clearPivottables--) | Clears pivot tables from the spreadsheet. |
| [contains(Object o)](#contains-java.lang.Object-) | Return whether instance contains this object |
| [createRange(String address, int sheetIndex)](#createRange-java.lang.String-int-) | Creates a [Range](../../com.aspose.cells/range) object from an address of the range. |
| [createUnionRange(String address, int sheetIndex)](#createUnionRange-java.lang.String-int-) | Creates a [Range](../../com.aspose.cells/range) object from an address of the range. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gets the [Range.getWorksheet()](../../com.aspose.cells/range\#getWorksheet--) element at the specified index. |
| [get(String sheetName)](#get-java.lang.String-) | Gets the [Range.getWorksheet()](../../com.aspose.cells/range\#getWorksheet--) element with the specified name. |
| [getActiveSheetIndex()](#getActiveSheetIndex--) | Represents the index of active worksheet when the spreadsheet is opened. |
| [getActiveSheetName()](#getActiveSheetName--) | Represents the name of active worksheet when the spreadsheet is opened. |
| [getBuiltInDocumentProperties()](#getBuiltInDocumentProperties--) | Returns a [DocumentProperty](../../com.aspose.cells/documentproperty) collection that represents all the built-in document properties of the spreadsheet. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Gets the number of elements contained in the CollectionBase instance. |
| [getCustomDocumentProperties()](#getCustomDocumentProperties--) | Returns a [DocumentProperty](../../com.aspose.cells/documentproperty) collection that represents all the custom document properties of the spreadsheet. |
| [getDxfs()](#getDxfs--) | Gets the master differential formatting records. |
| [getExternalLinks()](#getExternalLinks--) | Represents external links in a workbook. |
| [getNamedRanges()](#getNamedRanges--) | Gets all pre-defined named ranges in the spreadsheet. |
| [getNamedRangesAndTables()](#getNamedRangesAndTables--) | Gets all pre-defined named ranges in the spreadsheet. |
| [getNames()](#getNames--) | Gets the collection of all the Name objects in the spreadsheet. |
| [getOleSize()](#getOleSize--) | Gets displayed size when Workbook file is used as an Ole object. |
| [getRangeByName(String rangeName)](#getRangeByName-java.lang.String-) | Gets Range object by pre-defined name. |
| [getRangeByName(String rangeName, int currentSheetIndex, boolean includeTable)](#getRangeByName-java.lang.String-int-boolean-) | Gets [Range](../../com.aspose.cells/range) by pre-defined name or table's name |
| [getRevisionLogs()](#getRevisionLogs--) | Represents revision logs. |
| [getSensitivityLabels()](#getSensitivityLabels--) | Represents all sensitivity labels. |
| [getSheetByCodeName(String codeName)](#getSheetByCodeName-java.lang.String-) | Gets the worksheet by the code name. |
| [getTableStyles()](#getTableStyles--) | Gets [getTableStyles()](../../com.aspose.cells/worksheetcollection\#getTableStyles--) object. |
| [getThreadedCommentAuthors()](#getThreadedCommentAuthors--) | Gets the list of threaded comment authors. |
| [getWebExtensionTaskPanes()](#getWebExtensionTaskPanes--) | Gets the list of task panes. |
| [getWebExtensions()](#getWebExtensions--) | Gets the list of task panes. |
| [getXmlMaps()](#getXmlMaps--) | Gets the XML maps in the workbook. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determines the index of a specific item in the CollectionBase instance. |
| [insert(int index, int sheetType)](#insert-int-int-) | Insert a worksheet. |
| [insert(int index, int sheetType, String sheetName)](#insert-int-int-java.lang.String-) | Insert a worksheet. |
| [isRefreshAllConnections()](#isRefreshAllConnections--) | Indicates whether refresh all connections on opening file in MS Excel. |
| [iterator()](#iterator--) | Returns an enumerator that iterates through the CollectionBase instance. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshAll()](#refreshAll--) | Refresh all pivot tables and charts with pivot source. |
| [refreshPivotTables()](#refreshPivotTables--) | Refreshes all the PivotTables in the Excel file. |
| [refreshPivotTables(PivotTableRefreshOption option)](#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-) | Refreshes all the PivotTables in the Excel file. |
| [registerAddInFunction(int id, String functionName)](#registerAddInFunction-int-java.lang.String-) | Adds addin function into the workbook |
| [registerAddInFunction(String addInFile, String functionName, boolean lib)](#registerAddInFunction-java.lang.String-java.lang.String-boolean-) | Adds addin function into the workbook |
| [removeAt(int index)](#removeAt-int-) | Removes the element at a specified index. |
| [removeAt(String name)](#removeAt-java.lang.String-) | Removes the element at a specified name. |
| [setActiveSheetIndex(int value)](#setActiveSheetIndex-int-) | Represents the index of active worksheet when the spreadsheet is opened. |
| [setActiveSheetName(String value)](#setActiveSheetName-java.lang.String-) | Represents the name of active worksheet when the spreadsheet is opened. |
| [setOleSize(int startRow, int endRow, int startColumn, int endColumn)](#setOleSize-int-int-int-int-) | Sets displayed size when Workbook file is used as an Ole object. |
| [setOleSize(Object value)](#setOleSize-java.lang.Object-) | Sets displayed size when Workbook file is used as an Ole object. |
| [setRefreshAllConnections(boolean value)](#setRefreshAllConnections-boolean-) | Indicates whether refresh all connections on opening file in MS Excel. |
| [setXmlMaps(XmlMapCollection value)](#setXmlMaps-com.aspose.cells.XmlMapCollection-) | Sets the XML maps in the workbook. |
| [sortNames()](#sortNames--) | Sorts the defined names. |
| [swapSheet(int sheetIndex1, int sheetIndex2)](#swapSheet-int-int-) | Swaps the two sheets. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add() {#add--}
```
public int add()
```
Adds a worksheet to the collection.
**Returns:**
int - [Range.getWorksheet()](../../com.aspose.cells/range\#getWorksheet--) object index.
### add(int type) {#add-int-}
```
public int add(int type)
```
Adds a worksheet to the collection.
**Example**
```
Workbook workbook = new Workbook();
workbook.getWorksheets().add(SheetType.CHART);
Cells cells = workbook.getWorksheets().get(0).getCells();
cells.get("c2").putValue(5000);
cells.get("c3").putValue(3000);
cells.get("c4").putValue(4000);
cells.get("c5").putValue(5000);
cells.get("c6").putValue(6000);
ChartCollection charts = workbook.getWorksheets().get(1).getCharts();
int chartIndex = charts.add(ChartType.COLUMN, 10,10,20,20);
Chart chart = charts.get(chartIndex);
chart.getNSeries().add("Sheet1!C2:C6", true);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | [SheetType](../../com.aspose.cells/sheettype). Worksheet type. |
**Returns:**
int - [Range.getWorksheet()](../../com.aspose.cells/range\#getWorksheet--) object index.
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```
Adds an item to the CollectionBase instance.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | The Object to add to the CollectionBase instance. |
**Returns:**
int - The position into which the new element was inserted.
### add(String sheetName) {#add-java.lang.String-}
```
public Worksheet add(String sheetName)
```
Adds a worksheet to the collection.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | java.lang.String | Worksheet name |
**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - [Range.getWorksheet()](../../com.aspose.cells/range\#getWorksheet--) object.
### addCopy(Worksheet[] source, String[] destSheetNames) {#addCopy-com.aspose.cells.Worksheet---java.lang.String---}
```
public void addCopy(Worksheet[] source, String[] destSheetNames)
```
Copy a group of worksheets.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | [Worksheet\[\]](../../com.aspose.cells/worksheet) | The source worksheets. |
| destSheetNames | java.lang.String[] | The names of the copied sheets. |
### addCopy(int sheetIndex) {#addCopy-int-}
```
public int addCopy(int sheetIndex)
```
Adds a worksheet to the collection and copies data from an existed worksheet.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | int | Index of source worksheet. |
**Returns:**
int - [Range.getWorksheet()](../../com.aspose.cells/range\#getWorksheet--) object index.
### addCopy(String sheetName) {#addCopy-java.lang.String-}
```
public int addCopy(String sheetName)
```
Adds a worksheet to the collection and copies data from an existed worksheet.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | java.lang.String | Name of source worksheet. |
**Returns:**
int - [Range.getWorksheet()](../../com.aspose.cells/range\#getWorksheet--) object index.
### clear() {#clear--}
```
public void clear()
```
Clear all worksheets.
**Remarks**
A workbook must contains a worksheet.
### clearPivottables() {#clearPivottables--}
```
public void clearPivottables()
```
Clears pivot tables from the spreadsheet.
### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```
Return whether instance contains this object
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | test object |
**Returns:**
boolean - Whether instance contains this object
### createRange(String address, int sheetIndex) {#createRange-java.lang.String-int-}
```
public Range createRange(String address, int sheetIndex)
```
Creates a [Range](../../com.aspose.cells/range) object from an address of the range.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| address | java.lang.String | The address of the range. |
| sheetIndex | int | The sheet index. |
**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### createUnionRange(String address, int sheetIndex) {#createUnionRange-java.lang.String-int-}
```
public UnionRange createUnionRange(String address, int sheetIndex)
```
Creates a [Range](../../com.aspose.cells/range) object from an address of the range.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| address | java.lang.String | The address of the range. |
| sheetIndex | int | The sheet index. |
**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - A [Range](../../com.aspose.cells/range) object
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |
**Returns:**
boolean
### get(int index) {#get-int-}
```
public Worksheet get(int index)
```
Gets the [Range.getWorksheet()](../../com.aspose.cells/range\#getWorksheet--) element at the specified index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero based index of the element. |
**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - The element at the specified index.
### get(String sheetName) {#get-java.lang.String-}
```
public Worksheet get(String sheetName)
```
Gets the [Range.getWorksheet()](../../com.aspose.cells/range\#getWorksheet--) element with the specified name.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | java.lang.String | Worksheet name |
**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - The element with the specified name.
### getActiveSheetIndex() {#getActiveSheetIndex--}
```
public int getActiveSheetIndex()
```
Represents the index of active worksheet when the spreadsheet is opened.
**Remarks**
Sheet index is zero based.
**Returns:**
int
### getActiveSheetName() {#getActiveSheetName--}
```
public String getActiveSheetName()
```
Represents the name of active worksheet when the spreadsheet is opened.
**Returns:**
java.lang.String
### getBuiltInDocumentProperties() {#getBuiltInDocumentProperties--}
```
public BuiltInDocumentPropertyCollection getBuiltInDocumentProperties()
```
Returns a [DocumentProperty](../../com.aspose.cells/documentproperty) collection that represents all the built-in document properties of the spreadsheet.
**Remarks**
A new property cannot be added to built-in document properties list. You can only get a built-in property and change its value. The following is the built-in properties name list:
Title
Subject
Author
Keywords
Comments
Template
Last Author
Revision Number
Application Name
Last Print Date
Creation Date
Last Save Time
Total Editing Time
Number of Pages
Number of Words
Number of Characters
Security
Category
Format
Manager
Company
Number of Bytes
Number of Lines
Number of Paragraphs
Number of Slides
Number of Notes
Number of Hidden Slides
Number of Multimedia Clips
**Example**
```
Workbook workbook = new Workbook();
DocumentProperty doc = workbook.getWorksheets().getBuiltInDocumentProperties().get("Author");
doc.setValue("John Smith");
```
**Returns:**
[BuiltInDocumentPropertyCollection](../../com.aspose.cells/builtindocumentpropertycollection)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```
Gets the number of elements contained in the CollectionBase instance.
**Returns:**
int - The number of elements contained in the CollectionBase instance.
### getCustomDocumentProperties() {#getCustomDocumentProperties--}
```
public CustomDocumentPropertyCollection getCustomDocumentProperties()
```
Returns a [DocumentProperty](../../com.aspose.cells/documentproperty) collection that represents all the custom document properties of the spreadsheet.
**Example**
```
Workbook workbook = new Workbook();
workbook.getWorksheets().getCustomDocumentProperties().add("Checked by", "Jane");
```
**Returns:**
[CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection)
### getDxfs() {#getDxfs--}
```
public DxfCollection getDxfs()
```
Gets the master differential formatting records.
**Returns:**
[DxfCollection](../../com.aspose.cells/dxfcollection)
### getExternalLinks() {#getExternalLinks--}
```
public ExternalLinkCollection getExternalLinks()
```
Represents external links in a workbook.
**Returns:**
[ExternalLinkCollection](../../com.aspose.cells/externallinkcollection)
### getNamedRanges() {#getNamedRanges--}
```
public Range[] getNamedRanges()
```
Gets all pre-defined named ranges in the spreadsheet.
**Returns:**
com.aspose.cells.Range[] - An array of Range objects. If the defined Name's reference is external or has multiple ranges, no Range object will be returned for this Name.
Returns null if the named range does not exist.
### getNamedRangesAndTables() {#getNamedRangesAndTables--}
```
public Range[] getNamedRangesAndTables()
```
Gets all pre-defined named ranges in the spreadsheet.
**Returns:**
com.aspose.cells.Range[] - An array of Range objects.
Returns null if the named range does not exist.
### getNames() {#getNames--}
```
public NameCollection getNames()
```
Gets the collection of all the Name objects in the spreadsheet.
**Returns:**
[NameCollection](../../com.aspose.cells/namecollection)
### getOleSize() {#getOleSize--}
```
public Object getOleSize()
```
Gets displayed size when Workbook file is used as an Ole object.
**Remarks**
Null means no ole size setting.
**Returns:**
java.lang.Object
### getRangeByName(String rangeName) {#getRangeByName-java.lang.String-}
```
public Range getRangeByName(String rangeName)
```
Gets Range object by pre-defined name.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rangeName | java.lang.String | Name of range. |
**Returns:**
[Range](../../com.aspose.cells/range) - Range object.
Returns null if the named range does not exist.
### getRangeByName(String rangeName, int currentSheetIndex, boolean includeTable) {#getRangeByName-java.lang.String-int-boolean-}
```
public Range getRangeByName(String rangeName, int currentSheetIndex, boolean includeTable)
```
Gets [Range](../../com.aspose.cells/range) by pre-defined name or table's name
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rangeName | java.lang.String | Name of range or table's name. |
| currentSheetIndex | int | The sheet index. -1 represents global . |
| includeTable | boolean | Indicates whether checking all tables. |
**Returns:**
[Range](../../com.aspose.cells/range) -
### getRevisionLogs() {#getRevisionLogs--}
```
public RevisionLogCollection getRevisionLogs()
```
Represents revision logs.
**Returns:**
[RevisionLogCollection](../../com.aspose.cells/revisionlogcollection)
### getSensitivityLabels() {#getSensitivityLabels--}
```
public SensitivityLabelCollection getSensitivityLabels()
```
Represents all sensitivity labels.
**Returns:**
[SensitivityLabelCollection](../../com.aspose.cells/sensitivitylabelcollection)
### getSheetByCodeName(String codeName) {#getSheetByCodeName-java.lang.String-}
```
public Worksheet getSheetByCodeName(String codeName)
```
Gets the worksheet by the code name.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| codeName | java.lang.String | Worksheet code name. |
**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - The element with the specified code name.
### getTableStyles() {#getTableStyles--}
```
public TableStyleCollection getTableStyles()
```
Gets [getTableStyles()](../../com.aspose.cells/worksheetcollection\#getTableStyles--) object.
**Returns:**
[TableStyleCollection](../../com.aspose.cells/tablestylecollection)
### getThreadedCommentAuthors() {#getThreadedCommentAuthors--}
```
public ThreadedCommentAuthorCollection getThreadedCommentAuthors()
```
Gets the list of threaded comment authors.
**Returns:**
[ThreadedCommentAuthorCollection](../../com.aspose.cells/threadedcommentauthorcollection)
### getWebExtensionTaskPanes() {#getWebExtensionTaskPanes--}
```
public WebExtensionTaskPaneCollection getWebExtensionTaskPanes()
```
Gets the list of task panes.
**Returns:**
[WebExtensionTaskPaneCollection](../../com.aspose.cells/webextensiontaskpanecollection)
### getWebExtensions() {#getWebExtensions--}
```
public WebExtensionCollection getWebExtensions()
```
Gets the list of task panes.
**Returns:**
[WebExtensionCollection](../../com.aspose.cells/webextensioncollection)
### getXmlMaps() {#getXmlMaps--}
```
public XmlMapCollection getXmlMaps()
```
Gets the XML maps in the workbook.
**Returns:**
[XmlMapCollection](../../com.aspose.cells/xmlmapcollection)
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```
Determines the index of a specific item in the CollectionBase instance.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | Determines the index of a specific item in the CollectionBase instance. |
**Returns:**
int - The index of value if found in the list; otherwise, -1.
### insert(int index, int sheetType) {#insert-int-int-}
```
public Worksheet insert(int index, int sheetType)
```
Insert a worksheet.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The sheet index |
| sheetType | int | [SheetType](../../com.aspose.cells/sheettype). The sheet type. |
**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - Returns an inserted worksheet.
### insert(int index, int sheetType, String sheetName) {#insert-int-int-java.lang.String-}
```
public Worksheet insert(int index, int sheetType, String sheetName)
```
Insert a worksheet.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The sheet index |
| sheetType | int | [SheetType](../../com.aspose.cells/sheettype). The sheet type. |
| sheetName | java.lang.String | The sheet name. |
**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - Returns an inserted worksheet.
### isRefreshAllConnections() {#isRefreshAllConnections--}
```
public boolean isRefreshAllConnections()
```
Indicates whether refresh all connections on opening file in MS Excel.
**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```
Returns an enumerator that iterates through the CollectionBase instance.
**Returns:**
java.util.Iterator - An iterator for the CollectionBase instance.
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### refreshAll() {#refreshAll--}
```
public void refreshAll()
```
Refresh all pivot tables and charts with pivot source.
### refreshPivotTables() {#refreshPivotTables--}
```
public void refreshPivotTables()
```
Refreshes all the PivotTables in the Excel file.
### refreshPivotTables(PivotTableRefreshOption option) {#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-}
```
public boolean refreshPivotTables(PivotTableRefreshOption option)
```
Refreshes all the PivotTables in the Excel file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | The option for refreshing data source of the pivot tables. |
**Returns:**
boolean
### registerAddInFunction(int id, String functionName) {#registerAddInFunction-int-java.lang.String-}
```
public String registerAddInFunction(int id, String functionName)
```
Adds addin function into the workbook
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| id | int | ID of the data which contains addin functions, can be got by the first call of [registerAddInFunction(String,String,boolean)](../../com.aspose.cells/worksheetcollection\#registerAddInFunction-String-String-boolean-) for the same addin file. |
| functionName | java.lang.String | the addin function name |
**Returns:**
java.lang.String - URL of the addin file which contains addin functions
### registerAddInFunction(String addInFile, String functionName, boolean lib) {#registerAddInFunction-java.lang.String-java.lang.String-boolean-}
```
public int registerAddInFunction(String addInFile, String functionName, boolean lib)
```
Adds addin function into the workbook
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| addInFile | java.lang.String | the file contains the addin functions |
| functionName | java.lang.String | the addin function name |
| lib | boolean | whether the given addin file is in the directory or sub-directory of Workbook Add-In library. This flag takes effect and makes difference when given addInFile is of relative path: true denotes the path is relative to Add-In library and false denotes the path is relative to this Workbook. |
**Returns:**
int - ID of the data which contains given addin function
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```
Removes the element at a specified index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The index value of the element to remove. |
### removeAt(String name) {#removeAt-java.lang.String-}
```
public void removeAt(String name)
```
Removes the element at a specified name.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the element to remove. |
### setActiveSheetIndex(int value) {#setActiveSheetIndex-int-}
```
public void setActiveSheetIndex(int value)
```
Represents the index of active worksheet when the spreadsheet is opened.
**Remarks**
Sheet index is zero based.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setActiveSheetName(String value) {#setActiveSheetName-java.lang.String-}
```
public void setActiveSheetName(String value)
```
Represents the name of active worksheet when the spreadsheet is opened.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setOleSize(int startRow, int endRow, int startColumn, int endColumn) {#setOleSize-int-int-int-int-}
```
public void setOleSize(int startRow, int endRow, int startColumn, int endColumn)
```
Sets displayed size when Workbook file is used as an Ole object.
**Remarks**
This method is generally used to adjust display size in ppt file or doc file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | int | Start row index. |
| endRow | int | End row index. |
| startColumn | int | Start column index. |
| endColumn | int | End column index. |
### setOleSize(Object value) {#setOleSize-java.lang.Object-}
```
public void setOleSize(Object value)
```
Sets displayed size when Workbook file is used as an Ole object.
**Remarks**
Null means no ole size setting.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Object |  |
### setRefreshAllConnections(boolean value) {#setRefreshAllConnections-boolean-}
```
public void setRefreshAllConnections(boolean value)
```
Indicates whether refresh all connections on opening file in MS Excel.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setXmlMaps(XmlMapCollection value) {#setXmlMaps-com.aspose.cells.XmlMapCollection-}
```
public void setXmlMaps(XmlMapCollection value)
```
Sets the XML maps in the workbook.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [XmlMapCollection](../../com.aspose.cells/xmlmapcollection) |  |
### sortNames() {#sortNames--}
```
public void sortNames()
```
Sorts the defined names.
**Remarks**
If you create a large amount of named ranges in the Excel file, please call this method after all named ranges are created and before saving
### swapSheet(int sheetIndex1, int sheetIndex2) {#swapSheet-int-int-}
```
public void swapSheet(int sheetIndex1, int sheetIndex2)
```
Swaps the two sheets.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex1 | int | The first worksheet. |
| sheetIndex2 | int | The second worksheet. |
### toString() {#toString--}
```
public String toString()
```
**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```
### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |
