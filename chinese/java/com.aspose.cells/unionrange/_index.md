---
title: "UnionRange"
second_title: "Aspose.Cells for Java API 参考"
description: "表示联合范围。"
type: docs
url: /zh/java/com.aspose.cells/unionrange/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class UnionRange implements Iterable
```

表示联合范围。
## 方法

| 方法 | 描述 |
| --- | --- |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | 对整个范围应用格式。 |
| [copy(UnionRange range, PasteOptions options)](#copy-com.aspose.cells.UnionRange-com.aspose.cells.PasteOptions-) | 使用粘贴特殊选项复制范围。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellCount()](#getCellCount--) | 获取范围内所有单元格的计数。 |
| [getClass()](#getClass--) |  |
| [getColumnCount()](#getColumnCount--) | 获取范围内的行数。 |
| [getFirstColumn()](#getFirstColumn--) | 获取范围第一列的索引。 |
| [getFirstRow()](#getFirstRow--) | 获取范围第一行的索引。 |
| [getHyperlinks()](#getHyperlinks--) | 获取范围内的所有超链接。 |
| [getName()](#getName--) | 获取范围的名称。 |
| [getRangeCount()](#getRangeCount--) | 获取范围的计数。 |
| [getRanges()](#getRanges--) | 获取所有联合范围。 |
| [getRefersTo()](#getRefersTo--) | 获取范围的引用。 |
| [getRowCount()](#getRowCount--) | 获取范围内的行数。 |
| [getValue()](#getValue--) | 获取范围的值。 |
| [hasRange()](#hasRange--) | 指示此对象是否具有范围。 |
| [hashCode()](#hashCode--) |  |
| [intersect(Range[] ranges)](#intersect-com.aspose.cells.Range---) | 与另一个范围相交。 |
| [intersect(UnionRange unionRange)](#intersect-com.aspose.cells.UnionRange-) | 与另一个范围相交。 |
| [intersect(String range)](#intersect-java.lang.String-) | 与另一个范围相交。 |
| [iterator()](#iterator--) | 获取此 Range 中单元格的枚举器。 |
| [merge()](#merge--) | 将一组单元格合并为单个单元格。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | 将值放入范围中，如有必要，值将被转换为其他数据类型，且单元格的数字格式将被重置。 |
| [setName(String value)](#setName-java.lang.String-) | 设置范围的名称。 |
| [setOutlineBorders(int borderStyle, Color borderColor)](#setOutlineBorders-int-com.aspose.cells.Color-) | 为一组单元格设置相同边框样式和颜色的外部轮廓边框。 |
| [setOutlineBorders(int[] borderStyles, Color[] borderColors)](#setOutlineBorders-int---com.aspose.cells.Color---) | 为一组单元格设置外部轮廓边框。 |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | 设置范围的样式。 |
| [setValue(Object value)](#setValue-java.lang.Object-) | 设置范围的值。 |
| [toString()](#toString--) |  |
| [unMerge()](#unMerge--) | 取消此范围的合并单元格。 |
| [union(Range[] ranges)](#union-com.aspose.cells.Range---) | 合并这些范围。 |
| [union(UnionRange unionRange)](#union-com.aspose.cells.UnionRange-) | 合并另一个范围。 |
| [union(String range)](#union-java.lang.String-) | 合并另一个范围。 |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


对整个范围应用格式。

**Remarks**

此范围中的每个单元格将包含一个 [Style](../../com.aspose.cells/style) 对象。因此这是一个占用内存较多的方法，请谨慎使用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | 将要应用的样式对象。 |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | 指示已应用格式属性的标志。 |

### copy(UnionRange range, PasteOptions options) {#copy-com.aspose.cells.UnionRange-com.aspose.cells.PasteOptions-}
```
public void copy(UnionRange range, PasteOptions options)
```


使用粘贴特殊选项复制范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| range | [UnionRange](../../com.aspose.cells/unionrange) | 源范围。 |
| options | [PasteOptions](../../com.aspose.cells/pasteoptions) | 粘贴特殊选项。 |

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
### getCellCount() {#getCellCount--}
```
public int getCellCount()
```


获取范围内所有单元格的计数。

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


获取范围内的行数。

**Remarks**

仅在仅包含一个范围时生效。

**Returns:**
int
### getFirstColumn() {#getFirstColumn--}
```
public int getFirstColumn()
```


获取范围第一列的索引。

**Remarks**

仅在仅包含一个范围时生效。

**Returns:**
int
### getFirstRow() {#getFirstRow--}
```
public int getFirstRow()
```


获取范围第一行的索引。

**Remarks**

仅在仅包含一个范围时生效。

**Returns:**
int
### getHyperlinks() {#getHyperlinks--}
```
public Hyperlink[] getHyperlinks()
```


获取范围内的所有超链接。

**Returns:**
com.aspose.cells.Hyperlink[]
### getName() {#getName--}
```
public String getName()
```


获取范围的名称。

**Remarks**

支持命名范围。例如，

range.Name = "Sheet1!MyRange";

**Returns:**
java.lang.String
### getRangeCount() {#getRangeCount--}
```
public int getRangeCount()
```


获取范围的计数。

**Returns:**
int
### getRanges() {#getRanges--}
```
public Range[] getRanges()
```


获取所有联合范围。

**Returns:**
com.aspose.cells.Range[]
### getRefersTo() {#getRefersTo--}
```
public String getRefersTo()
```


获取范围的引用。

**Returns:**
java.lang.String
### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


获取范围内的行数。

**Remarks**

仅在仅包含一个范围时生效。

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


获取范围的值。

**Returns:**
java.lang.Object
### hasRange() {#hasRange--}
```
public boolean hasRange()
```


指示此对象是否具有范围。

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### intersect(Range[] ranges) {#intersect-com.aspose.cells.Range---}
```
public UnionRange intersect(Range[] ranges)
```


与另一个范围相交。

**Remarks**

如果两个联合范围未相交，则返回 null。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| ranges | [Range\[\]](../../com.aspose.cells/range) | 范围。 |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange)
### intersect(UnionRange unionRange) {#intersect-com.aspose.cells.UnionRange-}
```
public UnionRange intersect(UnionRange unionRange)
```


与另一个范围相交。

**Remarks**

如果两个联合范围未相交，则返回 null。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| unionRange | [UnionRange](../../com.aspose.cells/unionrange) | 范围。 |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange)
### intersect(String range) {#intersect-java.lang.String-}
```
public UnionRange intersect(String range)
```


与另一个范围相交。

**Remarks**

如果两个联合范围未相交，则返回 null。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 范围 | java.lang.String | 范围。 |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange)
### iterator() {#iterator--}
```
public Iterator iterator()
```


获取此 Range 中单元格的枚举器。

**Remarks**

在使用返回的 Enumerator 遍历元素时，不应修改 cells 集合（例如会导致新建 Cell/Row 或删除现有 Cell/Row 的操作）。否则 Enumerator 可能无法正确遍历所有单元格（某些元素可能被重复遍历或被跳过）。

**Returns:**
java.util.Iterator - cells 枚举器
### merge() {#merge--}
```
public void merge()
```


将一组单元格合并为单个单元格。

**Remarks**

通过范围左上角单元格的地址引用合并单元格。

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### putValue(String stringValue, boolean isConverted, boolean setStyle) {#putValue-java.lang.String-boolean-boolean-}
```
public void putValue(String stringValue, boolean isConverted, boolean setStyle)
```


将值放入范围中，如有必要，值将被转换为其他数据类型，且单元格的数字格式将被重置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stringValue | java.lang.String | 输入值 |
| isConverted | boolean | True: 如适用，转换为其他数据类型。 |
| setStyle | boolean | True: 在转换为其他数据类型时将数字格式设置为单元格的样式 |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


设置范围的名称。

**Remarks**

支持命名范围。例如，

range.Name = "Sheet1!MyRange";

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setOutlineBorders(int borderStyle, Color borderColor) {#setOutlineBorders-int-com.aspose.cells.Color-}
```
public void setOutlineBorders(int borderStyle, Color borderColor)
```


为一组单元格设置相同边框样式和颜色的外部轮廓边框。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype)。边框样式。 |
| borderColor | [Color](../../com.aspose.cells/color) | 边框颜色。 |

### setOutlineBorders(int[] borderStyles, Color[] borderColors) {#setOutlineBorders-int---com.aspose.cells.Color---}
```
public void setOutlineBorders(int[] borderStyles, Color[] borderColors)
```


为一组单元格设置外部轮廓边框。

**Remarks**

borderStyles 和 borderStyles 的长度必须均为 4。borderStyles 的顺序必须为 top,bottom,left,right。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| borderStyles | int[] | [CellBorderType](../../com.aspose.cells/cellbordertype)。边框样式。 |
| borderColors | [Color\[\]](../../com.aspose.cells/color) | 边框颜色。 |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


设置范围的样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Style 对象。 |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


设置范围的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.Object |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unMerge() {#unMerge--}
```
public void unMerge()
```


取消此范围的合并单元格。

### union(Range[] ranges) {#union-com.aspose.cells.Range---}
```
public UnionRange union(Range[] ranges)
```


合并这些范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| ranges | [Range\[\]](../../com.aspose.cells/range) | 这些范围。 |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - 
### union(UnionRange unionRange) {#union-com.aspose.cells.UnionRange-}
```
public UnionRange union(UnionRange unionRange)
```


合并另一个范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| unionRange | [UnionRange](../../com.aspose.cells/unionrange) | 范围。 |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - 
### union(String range) {#union-java.lang.String-}
```
public UnionRange union(String range)
```


合并另一个范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 范围 | java.lang.String | 范围。 |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - 
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

