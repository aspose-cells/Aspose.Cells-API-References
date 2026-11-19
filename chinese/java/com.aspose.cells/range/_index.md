---
title: "Range"
second_title: "Aspose.Cells for Java API 参考"
description: "封装表示电子表格中单元格范围的对象。"
type: docs
url: /zh/java/com.aspose.cells/range/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Range implements Iterable
```

封装表示电子表格中单元格范围的对象。

**Remarks**

Range 类表示 Excel 电子表格的一个区域。使用它，您可以格式化并设置该区域的值。并且您也可以轻松复制 Excel 的区域。

**Example**

下面的示例展示了如何创建一个范围并设置 Excel 范围的值。

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         // Get the first Worksheet Cells.
         Cells cells = workbook.getWorksheets().get(0).getCells();
         // Create a range (A1:D3).
         Range range = cells.createRange("A1", "D3");
         // Set value to the range.
         range.setValue("Hello");
         //Save the Excel file
         workbook.save("book1.xlsm");
```
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [Range(CellArea ca, Cells cells)](#Range-com.aspose.cells.CellArea-com.aspose.cells.Cells-) | 类构造函数。 |
| [Range(int firstRow, int firstColumn, int rowNumber, int columnNumber, Cells cells)](#Range-int-int-int-int-com.aspose.cells.Cells-) | 类构造函数。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [addHyperlink(String address, String textToDisplay, String screenTip)](#addHyperlink-java.lang.String-java.lang.String-java.lang.String-) | 向指定的单元格或单元格范围添加超链接。 |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | 对整个范围应用格式。 |
| [autoFill(Range target)](#autoFill-com.aspose.cells.Range-) | 自动填充目标范围。 |
| [autoFill(Range target, int autoFillType)](#autoFill-com.aspose.cells.Range-int-) | 自动填充目标范围。 |
| [clear()](#clear--) | 清除此范围。 |
| [clearComments()](#clearComments--) | 清除此范围的批注。 |
| [clearContents()](#clearContents--) | 清除此范围的内容。 |
| [clearFormats()](#clearFormats--) | 清除此范围的格式。 |
| [clearHyperlinks(boolean clearFormat)](#clearHyperlinks-boolean-) | 仅移除超链接。 |
| [copy(Range range)](#copy-com.aspose.cells.Range-) | 从源范围复制数据（包括公式）、格式、绘图对象等。 |
| [copy(Range range, PasteOptions options)](#copy-com.aspose.cells.Range-com.aspose.cells.PasteOptions-) | 使用粘贴特殊选项复制范围。 |
| [copyData(Range range)](#copyData-com.aspose.cells.Range-) | 从源范围复制单元格数据（包括公式）。 |
| [copyStyle(Range range)](#copyStyle-com.aspose.cells.Range-) | 从源范围复制样式设置。 |
| [copyValue(Range range)](#copyValue-com.aspose.cells.Range-) | 从源范围复制单元格值。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int rowOffset, int columnOffset)](#get-int-int-) | 获取此范围内的 [Cell](../../com.aspose.cells/cell) 对象。 |
| [getAddress()](#getAddress--) | 获取范围的地址。 |
| [getCellOrNull(int rowOffset, int columnOffset)](#getCellOrNull-int-int-) | 获取此范围内的 [Cell](../../com.aspose.cells/cell) 对象或 null。 |
| [getClass()](#getClass--) |  |
| [getColumnCount()](#getColumnCount--) | 获取范围内的列数。 |
| [getColumnWidth()](#getColumnWidth--) | 设置或获取此范围的列宽 |
| [getCurrentRegion()](#getCurrentRegion--) | 返回表示当前区域的 Range 对象。 |
| [getEntireColumn()](#getEntireColumn--) | 获取表示包含指定范围的整列（或多列）的 Range 对象。 |
| [getEntireRow()](#getEntireRow--) | 获取表示包含指定范围的整行（或多行）的 Range 对象。 |
| [getFirstColumn()](#getFirstColumn--) | 获取范围第一列的索引。 |
| [getFirstRow()](#getFirstRow--) | 获取范围第一行的索引。 |
| [getHeight()](#getHeight--) | 获取范围的宽度（单位：磅）。 |
| [getHyperlinks()](#getHyperlinks--) | 获取范围内的所有超链接。 |
| [getLeft()](#getLeft--) | 获取从列 A 左边缘到范围左边缘的距离（单位：磅）。 |
| [getName()](#getName--) | 获取范围的名称。 |
| [getOffset(int rowOffset, int columnOffset)](#getOffset-int-int-) | 通过偏移获取 [Range](../../com.aspose.cells/range) 范围。 |
| [getRefersTo()](#getRefersTo--) | 获取范围的引用。 |
| [getRowCount()](#getRowCount--) | 获取范围内的行数。 |
| [getRowHeight()](#getRowHeight--) | 设置或获取此范围内行的高度 |
| [getTop()](#getTop--) | 获取从第 1 行顶部到范围顶部的距离（单位：磅）。 |
| [getValue()](#getValue--) | 获取范围的值。 |
| [getWidth()](#getWidth--) | 获取范围的宽度（单位：磅）。 |
| [getWorksheet()](#getWorksheet--) | 获取包含此范围的 [getWorksheet()](../../com.aspose.cells/range\\#getWorksheet--) 对象。 |
| [hashCode()](#hashCode--) |  |
| [intersect(Range range)](#intersect-com.aspose.cells.Range-) | 返回表示两个范围矩形交集的 [Range](../../com.aspose.cells/range) 对象。 |
| [isBlank()](#isBlank--) | 指示范围是否包含值。 |
| [isIntersect(Range range)](#isIntersect-com.aspose.cells.Range-) | 指示该范围是否相交。 |
| [iterator()](#iterator--) | 获取此 Range 中单元格的枚举器。 |
| [merge()](#merge--) | 将一组单元格合并为单个单元格。 |
| [moveTo(int destRow, int destColumn)](#moveTo-int-int-) | 将当前范围移动到目标范围。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | 将值放入范围中，如有必要，值将被转换为其他数据类型，且单元格的数字格式将被重置。 |
| [setColumnWidth(double value)](#setColumnWidth-double-) | 设置或获取此范围的列宽 |
| [setInsideBorders(int borderEdge, int lineStyle, CellsColor borderColor)](#setInsideBorders-int-int-com.aspose.cells.CellsColor-) | 设置范围的内部边框。 |
| [setName(String value)](#setName-java.lang.String-) | 设置范围的名称。 |
| [setOutlineBorder(int borderEdge, int borderStyle, CellsColor borderColor)](#setOutlineBorder-int-int-com.aspose.cells.CellsColor-) | 为一组单元格设置外部轮廓边框。 |
| [setOutlineBorder(int borderEdge, int borderStyle, Color borderColor)](#setOutlineBorder-int-int-com.aspose.cells.Color-) | 为一组单元格设置外部轮廓边框。 |
| [setOutlineBorders(int borderStyle, CellsColor borderColor)](#setOutlineBorders-int-com.aspose.cells.CellsColor-) | 为一组单元格设置相同边框样式和颜色的外部轮廓边框。 |
| [setOutlineBorders(int borderStyle, Color borderColor)](#setOutlineBorders-int-com.aspose.cells.Color-) | 为一组单元格设置相同边框样式和颜色的外部轮廓边框。 |
| [setOutlineBorders(int[] borderStyles, Color[] borderColors)](#setOutlineBorders-int---com.aspose.cells.Color---) | 为一组单元格设置外部轮廓边框。 |
| [setRowHeight(double value)](#setRowHeight-double-) | 设置或获取此范围内行的高度 |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | 设置范围的样式。 |
| [setStyle(Style style, boolean explicitFlag)](#setStyle-com.aspose.cells.Style-boolean-) | 应用单元格样式。 |
| [setValue(Object value)](#setValue-java.lang.Object-) | 设置范围的值。 |
| [toHtml(HtmlSaveOptions saveOptions)](#toHtml-com.aspose.cells.HtmlSaveOptions-) | 将范围转换为 HTML。 |
| [toImage(ImageOrPrintOptions options)](#toImage-com.aspose.cells.ImageOrPrintOptions-) | 将范围转换为图像。 |
| [toJson(JsonSaveOptions options)](#toJson-com.aspose.cells.JsonSaveOptions-) | 将范围转换为 JSON 值。 |
| [toString()](#toString--) | 返回表示当前 Range 对象的字符串。 |
| [transpose()](#transpose--) | 转置（旋转）数据，将行转换为列或反之。 |
| [unMerge()](#unMerge--) | 取消此范围的合并单元格。 |
| [union(Range range)](#union-com.aspose.cells.Range-) | 返回两个范围的并集。 |
| [unionRang(Range range)](#unionRang-com.aspose.cells.Range-) | 返回两个范围的并集结果。 |
| [unionRanges(Range[] ranges)](#unionRanges-com.aspose.cells.Range---) | 返回两个范围的并集结果。 |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Range(CellArea ca, Cells cells) {#Range-com.aspose.cells.CellArea-com.aspose.cells.Cells-}
```
public Range(CellArea ca, Cells cells)
```


类构造函数。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | 范围。 |
| cells | [Cells](../../com.aspose.cells/cells) |  |

### Range(int firstRow, int firstColumn, int rowNumber, int columnNumber, Cells cells) {#Range-int-int-int-int-com.aspose.cells.Cells-}
```
public Range(int firstRow, int firstColumn, int rowNumber, int columnNumber, Cells cells)
```


类构造函数。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| firstRow | int | 此范围的第一行（零基）。 |
| firstColumn | int | 此范围的第一列（零基） |
| rowNumber | int | 行数（从一开始计）。 |
| columnNumber | int | 列数（从一开始计）。 |
| cells | [Cells](../../com.aspose.cells/cells) | 此 Range 对象属于该 Cells 对象 |

### addHyperlink(String address, String textToDisplay, String screenTip) {#addHyperlink-java.lang.String-java.lang.String-java.lang.String-}
```
public Hyperlink addHyperlink(String address, String textToDisplay, String screenTip)
```


向指定的单元格或单元格范围添加超链接。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 地址 | java.lang.String | 超链接的地址。 |
| textToDisplay | java.lang.String | 指定超链接要显示的文本。 |
| screenTip | java.lang.String | 指定超链接的屏幕提示文本。 |

**Returns:**
[Hyperlink](../../com.aspose.cells/hyperlink) - [Hyperlink](../../com.aspose.cells/hyperlink) object.
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

### autoFill(Range target) {#autoFill-com.aspose.cells.Range-}
```
public void autoFill(Range target)
```


自动填充目标范围。

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         // Get the first Worksheet Cells.
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("A1").putValue(1);
         cells.get("A2").putValue(2);
         Range source = cells.createRange("A1:A2");
         Range target = cells.createRange("A3:A10");
         //fill 3,4,5....10 to the range A3:A10
         source.autoFill(target);
         //Save the Excel file
         workbook.save("book1.xlsm");
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| target | [Range](../../com.aspose.cells/range) | 目标范围。 |

### autoFill(Range target, int autoFillType) {#autoFill-com.aspose.cells.Range-int-}
```
public void autoFill(Range target, int autoFillType)
```


自动填充目标范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| target | [Range](../../com.aspose.cells/range) | 目标范围。 |
| autoFillType | int | [AutoFillType](../../com.aspose.cells/autofilltype)。自动填充类型。 |

### clear() {#clear--}
```
public void clear()
```


清除此范围。

### clearComments() {#clearComments--}
```
public void clearComments()
```


清除此范围的批注。

### clearContents() {#clearContents--}
```
public void clearContents()
```


清除此范围的内容。

### clearFormats() {#clearFormats--}
```
public void clearFormats()
```


清除此范围的格式。

### clearHyperlinks(boolean clearFormat) {#clearHyperlinks-boolean-}
```
public void clearHyperlinks(boolean clearFormat)
```


仅移除超链接。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| clearFormat | boolean | 指示是否清除超链接的格式。 |

### copy(Range range) {#copy-com.aspose.cells.Range-}
```
public void copy(Range range)
```


从源范围复制数据（包括公式）、格式、绘图对象等。

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         // Get the first Worksheet Cells.
         Cells cells = workbook.getWorksheets().get(0).getCells();
         Range range1 = cells.createRange("A1:A5");
         Range range2 = cells.createRange("A6:A10");
         //Copy the range.
         range1.copy(range2);
         //Save the Excel file
         workbook.save("book1.xlsm");
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | 源 [Range](../../com.aspose.cells/range) 对象。 |

### copy(Range range, PasteOptions options) {#copy-com.aspose.cells.Range-com.aspose.cells.PasteOptions-}
```
public void copy(Range range, PasteOptions options)
```


使用粘贴特殊选项复制范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | 源范围。 |
| options | [PasteOptions](../../com.aspose.cells/pasteoptions) | 粘贴特殊选项。 |

### copyData(Range range) {#copyData-com.aspose.cells.Range-}
```
public void copyData(Range range)
```


从源范围复制单元格数据（包括公式）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | 源 [Range](../../com.aspose.cells/range) 对象。 |

### copyStyle(Range range) {#copyStyle-com.aspose.cells.Range-}
```
public void copyStyle(Range range)
```


从源范围复制样式设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | 源 [Range](../../com.aspose.cells/range) 对象。 |

### copyValue(Range range) {#copyValue-com.aspose.cells.Range-}
```
public void copyValue(Range range)
```


从源范围复制单元格值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | 源 [Range](../../com.aspose.cells/range) 对象。 |

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
### get(int rowOffset, int columnOffset) {#get-int-int-}
```
public Cell get(int rowOffset, int columnOffset)
```


获取此范围内的 [Cell](../../com.aspose.cells/cell) 对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowOffset | int | 此范围内的行偏移量，基于零。 |
| columnOffset | int | 此范围内的列偏移量，基于零。 |

**Returns:**
[Cell](../../com.aspose.cells/cell) - [Cell](../../com.aspose.cells/cell) object.
### getAddress() {#getAddress--}
```
public String getAddress()
```


获取范围的地址。

**Returns:**
java.lang.String
### getCellOrNull(int rowOffset, int columnOffset) {#getCellOrNull-int-int-}
```
public Cell getCellOrNull(int rowOffset, int columnOffset)
```


获取此范围内的 [Cell](../../com.aspose.cells/cell) 对象或 null。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowOffset | int | 此范围内的行偏移量，基于零。 |
| columnOffset | int | 此范围内的列偏移量，基于零。 |

**Returns:**
[Cell](../../com.aspose.cells/cell) - [Cell](../../com.aspose.cells/cell) object.
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


获取范围内的列数。

**Returns:**
int
### getColumnWidth() {#getColumnWidth--}
```
public double getColumnWidth()
```


设置或获取此范围的列宽

**Returns:**
double
### getCurrentRegion() {#getCurrentRegion--}
```
public Range getCurrentRegion()
```


返回表示当前区域的 Range 对象。当前区域是由任意组合的空行和空列界定的范围。

**Returns:**
[Range](../../com.aspose.cells/range)
### getEntireColumn() {#getEntireColumn--}
```
public Range getEntireColumn()
```


获取表示包含指定范围的整列（或多列）的 Range 对象。

**Returns:**
[Range](../../com.aspose.cells/range)
### getEntireRow() {#getEntireRow--}
```
public Range getEntireRow()
```


获取表示包含指定范围的整行（或多行）的 Range 对象。

**Returns:**
[Range](../../com.aspose.cells/range)
### getFirstColumn() {#getFirstColumn--}
```
public int getFirstColumn()
```


获取范围第一列的索引。

**Returns:**
int
### getFirstRow() {#getFirstRow--}
```
public int getFirstRow()
```


获取范围第一行的索引。

**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```


获取范围的宽度（单位：磅）。

**Returns:**
double
### getHyperlinks() {#getHyperlinks--}
```
public Hyperlink[] getHyperlinks()
```


获取范围内的所有超链接。

**Returns:**
com.aspose.cells.Hyperlink[]
### getLeft() {#getLeft--}
```
public double getLeft()
```


获取从列 A 左边缘到范围左边缘的距离（单位：磅）。

**Returns:**
double
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
### getOffset(int rowOffset, int columnOffset) {#getOffset-int-int-}
```
public Range getOffset(int rowOffset, int columnOffset)
```


通过偏移获取 [Range](../../com.aspose.cells/range) 范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowOffset | int | 此范围内的行偏移量，基于零。 |
| columnOffset | int | 此范围内的列偏移量，基于零。 |

**Returns:**
[Range](../../com.aspose.cells/range) - 
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

**Returns:**
int
### getRowHeight() {#getRowHeight--}
```
public double getRowHeight()
```


设置或获取此范围内行的高度

**Returns:**
double
### getTop() {#getTop--}
```
public double getTop()
```


获取从第 1 行顶部到范围顶部的距离（单位：磅）。

**Returns:**
double
### getValue() {#getValue--}
```
public Object getValue()
```


获取范围的值。

**Remarks**

如果范围包含多个单元格，返回/应用的对象应为 Object[][].

**Returns:**
java.lang.Object
### getWidth() {#getWidth--}
```
public double getWidth()
```


获取范围的宽度（单位：磅）。

**Returns:**
double
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


获取包含此范围的 [getWorksheet()](../../com.aspose.cells/range\\#getWorksheet--) 对象。

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### intersect(Range range) {#intersect-com.aspose.cells.Range-}
```
public Range intersect(Range range)
```


返回表示两个范围矩形交集的 [Range](../../com.aspose.cells/range) 对象。

**Remarks**

如果两个范围未相交，返回 null。

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         // Get the first Worksheet Cells.
         Cells cells = workbook.getWorksheets().get(0).getCells();
         Range range1 = cells.createRange("A1:A5");
         Range range2 = cells.createRange("A3:A10");
         //Get intersected range of the two ranges.
         Range intersectRange = range1.intersect(range2);
         //Save the Excel file
         workbook.save("book1.xlsm");
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | 相交的范围。 |

**Returns:**
[Range](../../com.aspose.cells/range) - Returns a [Range](../../com.aspose.cells/range) object
### isBlank() {#isBlank--}
```
public boolean isBlank()
```


指示范围是否包含值。

**Returns:**
boolean -
### isIntersect(Range range) {#isIntersect-com.aspose.cells.Range-}
```
public boolean isIntersect(Range range)
```


指示该范围是否相交。

**Remarks**

如果两个范围不在同一工作表中，返回 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | 范围。 |

**Returns:**
boolean - 范围是否相交。
### iterator() {#iterator--}
```
public Iterator iterator()
```


获取此 Range 中单元格的枚举器。

**Remarks**

在使用返回的 Enumerator 遍历元素时，不应修改 cells 集合（例如会导致新建 Cell/Row 或删除现有 Cell/Row 的操作）。否则 Enumerator 可能无法正确遍历所有单元格（某些元素可能被重复遍历或被跳过）。

**Example**

```
         Workbook workbook = new Workbook("template.xlsx");
         	Cells cells = workbook.getWorksheets().get(0).getCells();
 
         	Iterator en = cells.createRange("B2:C3").iterator();
         	while (en.hasNext())
         	{
         	    Cell cell = (Cell)en.next();
         	    System.out.println(cell.getName() + ": " + cell.getValue());
         	}
```

**Returns:**
java.util.Iterator - cells 枚举器
### merge() {#merge--}
```
public void merge()
```


将一组单元格合并为单个单元格。

**Remarks**

通过范围左上角单元格的地址引用合并单元格。

### moveTo(int destRow, int destColumn) {#moveTo-int-int-}
```
public void moveTo(int destRow, int destColumn)
```


将当前范围移动到目标范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| destRow | int | 目标范围的起始行。 |
| destColumn | int | 目标范围的起始列。 |

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

### setColumnWidth(double value) {#setColumnWidth-double-}
```
public void setColumnWidth(double value)
```


设置或获取此范围的列宽

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setInsideBorders(int borderEdge, int lineStyle, CellsColor borderColor) {#setInsideBorders-int-int-com.aspose.cells.CellsColor-}
```
public void setInsideBorders(int borderEdge, int lineStyle, CellsColor borderColor)
```


设置范围的内部边框。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| borderEdge | int | [BorderType](../../com.aspose.cells/bordertype)。在边框类型内部，只能是 [BorderType.VERTICAL](../../com.aspose.cells/bordertype\#VERTICAL) 和 [BorderType.HORIZONTAL](../../com.aspose.cells/bordertype\#HORIZONTAL)。 |
| lineStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype)。边框样式。 |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | 边框的颜色。 |

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

### setOutlineBorder(int borderEdge, int borderStyle, CellsColor borderColor) {#setOutlineBorder-int-int-com.aspose.cells.CellsColor-}
```
public void setOutlineBorder(int borderEdge, int borderStyle, CellsColor borderColor)
```


为一组单元格设置外部轮廓边框。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| borderEdge | int | [BorderType](../../com.aspose.cells/bordertype)。边框边缘。 |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype)。边框样式。 |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | 边框颜色。 |

### setOutlineBorder(int borderEdge, int borderStyle, Color borderColor) {#setOutlineBorder-int-int-com.aspose.cells.Color-}
```
public void setOutlineBorder(int borderEdge, int borderStyle, Color borderColor)
```


为一组单元格设置外部轮廓边框。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| borderEdge | int | [BorderType](../../com.aspose.cells/bordertype)。边框边缘。 |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype)。边框样式。 |
| borderColor | [Color](../../com.aspose.cells/color) | 边框颜色。 |

### setOutlineBorders(int borderStyle, CellsColor borderColor) {#setOutlineBorders-int-com.aspose.cells.CellsColor-}
```
public void setOutlineBorders(int borderStyle, CellsColor borderColor)
```


为一组单元格设置相同边框样式和颜色的外部轮廓边框。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype)。边框样式。 |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | 边框颜色。 |

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

### setRowHeight(double value) {#setRowHeight-double-}
```
public void setRowHeight(double value)
```


设置或获取此范围内行的高度

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


设置范围的样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Style 对象。 |

### setStyle(Style style, boolean explicitFlag) {#setStyle-com.aspose.cells.Style-boolean-}
```
public void setStyle(Style style, boolean explicitFlag)
```


应用单元格样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | 单元格样式。 |
| explicitFlag | boolean | True，仅覆盖已显式设置的格式。 |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


设置范围的值。

**Remarks**

如果范围包含多个单元格，返回/应用的对象应为 Object[][].

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.Object |  |

### toHtml(HtmlSaveOptions saveOptions) {#toHtml-com.aspose.cells.HtmlSaveOptions-}
```
public byte[] toHtml(HtmlSaveOptions saveOptions)
```


将范围转换为 HTML。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| saveOptions | [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions) | 将范围转换为 HTML 的选项。 |

**Returns:**
byte[] -
### toImage(ImageOrPrintOptions options) {#toImage-com.aspose.cells.ImageOrPrintOptions-}
```
public byte[] toImage(ImageOrPrintOptions options)
```


将范围转换为图像。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | 将此范围转换为图像的选项 |

**Returns:**
byte[] -
### toJson(JsonSaveOptions options) {#toJson-com.aspose.cells.JsonSaveOptions-}
```
public String toJson(JsonSaveOptions options)
```


将范围转换为 JSON 值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| options | [JsonSaveOptions](../../com.aspose.cells/jsonsaveoptions) | 转换的选项 |

**Returns:**
java.lang.String -
### toString() {#toString--}
```
public String toString()
```


返回表示当前 Range 对象的字符串。

**Returns:**
java.lang.String -
### transpose() {#transpose--}
```
public void transpose()
```


转置（旋转）数据，将行转换为列或反之。

### unMerge() {#unMerge--}
```
public void unMerge()
```


取消此范围的合并单元格。

### union(Range range) {#union-com.aspose.cells.Range-}
```
public ArrayList union(Range range)
```


返回两个范围的并集。

**Remarks**

注意：此方法已过时。请改用 Range.UnionRanges() 方法。该方法将在自 2023 年 11 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | 范围 |

**Returns:**
java.util.ArrayList - 两个范围的并集。
### unionRang(Range range) {#unionRang-com.aspose.cells.Range-}
```
public Range[] unionRang(Range range)
```


返回两个范围的并集结果。

**Remarks**

注意：此方法已过时。请改用 Range.UnionRanges() 方法。该方法将在自 2024 年 5 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | 范围 |

**Returns:**
com.aspose.cells.Range[] - 两个范围的并集。
### unionRanges(Range[] ranges) {#unionRanges-com.aspose.cells.Range---}
```
public UnionRange unionRanges(Range[] ranges)
```


返回两个范围的并集结果。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| ranges | [Range\[\]](../../com.aspose.cells/range) | 范围 |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - The union of two ranges.
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

