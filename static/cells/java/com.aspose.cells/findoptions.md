##FindOptions
Represents find options.
**Inheritance:**
java.lang.Object
```
public class FindOptions
```
Represents find options.
**Example**
```
//Instantiate the workbook object
Workbook workbook = new Workbook("book1.xls");
//Get Cells collection
Cells cells = workbook.getWorksheets().get(0).getCells();
//Instantiate FindOptions Object
FindOptions findOptions = new FindOptions();
//Create a Cells Area
CellArea ca = new CellArea();
ca.StartRow = 8;
ca.StartColumn = 2;
ca.EndRow = 17;
ca.EndColumn = 13;
//Set cells area for find options
findOptions.setRange(ca);
//Set searching properties
findOptions.setSearchBackward(false);
findOptions.setSeachOrderByRows(true);
findOptions.setLookInType(LookInType.VALUES);
//Find the cell with 0 value
Cell cell = cells.find(0, null, findOptions);
```
## Constructors
| Constructor | Description |
| --- | --- |
| [FindOptions()](#FindOptions--) |  |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCaseSensitive()](#getCaseSensitive--) | Indicates if the searched string is case sensitive. |
| [getClass()](#getClass--) |  |
| [getConvertNumericData()](#getConvertNumericData--) | Gets a value that indicates whether converting the searched string value to numeric data. |
| [getLookAtType()](#getLookAtType--) | Look at type. |
| [getLookInType()](#getLookInType--) | Look in type. |
| [getRange()](#getRange--) | Gets and sets the searched range. |
| [getRegexKey()](#getRegexKey--) | Indicates whether the searched key is regex. |
| [getSeachOrderByRows()](#getSeachOrderByRows--) | Indicates whether search order by rows or columns. |
| [getSearchBackward()](#getSearchBackward--) | Whether search backward for cells. |
| [getSearchNext()](#getSearchNext--) | Search order. |
| [getSearchOrderByRows()](#getSearchOrderByRows--) | Indicates whether search order by rows or columns. |
| [getStyle()](#getStyle--) | The format to search for. |
| [getValueTypeSensitive()](#getValueTypeSensitive--) | Indicates whether searched cell value type should be same with the searched key. |
| [hashCode()](#hashCode--) |  |
| [isRangeSet()](#isRangeSet--) | Indicates whether the searched range is set. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCaseSensitive(boolean value)](#setCaseSensitive-boolean-) | Indicates if the searched string is case sensitive. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | Sets a value that indicates whether converting the searched string value to numeric data. |
| [setLookAtType(int value)](#setLookAtType-int-) | Look at type. |
| [setLookInType(int value)](#setLookInType-int-) | Look in type. |
| [setRange(CellArea ca)](#setRange-com.aspose.cells.CellArea-) | Sets the searched range. |
| [setRegexKey(boolean value)](#setRegexKey-boolean-) | Indicates whether the searched key is regex. |
| [setSeachOrderByRows(boolean value)](#setSeachOrderByRows-boolean-) | Indicates whether search order by rows or columns. |
| [setSearchBackward(boolean value)](#setSearchBackward-boolean-) | Whether search backward for cells. |
| [setSearchNext(boolean value)](#setSearchNext-boolean-) | Search order. |
| [setSearchOrderByRows(boolean value)](#setSearchOrderByRows-boolean-) | Indicates whether search order by rows or columns. |
| [setStyle(Style value)](#setStyle-com.aspose.cells.Style-) | The format to search for. |
| [setValueTypeSensitive(boolean value)](#setValueTypeSensitive-boolean-) | Indicates whether searched cell value type should be same with the searched key. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### FindOptions() {#FindOptions--}
```
public FindOptions()
```
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
### getCaseSensitive() {#getCaseSensitive--}
```
public boolean getCaseSensitive()
```
Indicates if the searched string is case sensitive.
**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```
Gets a value that indicates whether converting the searched string value to numeric data.
**Returns:**
boolean
### getLookAtType() {#getLookAtType--}
```
public int getLookAtType()
```
Look at type.
See [LookAtType](../../com.aspose.cells/lookattype).
**Remarks**
When [getRegexKey()](../../com.aspose.cells/findoptions\#getRegexKey--) is true and user has specified the exact rule for the regex, for performance consideration this property should be set as [LookAtType.ENTIRE\_CONTENT](../../com.aspose.cells/lookattype\#ENTIRE-CONTENT). Otherwise we will refactor the search key to ensure it can be matched according to the specific type. For example, when the type is [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\#CONTAINS)(this is the default value for this property), we will add wildcards at the beginning and end of the search key automatically. In this case, the regular expressions will become more complex and the performance will also decrease.
**Returns:**
int
### getLookInType() {#getLookInType--}
```
public int getLookInType()
```
Look in type.
See [LookInType](../../com.aspose.cells/lookintype).
**Returns:**
int
### getRange() {#getRange--}
```
public CellArea getRange()
```
Gets and sets the searched range.
**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - Returns the searched range.
### getRegexKey() {#getRegexKey--}
```
public boolean getRegexKey()
```
Indicates whether the searched key is regex. If true the searched key will be taken as regex and parsed. Otherwise the key will be parsed according to the rules in ms excel.
**Remarks**
Even though the search key has been specified as regex, it may be refactored according to specified [LookAtType](../../com.aspose.cells/lookattype). For example, when the type is [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\#CONTAINS)(this is the default value for this options), wildcards will be added at the beginning and end of the search key automatically to ensure the match will be checked as "contains". In this case, the regular expressions will become more complex and the performance will also decrease. So, for performance consideration, if user has specified the exact rule for the regex, then there is no need to use [LookAtType](../../com.aspose.cells/lookattype) as additional constraint and user may set it as [LookAtType.ENTIRE\_CONTENT](../../com.aspose.cells/lookattype\#ENTIRE-CONTENT) to get better performance.
**Returns:**
boolean
### getSeachOrderByRows() {#getSeachOrderByRows--}
```
public boolean getSeachOrderByRows()
```
Indicates whether search order by rows or columns.
**Remarks**
NOTE: This member is now obsolete. Instead, please use FindOptions.SearchOrderByRows property. This property will be removed 12 months later since November 2018. Aspose apologizes for any inconvenience you may have experienced.
**Returns:**
boolean
### getSearchBackward() {#getSearchBackward--}
```
public boolean getSearchBackward()
```
Whether search backward for cells.
**Returns:**
boolean
### getSearchNext() {#getSearchNext--}
```
public boolean getSearchNext()
```
Search order. True: search next. False: search previous.
**Remarks**
NOTE: This member is now obsolete. Instead, please use FindOptions.SearchBackward property. This property will be removed 12 months later since November 2018. Aspose apologizes for any inconvenience you may have experienced.
**Returns:**
boolean
### getSearchOrderByRows() {#getSearchOrderByRows--}
```
public boolean getSearchOrderByRows()
```
Indicates whether search order by rows or columns.
**Returns:**
boolean
### getStyle() {#getStyle--}
```
public Style getStyle()
```
The format to search for.
**Returns:**
[Style](../../com.aspose.cells/style)
### getValueTypeSensitive() {#getValueTypeSensitive--}
```
public boolean getValueTypeSensitive()
```
Indicates whether searched cell value type should be same with the searched key.
**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isRangeSet() {#isRangeSet--}
```
public boolean isRangeSet()
```
Indicates whether the searched range is set.
**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### setCaseSensitive(boolean value) {#setCaseSensitive-boolean-}
```
public void setCaseSensitive(boolean value)
```
Indicates if the searched string is case sensitive.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```
Sets a value that indicates whether converting the searched string value to numeric data.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setLookAtType(int value) {#setLookAtType-int-}
```
public void setLookAtType(int value)
```
Look at type.
See [LookAtType](../../com.aspose.cells/lookattype).
**Remarks**
When [getRegexKey()](../../com.aspose.cells/findoptions\#getRegexKey--) is true and user has specified the exact rule for the regex, for performance consideration this property should be set as [LookAtType.ENTIRE\_CONTENT](../../com.aspose.cells/lookattype\#ENTIRE-CONTENT). Otherwise we will refactor the search key to ensure it can be matched according to the specific type. For example, when the type is [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\#CONTAINS)(this is the default value for this property), we will add wildcards at the beginning and end of the search key automatically. In this case, the regular expressions will become more complex and the performance will also decrease.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setLookInType(int value) {#setLookInType-int-}
```
public void setLookInType(int value)
```
Look in type.
See [LookInType](../../com.aspose.cells/lookintype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setRange(CellArea ca) {#setRange-com.aspose.cells.CellArea-}
```
public void setRange(CellArea ca)
```
Sets the searched range.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | the searched range. |
### setRegexKey(boolean value) {#setRegexKey-boolean-}
```
public void setRegexKey(boolean value)
```
Indicates whether the searched key is regex. If true the searched key will be taken as regex and parsed. Otherwise the key will be parsed according to the rules in ms excel.
**Remarks**
Even though the search key has been specified as regex, it may be refactored according to specified [LookAtType](../../com.aspose.cells/lookattype). For example, when the type is [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\#CONTAINS)(this is the default value for this options), wildcards will be added at the beginning and end of the search key automatically to ensure the match will be checked as "contains". In this case, the regular expressions will become more complex and the performance will also decrease. So, for performance consideration, if user has specified the exact rule for the regex, then there is no need to use [LookAtType](../../com.aspose.cells/lookattype) as additional constraint and user may set it as [LookAtType.ENTIRE\_CONTENT](../../com.aspose.cells/lookattype\#ENTIRE-CONTENT) to get better performance.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setSeachOrderByRows(boolean value) {#setSeachOrderByRows-boolean-}
```
public void setSeachOrderByRows(boolean value)
```
Indicates whether search order by rows or columns.
**Remarks**
NOTE: This member is now obsolete. Instead, please use FindOptions.SearchOrderByRows property. This property will be removed 12 months later since November 2018. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setSearchBackward(boolean value) {#setSearchBackward-boolean-}
```
public void setSearchBackward(boolean value)
```
Whether search backward for cells.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setSearchNext(boolean value) {#setSearchNext-boolean-}
```
public void setSearchNext(boolean value)
```
Search order. True: search next. False: search previous.
**Remarks**
NOTE: This member is now obsolete. Instead, please use FindOptions.SearchBackward property. This property will be removed 12 months later since November 2018. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setSearchOrderByRows(boolean value) {#setSearchOrderByRows-boolean-}
```
public void setSearchOrderByRows(boolean value)
```
Indicates whether search order by rows or columns.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setStyle(Style value) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style value)
```
The format to search for.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |
### setValueTypeSensitive(boolean value) {#setValueTypeSensitive-boolean-}
```
public void setValueTypeSensitive(boolean value)
```
Indicates whether searched cell value type should be same with the searched key.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
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
