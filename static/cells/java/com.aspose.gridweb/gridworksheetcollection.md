##GridWorksheetCollection
Encapsulates a collection of  objects.
**Inheritance:**
java.lang.Object, [com.aspose.gridweb.CollectionBase](../../com.aspose.gridweb/collectionbase)
```
public class GridWorksheetCollection extends CollectionBase
```
Encapsulates a collection of [GridWorksheet](../../com.aspose.gridweb/gridworksheet) objects.
## Methods
| Method | Description |
| --- | --- |
| [add()](#add--) | Adds a worksheet to the collection. |
| [add(Object o)](#add-java.lang.Object-) | Adds an item to the CollectionBase instance. |
| [add(String sheetName)](#add-java.lang.String-) | Adds a worksheet to the collection. |
| [addCopy(int sheetIndex)](#addCopy-int-) | Adds a worksheet to the collection and copies data from an existed worksheet. |
| [addCopy(String sheetName)](#addCopy-java.lang.String-) | Adds a worksheet to the collection and copies data from an existed worksheet. |
| [calculateFormula()](#calculateFormula--) | Calculates the result of formulas. |
| [clear()](#clear--) | Clear all worksheets. |
| [contains(Object o)](#contains-java.lang.Object-) | Return whether instance contains this object |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gets the [GridWorksheet](../../com.aspose.gridweb/gridworksheet) element at the specified index. |
| [get(String sheetName)](#get-java.lang.String-) | Gets the [GridWorksheet](../../com.aspose.gridweb/gridworksheet) element with the specified name. |
| [getActiveSheetIndex()](#getActiveSheetIndex--) | Represents the index of active worksheet when the spreadsheet is opened. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Gets the size of enumerator |
| [getDefaultFontName()](#getDefaultFontName--) | Gets the control's default font name. |
| [getDefaultFontSize()](#getDefaultFontSize--) | ????????? |
| [getNames()](#getNames--) | Gets the collection of all the Name objects in the spreadsheet. |
| [getNumberDecimalSeparator()](#getNumberDecimalSeparator--) | Gets the decimal separator for formatting/parsing numeric values. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determines the index of a specific item in the CollectionBase instance. |
| [insert(int index, String sheetName)](#insert-int-java.lang.String-) | Insert a worksheet. |
| [iterator()](#iterator--) | Gets the rows enumerator |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Removes the element at a specified index. |
| [removeAt(String name)](#removeAt-java.lang.String-) | Removes the element at a specified name. |
| [setActiveSheetIndex(int value)](#setActiveSheetIndex-int-) | Represents the index of active worksheet when the spreadsheet is opened. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Sets the control's default font name. |
| [setDefaultFontSize(FontUnit value)](#setDefaultFontSize-com.aspose.gridweb.FontUnit-) | ????????? |
| [setNumberDecimalSeparator(char value)](#setNumberDecimalSeparator-char-) | Sets the decimal separator for formatting/parsing numeric values. |
| [setVisible(String sheetName, boolean isVisible)](#setVisible-java.lang.String-boolean-) | Sets the visible for the sheet . |
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
int - [GridWorksheet](../../com.aspose.gridweb/gridworksheet) object index.
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
public GridWorksheet add(String sheetName)
```
Adds a worksheet to the collection.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | java.lang.String | Worksheet name |
**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet) - [GridWorksheet](../../com.aspose.gridweb/gridworksheet) object.
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
int - [GridWorksheet](../../com.aspose.gridweb/gridworksheet) object index.
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
int - [GridWorksheet](../../com.aspose.gridweb/gridworksheet) object index.
### calculateFormula() {#calculateFormula--}
```
public void calculateFormula()
```
Calculates the result of formulas.
### clear() {#clear--}
```
public void clear()
```
Clear all worksheets.
**Remarks**
A workbook must contains a worksheet.
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
public GridWorksheet get(int index)
```
Gets the [GridWorksheet](../../com.aspose.gridweb/gridworksheet) element at the specified index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero based index of the element. |
**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet) - The element at the specified index.
### get(String sheetName) {#get-java.lang.String-}
```
public GridWorksheet get(String sheetName)
```
Gets the [GridWorksheet](../../com.aspose.gridweb/gridworksheet) element with the specified name.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | java.lang.String | The name of the worksheet. |
**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet) - The GridWorksheet with the name.
### getActiveSheetIndex() {#getActiveSheetIndex--}
```
public int getActiveSheetIndex()
```
Represents the index of active worksheet when the spreadsheet is opened.
**Remarks**
Sheet index is zero based.
**Returns:**
int
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
Gets the size of enumerator
**Returns:**
int
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```
Gets the control's default font name.
**Example**
```
GridWeb GridWeb1=new GridWeb();
GridWeb1.setDefaultFontName("Arial");
```
**Returns:**
java.lang.String
### getDefaultFontSize() {#getDefaultFontSize--}
```
public FontUnit getDefaultFontSize()
```
?????????
**Returns:**
[FontUnit](../../com.aspose.gridweb/fontunit)
### getNames() {#getNames--}
```
public GridNameCollection getNames()
```
Gets the collection of all the Name objects in the spreadsheet.
**Returns:**
[GridNameCollection](../../com.aspose.gridweb/gridnamecollection)
### getNumberDecimalSeparator() {#getNumberDecimalSeparator--}
```
public char getNumberDecimalSeparator()
```
Gets the decimal separator for formatting/parsing numeric values. Default is the decimal separator of current Region.
**Returns:**
char
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
### insert(int index, String sheetName) {#insert-int-java.lang.String-}
```
public GridWorksheet insert(int index, String sheetName)
```
Insert a worksheet.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The sheet index |
| sheetName | java.lang.String |  |
**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet)
### iterator() {#iterator--}
```
public Iterator iterator()
```
Gets the rows enumerator
**Returns:**
java.util.Iterator - The rows enumerator
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
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
### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```
Sets the control's default font name.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setDefaultFontSize(FontUnit value) {#setDefaultFontSize-com.aspose.gridweb.FontUnit-}
```
public void setDefaultFontSize(FontUnit value)
```
?????????
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FontUnit](../../com.aspose.gridweb/fontunit) |  |
### setNumberDecimalSeparator(char value) {#setNumberDecimalSeparator-char-}
```
public void setNumberDecimalSeparator(char value)
```
Sets the decimal separator for formatting/parsing numeric values. Default is the decimal separator of current Region.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | char |  |
### setVisible(String sheetName, boolean isVisible) {#setVisible-java.lang.String-boolean-}
```
public void setVisible(String sheetName, boolean isVisible)
```
Sets the visible for the sheet .
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | java.lang.String | Name of source worksheet. |
| isVisible | boolean | Whether the worksheet is visible |
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
