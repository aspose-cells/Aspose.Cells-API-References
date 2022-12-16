---
title: Row
second_title: Aspose.Cells for Java API Reference
description: Represents a single row in a worksheet.
type: docs
url: /java/com.aspose.cells/row/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Row implements Iterable
```

Represents a single row in a worksheet.

```
//Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
         Style style = workbook.createStyle();
 
         //Setting the background color to Blue
         style.setBackgroundColor(Color.getBlue());
 
         //Setting the foreground color to Red
         style.setForegroundColor(Color.getRed());
 
         //setting Background Pattern
         style.setPattern(BackgroundType.DIAGONAL_STRIPE);
 
         //New Style Flag
         StyleFlag styleFlag = new StyleFlag();
 
         //Set All Styles
         styleFlag.setAll(true);
 
          //Get first row
         Row row = worksheet.getCells().getRows().get(0);
          //Apply Style to first row
         row.applyStyle(style, styleFlag);
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Methods

| Method | Description |
| --- | --- |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Applies formats for a whole row. |
| [copySettings(Row source, boolean checkStyle)](#copySettings-com.aspose.cells.Row-boolean-) | Copy settings of row, such as style, height, visibility, ...etc. |
| [equals(Row row)](#equals-com.aspose.cells.Row-) | Checks whether this object refers to the same row with another row object. |
| [equals(Object obj)](#equals-java.lang.Object-) | Checks whether this object refers to the same row with another. |
| [get(int column)](#get-int-) | Gets the cell. |
| [getCellByIndex(int index)](#getCellByIndex-int-) | Get the cell by specific index in the list. |
| [getCellOrNull(int column)](#getCellOrNull-int-) | Gets the cell or null in the specific index. |
| [getClass()](#getClass--) |  |
| [getFirstCell()](#getFirstCell--) | Gets the first cell object in the row. |
| [getFirstDataCell()](#getFirstDataCell--) | Gets the first non-blank cell in the row. |
| [getGroupLevel()](#getGroupLevel--) | Gets the group level of the row. |
| [getHeight()](#getHeight--) | Gets the row height in unit of Points. |
| [getIndex()](#getIndex--) | Gets the index of this row. |
| [getLastCell()](#getLastCell--) | Gets the last cell object in the row. |
| [getLastDataCell()](#getLastDataCell--) | Gets the last non-blank cell in the row. |
| [getStyle()](#getStyle--) | Represents the style of this row. |
| [hashCode()](#hashCode--) |  |
| [isBlank()](#isBlank--) | Indicates whether the row contains any data |
| [isCollapsed()](#isCollapsed--) | whether the row is collapsed |
| [isHeightMatched()](#isHeightMatched--) | Indicates that row height and default font height matches. |
| [isHidden()](#isHidden--) | Indicates whether the row is hidden. |
| [iterator()](#iterator--) | Gets the cells enumerator |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCollapsed(boolean value)](#setCollapsed-boolean-) | whether the row is collapsed |
| [setHeight(double value)](#setHeight-double-) | Sets the row height in unit of Points. |
| [setHeightMatched(boolean value)](#setHeightMatched-boolean-) | Indicates that row height and default font height matches. |
| [setHidden(boolean value)](#setHidden-boolean-) | Indicates whether the row is hidden. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


Applies formats for a whole row.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | The style object which will be applied. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Flags which indicates applied formatting properties. |

### copySettings(Row source, boolean checkStyle) {#copySettings-com.aspose.cells.Row-boolean-}
```
public void copySettings(Row source, boolean checkStyle)
```


Copy settings of row, such as style, height, visibility, ...etc.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | [Row](../../com.aspose.cells/row) | the source row whose settings will be copied to this one |
| checkStyle | boolean | whether check and gather style. Only takes effect and be needed when two row objects belong to different workbook and the styles of two workbooks are different. |

### equals(Row row) {#equals-com.aspose.cells.Row-}
```
public boolean equals(Row row)
```


Checks whether this object refers to the same row with another row object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | [Row](../../com.aspose.cells/row) | another row object |

**Returns:**
boolean - true if two row objects refers to the same row.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Checks whether this object refers to the same row with another.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | another object |

**Returns:**
boolean - true if two objects refers to the same row.
### get(int column) {#get-int-}
```
public Cell get(int column)
```


Gets the cell.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | int | The column index |

**Returns:**
[Cell](../../com.aspose.cells/cell) - 
### getCellByIndex(int index) {#getCellByIndex-int-}
```
public Cell getCellByIndex(int index)
```


Get the cell by specific index in the list. NOTE: This member is now obsolete. Instead, please use Row.GetEnumerator() method to iterate all cells in this row. This property will be removed 12 months later since February 2015. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The position. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - The Cell object.
### getCellOrNull(int column) {#getCellOrNull-int-}
```
public Cell getCellOrNull(int column)
```


Gets the cell or null in the specific index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | int | The column index |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Returns the cell object if the cell exists. Or returns null if the cell object does not exist.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFirstCell() {#getFirstCell--}
```
public Cell getFirstCell()
```


Gets the first cell object in the row.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getFirstDataCell() {#getFirstDataCell--}
```
public Cell getFirstDataCell()
```


Gets the first non-blank cell in the row.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getGroupLevel() {#getGroupLevel--}
```
public byte getGroupLevel()
```


Gets the group level of the row.

**Returns:**
byte
### getHeight() {#getHeight--}
```
public double getHeight()
```


Gets the row height in unit of Points.

**Returns:**
double
### getIndex() {#getIndex--}
```
public int getIndex()
```


Gets the index of this row.

**Returns:**
int
### getLastCell() {#getLastCell--}
```
public Cell getLastCell()
```


Gets the last cell object in the row.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getLastDataCell() {#getLastDataCell--}
```
public Cell getLastDataCell()
```


Gets the last non-blank cell in the row.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Represents the style of this row. You have to call Row.ApplyStyle() method to save your changing with the row style, otherwise it will not effect.

**Returns:**
[Style](../../com.aspose.cells/style)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBlank() {#isBlank--}
```
public boolean isBlank()
```


Indicates whether the row contains any data

**Returns:**
boolean
### isCollapsed() {#isCollapsed--}
```
public boolean isCollapsed()
```


whether the row is collapsed

**Returns:**
boolean
### isHeightMatched() {#isHeightMatched--}
```
public boolean isHeightMatched()
```


Indicates that row height and default font height matches.

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Indicates whether the row is hidden.

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


Gets the cells enumerator

```
Workbook workbook = new Workbook("template.xlsx");
         	Cells cells = workbook.getWorksheets().get(0).getCells();
 
         	Iterator en = cells.getRows().get(1).iterator();
         	while (en.hasNext())
         	{
         	    Cell cell = (Cell)en.next();
         	    System.out.println(cell.getName() + ": " + cell.getValue());
         	}
```

**Returns:**
java.util.Iterator - The cells enumerator
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setCollapsed(boolean value) {#setCollapsed-boolean-}
```
public void setCollapsed(boolean value)
```


whether the row is collapsed

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


Sets the row height in unit of Points.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setHeightMatched(boolean value) {#setHeightMatched-boolean-}
```
public void setHeightMatched(boolean value)
```


Indicates that row height and default font height matches.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Indicates whether the row is hidden.

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

