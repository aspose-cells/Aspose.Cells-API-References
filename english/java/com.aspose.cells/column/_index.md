---
title: Column
second_title: Aspose.Cells for Java API Reference
description: Represents a single column in a worksheet.
type: docs
url: /java/com.aspose.cells/column/
---

**Inheritance:**
java.lang.Object
```
public class Column
```

Represents a single column in a worksheet.

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
 
         //Get first Column
         Column column = worksheet.getCells().getColumns().get(0);
 
         //Apply Style to first Column
         column.applyStyle(style, styleFlag);
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Methods

| Method | Description |
| --- | --- |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Applies formats for a whole column. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getGroupLevel()](#getGroupLevel--) | Gets the group level of the column. |
| [getIndex()](#getIndex--) | Gets the index of this column. |
| [getStyle()](#getStyle--) | Gets the style of this column. |
| [getWidth()](#getWidth--) | Gets the column width in unit of characters. |
| [hashCode()](#hashCode--) |  |
| [isCollapsed()](#isCollapsed--) | whether the column is collapsed |
| [isHidden()](#isHidden--) | Indicates whether the column is hidden. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCollapsed(boolean value)](#setCollapsed-boolean-) | whether the column is collapsed |
| [setHidden(boolean value)](#setHidden-boolean-) | Indicates whether the column is hidden. |
| [setWidth(double value)](#setWidth-double-) | Sets the column width in unit of characters. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


Applies formats for a whole column.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | The style object which will be applied. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Flags which indicates applied formatting properties. |

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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getGroupLevel() {#getGroupLevel--}
```
public byte getGroupLevel()
```


Gets the group level of the column.

**Returns:**
byte
### getIndex() {#getIndex--}
```
public int getIndex()
```


Gets the index of this column.

**Returns:**
int
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Gets the style of this column. You have to call Column.ApplyStyle() method to save your changing with the row style, otherwise it will not effect.

**Returns:**
[Style](../../com.aspose.cells/style)
### getWidth() {#getWidth--}
```
public double getWidth()
```


Gets the column width in unit of characters.

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCollapsed() {#isCollapsed--}
```
public boolean isCollapsed()
```


whether the column is collapsed

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Indicates whether the column is hidden.

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




### setCollapsed(boolean value) {#setCollapsed-boolean-}
```
public void setCollapsed(boolean value)
```


whether the column is collapsed

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Indicates whether the column is hidden.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```


Sets the column width in unit of characters.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

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

