---
title: FindOptions
second_title: Aspose.Cells for Java API Reference
description: Represents find options.
type: docs
weight: 219
url: /java/com.aspose.cells/findoptions/
---

**Inheritance:**
java.lang.Object
```
public class FindOptions
```

Represents find options.

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
| [getConvertNumericData()](#getConvertNumericData--) | a value that indicates whether converting the searched string value to numeric data. |
| [getLookAtType()](#getLookAtType--) | Look at type. |
| [getLookInType()](#getLookInType--) | Look in type. |
| [getRange()](#getRange--) | Gets and sets the searched range. |
| [getRegexKey()](#getRegexKey--) | Indicates whether the searched key is regex. |
| [getSeachOrderByRows()](#getSeachOrderByRows--) | Indicates whether search order by rows or columns. |
| [getSearchBackward()](#getSearchBackward--) | Whether search backward for cells. |
| [getSearchNext()](#getSearchNext--) | Search order. |
| [getStyle()](#getStyle--) | The format to search for. |
| [getValueTypeSensitive()](#getValueTypeSensitive--) | Indicates whether searched cell value type should be same with the searched key. |
| [hashCode()](#hashCode--) |  |
| [isRangeSet()](#isRangeSet--) | Indicates whether the searched range is set. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCaseSensitive(boolean value)](#setCaseSensitive-boolean-) | For the description of this property, please see [getCaseSensitive()](../../com.aspose.cells/findoptions\#getCaseSensitive--) |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | For the description of this property, please see [getConvertNumericData()](../../com.aspose.cells/findoptions\#getConvertNumericData--) |
| [setLookAtType(int value)](#setLookAtType-int-) | For the description of this property, please see [getLookAtType()](../../com.aspose.cells/findoptions\#getLookAtType--) |
| [setLookInType(int value)](#setLookInType-int-) | For the description of this property, please see [getLookInType()](../../com.aspose.cells/findoptions\#getLookInType--) |
| [setRange(CellArea ca)](#setRange-com.aspose.cells.CellArea-) | Sets the searched range. |
| [setRegexKey(boolean value)](#setRegexKey-boolean-) | For the description of this property, please see [getRegexKey()](../../com.aspose.cells/findoptions\#getRegexKey--) |
| [setSeachOrderByRows(boolean value)](#setSeachOrderByRows-boolean-) | For the description of this property, please see [getSeachOrderByRows()](../../com.aspose.cells/findoptions\#getSeachOrderByRows--) |
| [setSearchBackward(boolean value)](#setSearchBackward-boolean-) | For the description of this property, please see [getSearchBackward()](../../com.aspose.cells/findoptions\#getSearchBackward--) |
| [setSearchNext(boolean value)](#setSearchNext-boolean-) | For the description of this property, please see [getSearchNext()](../../com.aspose.cells/findoptions\#getSearchNext--) |
| [setStyle(Style value)](#setStyle-com.aspose.cells.Style-) | For the description of this property, please see [getStyle()](../../com.aspose.cells/findoptions\#getStyle--) |
| [setValueTypeSensitive(boolean value)](#setValueTypeSensitive-boolean-) | For the description of this property, please see [getValueTypeSensitive()](../../com.aspose.cells/findoptions\#getValueTypeSensitive--) |
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


a value that indicates whether converting the searched string value to numeric data.

**Returns:**
boolean
### getLookAtType() {#getLookAtType--}
```
public int getLookAtType()
```


Look at type.

**Returns:**
int
### getLookInType() {#getLookInType--}
```
public int getLookInType()
```


Look in type.

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

**Returns:**
boolean
### getSeachOrderByRows() {#getSeachOrderByRows--}
```
public boolean getSeachOrderByRows()
```


Indicates whether search order by rows or columns.

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


Search order. True: search next. False: search previous. NOTE: This member is now obsolete. Instead, please use FindOptions.SearchBackward property. This property will be removed 12 months later since November 2018. Aspose apologizes for any inconvenience you may have experienced.

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


For the description of this property, please see [getCaseSensitive()](../../com.aspose.cells/findoptions\#getCaseSensitive--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


For the description of this property, please see [getConvertNumericData()](../../com.aspose.cells/findoptions\#getConvertNumericData--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setLookAtType(int value) {#setLookAtType-int-}
```
public void setLookAtType(int value)
```


For the description of this property, please see [getLookAtType()](../../com.aspose.cells/findoptions\#getLookAtType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setLookInType(int value) {#setLookInType-int-}
```
public void setLookInType(int value)
```


For the description of this property, please see [getLookInType()](../../com.aspose.cells/findoptions\#getLookInType--)

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


For the description of this property, please see [getRegexKey()](../../com.aspose.cells/findoptions\#getRegexKey--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSeachOrderByRows(boolean value) {#setSeachOrderByRows-boolean-}
```
public void setSeachOrderByRows(boolean value)
```


For the description of this property, please see [getSeachOrderByRows()](../../com.aspose.cells/findoptions\#getSeachOrderByRows--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSearchBackward(boolean value) {#setSearchBackward-boolean-}
```
public void setSearchBackward(boolean value)
```


For the description of this property, please see [getSearchBackward()](../../com.aspose.cells/findoptions\#getSearchBackward--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSearchNext(boolean value) {#setSearchNext-boolean-}
```
public void setSearchNext(boolean value)
```


For the description of this property, please see [getSearchNext()](../../com.aspose.cells/findoptions\#getSearchNext--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setStyle(Style value) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style value)
```


For the description of this property, please see [getStyle()](../../com.aspose.cells/findoptions\#getStyle--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setValueTypeSensitive(boolean value) {#setValueTypeSensitive-boolean-}
```
public void setValueTypeSensitive(boolean value)
```


For the description of this property, please see [getValueTypeSensitive()](../../com.aspose.cells/findoptions\#getValueTypeSensitive--)

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

