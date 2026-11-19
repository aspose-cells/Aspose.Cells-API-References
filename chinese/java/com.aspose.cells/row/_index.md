---
title: "行"
second_title: "Aspose.Cells for Java API 参考"
description: "表示工作表中的单行。"
type: docs
url: /zh/java/com.aspose.cells/row/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Row implements Iterable
```

表示工作表中的单行。

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
 
          //Get first row
         Row row = worksheet.getCells().getRows().get(0);
          //Apply Style to first row
         row.applyStyle(style, styleFlag);
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | 对整行应用格式。 |
| [copySettings(Row source, boolean checkStyle)](#copySettings-com.aspose.cells.Row-boolean-) | 复制行的设置，例如样式、高度、可见性，...等。 |
| [equals(Row row)](#equals-com.aspose.cells.Row-) | 检查此对象是否与另一个行对象指向相同的行。 |
| [equals(Object obj)](#equals-java.lang.Object-) | 检查此对象是否与另一个对象指向相同的行。 |
| [get(int column)](#get-int-) | 获取单元格。 |
| [getCellByIndex(int index)](#getCellByIndex-int-) | 通过此行单元格集合中的特定索引获取单元格。 |
| [getCellOrNull(int column)](#getCellOrNull-int-) | 获取特定索引处的单元格，若不存在则返回 null。 |
| [getClass()](#getClass--) |  |
| [getFirstCell()](#getFirstCell--) | 获取行中的第一个单元格对象。 |
| [getFirstDataCell()](#getFirstDataCell--) | 获取行中的第一个非空单元格。 |
| [getGroupLevel()](#getGroupLevel--) | 获取行的分组级别。 |
| [getHeight()](#getHeight--) | 获取以点为单位的行高。 |
| [getIndex()](#getIndex--) | 获取此行的索引。 |
| [getLastCell()](#getLastCell--) | 获取行中的最后一个单元格对象。 |
| [getLastDataCell()](#getLastDataCell--) | 获取行中的最后一个非空单元格。 |
| [getStyle()](#getStyle--) | 获取此行的样式。 |
| [hasCustomStyle()](#hasCustomStyle--) | 指示此行是否具有自定义样式设置（不同于从工作簿继承的默认样式）。 |
| [hashCode()](#hashCode--) |  |
| [isBlank()](#isBlank--) | 指示该行是否包含任何数据 |
| [isCollapsed()](#isCollapsed--) | 行是否已折叠 |
| [isHeightMatched()](#isHeightMatched--) | 指示行高是否匹配工作簿当前的默认字体设置。 |
| [isHidden()](#isHidden--) | 指示该行是否隐藏。 |
| [iterator()](#iterator--) | 获取单元格枚举器 |
| [iterator(boolean reversed, boolean sync)](#iterator-boolean-boolean-) | 获取一个遍历此行单元格的枚举器。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCollapsed(boolean value)](#setCollapsed-boolean-) | 行是否已折叠 |
| [setGroupLevel(byte value)](#setGroupLevel-byte-) | 获取行的分组级别。 |
| [setHeight(double value)](#setHeight-double-) | 设置以点为单位的行高。 |
| [setHeightMatched(boolean value)](#setHeightMatched-boolean-) | 指示行高是否匹配工作簿当前的默认字体设置。 |
| [setHidden(boolean value)](#setHidden-boolean-) | 指示该行是否隐藏。 |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | 设置此行的样式。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


对整行应用格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | 将要应用的样式对象。 |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | 指示已应用格式属性的标志。 |

### copySettings(Row source, boolean checkStyle) {#copySettings-com.aspose.cells.Row-boolean-}
```
public void copySettings(Row source, boolean checkStyle)
```


复制行的设置，例如样式、高度、可见性，...等。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| source | [Row](../../com.aspose.cells/row) | 源行，其设置将被复制到此行 |
| checkStyle | boolean | 是否检查并收集样式。仅在两个行对象属于不同工作簿且两个工作簿的样式不同的情况下才生效并且需要。 |

### equals(Row row) {#equals-com.aspose.cells.Row-}
```
public boolean equals(Row row)
```


检查此对象是否与另一个行对象指向相同的行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| row | [Row](../../com.aspose.cells/row) | 另一个行对象 |

**Returns:**
布尔型 - 如果两个行对象引用同一行则为 true。
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


检查此对象是否与另一个对象指向相同的行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | java.lang.Object | 另一个对象 |

**Returns:**
布尔型 - 如果两个对象引用同一行则为 true。
### get(int column) {#get-int-}
```
public Cell get(int column)
```


获取单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | int | 列索引 |

**Returns:**
[Cell](../../com.aspose.cells/cell) - 
### getCellByIndex(int index) {#getCellByIndex-int-}
```
public Cell getCellByIndex(int index)
```


通过此行单元格集合中的特定索引获取单元格。

**Remarks**

要在不修改的情况下顺序遍历所有单元格，使用 [iterator()](../../com.aspose.cells/row\#iterator--) 的性能优于逐个获取单元格的此方法。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 此行单元格集合中单元格的索引（位置）。 |

**Returns:**
[Cell](../../com.aspose.cells/cell) - The Cell object at given position.
### getCellOrNull(int column) {#getCellOrNull-int-}
```
public Cell getCellOrNull(int column)
```


获取特定索引处的单元格，若不存在则返回 null。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | int | 列索引 |

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


获取行中的第一个单元格对象。

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getFirstDataCell() {#getFirstDataCell--}
```
public Cell getFirstDataCell()
```


获取行中的第一个非空单元格。

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getGroupLevel() {#getGroupLevel--}
```
public byte getGroupLevel()
```


获取行的分组级别。

**Returns:**
byte
### getHeight() {#getHeight--}
```
public double getHeight()
```


获取以点为单位的行高。

**Returns:**
double
### getIndex() {#getIndex--}
```
public int getIndex()
```


获取此行的索引。

**Returns:**
int
### getLastCell() {#getLastCell--}
```
public Cell getLastCell()
```


获取行中的最后一个单元格对象。

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getLastDataCell() {#getLastDataCell--}
```
public Cell getLastDataCell()
```


获取行中的最后一个非空单元格。

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getStyle() {#getStyle--}
```
public Style getStyle()
```


获取此行的样式。

**Remarks**

直接修改返回的样式对象对该行或该行中的任何单元格没有影响。必须调用 [applyStyle(Style,StyleFlag)](../../com.aspose.cells/row\#applyStyle-Style-StyleFlag-) 或 [setStyle(Style)](../../com.aspose.cells/row\#setStyle-Style-) 方法才能将更改应用到此行。

行的样式是将被该行单元格继承的样式（那些没有自定义样式设置的单元格，例如尚未显式设置样式的已有单元格，或尚未实例化的单元格）。

**Returns:**
[Style](../../com.aspose.cells/style)
### hasCustomStyle() {#hasCustomStyle--}
```
public boolean hasCustomStyle()
```


指示此行是否具有自定义样式设置（不同于从工作簿继承的默认样式）。

**Returns:**
boolean
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


指示该行是否包含任何数据

**Returns:**
boolean
### isCollapsed() {#isCollapsed--}
```
public boolean isCollapsed()
```


行是否已折叠

**Returns:**
boolean
### isHeightMatched() {#isHeightMatched--}
```
public boolean isHeightMatched()
```


指示行高是否匹配工作簿当前的默认字体设置。该属性为 true 时也表示行高为 "automatic"，即未由用户设置自定义高度值。

**Remarks**

当此属性为 true 时，如果该行的内容发生变化，通常需要重新计算行高（例如通过 [Worksheet.autoFitRows()](../../com.aspose.cells/worksheet\#autoFitRows--)），以获得在 Microsoft Excel 中打开工作簿时显示的相同结果。

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


指示该行是否隐藏。

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


获取单元格枚举器

**Example**

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
java.util.Iterator - 将遍历此行中所有现有单元格的枚举器。
### iterator(boolean reversed, boolean sync) {#iterator-boolean-boolean-}
```
public Iterator iterator(boolean reversed, boolean sync)
```


获取一个遍历此行单元格的枚举器。

**Remarks**

如果在使用枚举器遍历期间行可能被修改（例如导致新 Cell 实例化或现有 Cell 被移除的操作），应使用同步枚举器而非普通枚举器，以便遍历能够从上一次 MoveNext() 已遍历的位置的下一个位置继续。虽然同步枚举器的优势在于不会跳过或重复遍历元素，但其缺点是相较于普通枚举器性能会略有下降。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 反向 | boolean | 是否以相反顺序枚举单元格 |
| 同步 | boolean | 返回的枚举器是否应检查此行单元格的修改并保持同步。 |

**Returns:**
java.util.Iterator - 将遍历此行中所有现有单元格的枚举器。
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


行是否已折叠

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setGroupLevel(byte value) {#setGroupLevel-byte-}
```
public void setGroupLevel(byte value)
```


获取行的分组级别。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | byte |  |

### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


设置以点为单位的行高。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setHeightMatched(boolean value) {#setHeightMatched-boolean-}
```
public void setHeightMatched(boolean value)
```


指示行高是否匹配工作簿当前的默认字体设置。该属性为 true 时也表示行高为 "automatic"，即未由用户设置自定义高度值。

**Remarks**

当此属性为 true 时，如果该行的内容发生变化，通常需要重新计算行高（例如通过 [Worksheet.autoFitRows()](../../com.aspose.cells/worksheet\#autoFitRows--)），以获得在 Microsoft Excel 中打开工作簿时显示的相同结果。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


指示该行是否隐藏。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


设置此行的样式。

**Remarks**

此方法仅将给定的样式设为该行的默认样式，而不更改该行中已有单元格的样式设置。若要同时将已有单元格的样式更新为指定样式，请使用 [applyStyle(Style,StyleFlag)](../../com.aspose.cells/row\#applyStyle-Style-StyleFlag-)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | 用于该行单元格的默认样式。 |

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

