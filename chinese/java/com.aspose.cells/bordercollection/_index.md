---
title: "BorderCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "封装一个对象集合。"
type: docs
url: /zh/java/com.aspose.cells/bordercollection/
---

**Inheritance:**
java.lang.Object
```
public class BorderCollection
```

封装一个 [Border](../../com.aspose.cells/border) 对象的集合。

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Adding a new worksheet to the Excel object
         workbook.getWorksheets().add();
 
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Accessing the "A1" cell from the worksheet
         Cell cell = worksheet.getCells().get("A1");
 
         //Adding some value to the "A1" cell
         cell.putValue("Visit Aspose!");
 
         Style style = cell.getStyle();
 
         //Setting the line style of the top border
         style.getBorders().getByBorderType(BorderType.TOP_BORDER).setLineStyle(CellBorderType.THICK);
 
         //Setting the color of the top border
         style.getBorders().getByBorderType(BorderType.TOP_BORDER).setColor(Color.getBlack());
 
         //Setting the line style of the bottom border
         style.getBorders().getByBorderType(BorderType.BOTTOM_BORDER).setLineStyle(CellBorderType.THICK);
 
         //Setting the color of the bottom border
         style.getBorders().getByBorderType(BorderType.BOTTOM_BORDER).setColor(Color.getBlack());
 
         //Setting the line style of the left border
         style.getBorders().getByBorderType(BorderType.LEFT_BORDER).setLineStyle(CellBorderType.THICK);
 
         //Setting the color of the left border
         style.getBorders().getByBorderType(BorderType.LEFT_BORDER).setColor(Color.getBlack());
 
         //Setting the line style of the right border
         style.getBorders().getByBorderType(BorderType.RIGHT_BORDER).setLineStyle(CellBorderType.THICK);
 
         //Setting the color of the right border
         style.getBorders().getByBorderType(BorderType.RIGHT_BORDER).setColor(Color.getBlack());
 
         cell.setStyle(style);
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getByBorderType(int borderType)](#getByBorderType-int-) | 获取指定索引处的 [Border](../../com.aspose.cells/border) 元素。 |
| [getClass()](#getClass--) |  |
| [getDiagonalColor()](#getDiagonalColor--) | 获取对角线的 [Color](../../com.aspose.cells/color)。 |
| [getDiagonalStyle()](#getDiagonalStyle--) | 获取对角线的样式。 |
| [hashCode()](#hashCode--) |  |
| [isOutline()](#isOutline--) | 指示是否仅将左、右、上、下边框应用于单元格范围的外部边框。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setColor(Color color)](#setColor-com.aspose.cells.Color-) | 设置集合中所有边框的 [Color](../../com.aspose.cells/color)。 |
| [setDiagonalColor(Color value)](#setDiagonalColor-com.aspose.cells.Color-) | 设置对角线的 [Color](../../com.aspose.cells/color)。 |
| [setDiagonalStyle(int value)](#setDiagonalStyle-int-) | 设置对角线的样式。 |
| [setOutline(boolean value)](#setOutline-boolean-) | 指示是否仅将左、右、上、下边框应用于单元格范围的外部边框。 |
| [setStyle(int style)](#setStyle-int-) | 设置集合中所有边框的样式。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getByBorderType(int borderType) {#getByBorderType-int-}
```
public Border getByBorderType(int borderType)
```


获取指定索引处的 [Border](../../com.aspose.cells/border) 元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| borderType | int | [BorderType](../../com.aspose.cells/bordertype)。要检索的边框。 |

**Returns:**
[Border](../../com.aspose.cells/border) - The element at the specified index.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDiagonalColor() {#getDiagonalColor--}
```
public Color getDiagonalColor()
```


获取对角线的 [Color](../../com.aspose.cells/color)。

**Returns:**
[Color](../../com.aspose.cells/color)
### getDiagonalStyle() {#getDiagonalStyle--}
```
public int getDiagonalStyle()
```


获取对角线的样式。

参见 [CellBorderType](../../com.aspose.cells/cellbordertype)。

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isOutline() {#isOutline--}
```
public boolean isOutline()
```


指示是否仅将左、右、上、下边框应用于单元格范围的外部边框。默认值为 true。

**Remarks**

仅在对条件格式、数据透视表的范围应用时有效。如果为 false，左、右、上、下将应用于每个单元格；否则仅应用于单元格范围的外部边框。如果为 true，请为条件格式、数据透视表的范围设置内部水平和垂直边框。

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




### setColor(Color color) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color color)
```


设置集合中所有边框的 [Color](../../com.aspose.cells/color)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | 边框的 [Color](../../com.aspose.cells/color)。 |

### setDiagonalColor(Color value) {#setDiagonalColor-com.aspose.cells.Color-}
```
public void setDiagonalColor(Color value)
```


设置对角线的 [Color](../../com.aspose.cells/color)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setDiagonalStyle(int value) {#setDiagonalStyle-int-}
```
public void setDiagonalStyle(int value)
```


设置对角线的样式。

参见 [CellBorderType](../../com.aspose.cells/cellbordertype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setOutline(boolean value) {#setOutline-boolean-}
```
public void setOutline(boolean value)
```


指示是否仅将左、右、上、下边框应用于单元格范围的外部边框。默认值为 true。

**Remarks**

仅在对条件格式、数据透视表的范围应用时有效。如果为 false，左、右、上、下将应用于每个单元格；否则仅应用于单元格范围的外部边框。如果为 true，请为条件格式、数据透视表的范围设置内部水平和垂直边框。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setStyle(int style) {#setStyle-int-}
```
public void setStyle(int style)
```


设置集合中所有边框的样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| style | int | [CellBorderType](../../com.aspose.cells/cellbordertype)。边框的样式 |

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

