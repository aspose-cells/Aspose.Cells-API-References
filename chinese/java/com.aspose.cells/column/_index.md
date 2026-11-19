---
title: "Column"
second_title: "Aspose.Cells for Java API 参考"
description: "表示工作表中的单列。"
type: docs
url: /zh/java/com.aspose.cells/column/
---

**Inheritance:**
java.lang.Object
```
public class Column
```

表示工作表中的单列。

**Example**

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
## 方法

| 方法 | 描述 |
| --- | --- |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | 对整列应用格式。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getGroupLevel()](#getGroupLevel--) | 获取列的分组级别。 |
| [getIndex()](#getIndex--) | 获取此列的索引。 |
| [getStyle()](#getStyle--) | 获取此列的样式。 |
| [getWidth()](#getWidth--) | 获取列宽（以字符为单位）。 |
| [hasCustomStyle()](#hasCustomStyle--) | 指示此列是否具有自定义样式设置（不同于从工作簿继承的默认样式）。 |
| [hashCode()](#hashCode--) |  |
| [isCollapsed()](#isCollapsed--) | 列是否已折叠 |
| [isHidden()](#isHidden--) | 指示列是否隐藏。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCollapsed(boolean value)](#setCollapsed-boolean-) | 列是否已折叠 |
| [setGroupLevel(byte value)](#setGroupLevel-byte-) | 获取列的分组级别。 |
| [setHidden(boolean value)](#setHidden-boolean-) | 指示列是否隐藏。 |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | 设置此列的样式。 |
| [setWidth(double value)](#setWidth-double-) | 设置列宽（以字符为单位）。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


对整列应用格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | 将要应用的样式对象。 |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | 指示已应用格式属性的标志。 |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
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


获取列的分组级别。

**Returns:**
byte
### getIndex() {#getIndex--}
```
public int getIndex()
```


获取此列的索引。

**Returns:**
int
### getStyle() {#getStyle--}
```
public Style getStyle()
```


获取此列的样式。

**Remarks**

直接修改返回的样式对象对该列或该列中的任何单元格没有影响。必须调用 [applyStyle(Style,StyleFlag)](../../com.aspose.cells/column\#applyStyle-Style-StyleFlag-) 或 [setStyle(Style)](../../com.aspose.cells/column\#setStyle-Style-) 方法才能将更改应用于该列。

Column's style 是将在此列的单元格中继承的样式（那些没有自定义样式设置的单元格，例如尚未显式设置样式的现有单元格，或尚未实例化的单元格）

**Returns:**
[Style](../../com.aspose.cells/style)
### getWidth() {#getWidth--}
```
public double getWidth()
```


获取列宽（以字符为单位）。

**Remarks**

对于电子表格，列宽以普通样式字体中数字 0~9 的最大数字宽度对应的字符数来衡量。

**Returns:**
double
### hasCustomStyle() {#hasCustomStyle--}
```
public boolean hasCustomStyle()
```


指示此列是否具有自定义样式设置（不同于从工作簿继承的默认样式）。

**Returns:**
boolean
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


列是否已折叠

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


指示列是否隐藏。

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


列是否已折叠

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setGroupLevel(byte value) {#setGroupLevel-byte-}
```
public void setGroupLevel(byte value)
```


获取列的分组级别。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | byte |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


指示列是否隐藏。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


设置此列的样式。

**Remarks**

此方法仅将给定的样式设置为此列的默认样式，而不更改此列中现有单元格的样式设置。若要同时将现有单元格的样式设置更新为指定样式，请使用 [applyStyle(Style,StyleFlag)](../../com.aspose.cells/column\#applyStyle-Style-StyleFlag-)

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | 用于此列单元格的默认样式。 |

### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```


设置列宽（以字符为单位）。

**Remarks**

对于电子表格，列宽以普通样式字体中数字 0~9 的最大数字宽度对应的字符数来衡量。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

