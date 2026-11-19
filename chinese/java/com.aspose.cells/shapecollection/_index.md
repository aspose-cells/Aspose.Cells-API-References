---
title: "ShapeCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "表示工作表/图表中的所有形状。"
type: docs
url: /zh/java/com.aspose.cells/shapecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ShapeCollection extends CollectionBase
```

表示工作表/图表中的所有形状。

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //get ShapeCollection
         ShapeCollection shapes = workbook.getWorksheets().get(0).getShapes();
 
         //do your business
 
         //Save the excel file.
         workbook.save("result.xlsx");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | 向 CollectionBase 实例添加一个项。 |
| [addActiveXControl(int type, int topRow, int top, int leftColumn, int left, int width, int height)](#addActiveXControl-int-int-int-int-int-int-int-) | 创建一个 Activex 控件。 |
| [addArc(int topRow, int top, int leftColumn, int left, int height, int width)](#addArc-int-int-int-int-int-int-) | 向工作表添加一个 ArcShape。 |
| [addAutoShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)](#addAutoShape-int-int-int-int-int-int-int-) | 向工作表添加一个 AutoShape。 |
| [addAutoShapeInChart(int type, int top, int left, int height, int width)](#addAutoShapeInChart-int-int-int-int-int-) | 向图表添加一个 AutoShape。 |
| [addButton(int topRow, int top, int leftColumn, int left, int height, int width)](#addButton-int-int-int-int-int-int-) | 向工作表添加一个 Button。 |
| [addCheckBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addCheckBox-int-int-int-int-int-int-) | 向工作表添加一个复选框。 |
| [addComboBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addComboBox-int-int-int-int-int-int-) | 向工作表添加一个 ComboBox。 |
| [addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left)](#addCopy-com.aspose.cells.Shape-int-int-int-int-) | 向工作表添加并复制一个形状。 |
| [addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left, CopyOptions copyOptions)](#addCopy-com.aspose.cells.Shape-int-int-int-int-com.aspose.cells.CopyOptions-) | 向工作表添加并复制一个形状。 |
| [addEquation(int topRow, int top, int leftColumn, int left, int height, int width)](#addEquation-int-int-int-int-int-int-) | 向工作表添加一个公式对象。 |
| [addFreeFloatingShape(int type, int top, int left, int height, int width, byte[] imageData, boolean isOriginalSize)](#addFreeFloatingShape-int-int-int-int-int-byte---boolean-) | 向工作表添加一个自由浮动形状。仅适用于线条/图像形状。 |
| [addFreeform(int topRow, int top, int leftColumn, int left, int height, int width, ShapePath[] paths)](#addFreeform-int-int-int-int-int-int-com.aspose.cells.ShapePath---) | 向工作表添加一个自由形状。 |
| [addGroupBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addGroupBox-int-int-int-int-int-int-) | 向工作表添加一个 GroupBox。 |
| [addIcons(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageByteData, byte[] compatibleImageData)](#addIcons-int-int-int-int-int-int-byte---byte---) | 添加 svg 图像。 |
| [addLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, int width, String latex)](#addLaTeXEquation-int-int-int-int-int-int-java.lang.String-) | 使用 LaTeX 格式字符串向工作表添加一个公式对象。 |
| [addLabel(int topRow, int top, int leftColumn, int left, int height, int width)](#addLabel-int-int-int-int-int-int-) | 向工作表添加一个标签。 |
| [addLabelInChart(int top, int left, int height, int width)](#addLabelInChart-int-int-int-int-) | 向图表添加一个标签。 |
| [addLine(int topRow, int top, int leftColumn, int left, int height, int width)](#addLine-int-int-int-int-int-int-) | 向工作表添加一个线形状。 |
| [addLinkedPicture(int topRow, int leftColumn, int height, int width, String sourceFullName)](#addLinkedPicture-int-int-int-int-java.lang.String-) | 添加一个链接图片。 |
| [addListBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addListBox-int-int-int-int-int-int-) | 向工作表添加一个 ListBox。 |
| [addOleObject(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageData)](#addOleObject-int-int-int-int-int-int-byte---) | 添加一个 OleObject。 |
| [addOleObjectWithLinkedImage(int topRow, int leftColumn, int height, int width, String sourceFullName)](#addOleObjectWithLinkedImage-int-int-int-int-java.lang.String-) | 添加一个链接图片。 |
| [addOval(int topRow, int top, int leftColumn, int left, int height, int width)](#addOval-int-int-int-int-int-int-) | 向工作表添加一个椭圆。 |
| [addPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream)](#addPicture-int-int-int-int-java.io.InputStream-) | 向集合中添加一张图片。 |
| [addPicture(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale)](#addPicture-int-int-java.io.InputStream-int-int-) | 向集合中添加一张图片。 |
| [addPictureInChart(int top, int left, InputStream stream, int widthScale, int heightScale)](#addPictureInChart-int-int-java.io.InputStream-int-int-) | 向图表中添加一张图片。 |
| [addRadioButton(int topRow, int top, int leftColumn, int left, int height, int width)](#addRadioButton-int-int-int-int-int-int-) | 向工作表添加一个 RadioButton。 |
| [addRectangle(int topRow, int top, int leftColumn, int left, int height, int width)](#addRectangle-int-int-int-int-int-int-) | 向工作表添加一个矩形形状。 |
| [addScrollBar(int topRow, int top, int leftColumn, int left, int height, int width)](#addScrollBar-int-int-int-int-int-int-) | 向工作表添加一个滚动条。 |
| [addShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)](#addShape-int-int-int-int-int-int-int-) | 向工作表添加一个形状。 |
| [addShapeInChart(int type, int placement, int left, int top, int right, int bottom)](#addShapeInChart-int-int-int-int-int-int-) | 向图表添加形状。所有单位为图表区域的 1/4000。 |
| [addShapeInChart(int type, int placement, int left, int top, int right, int bottom, byte[] imageData)](#addShapeInChart-int-int-int-int-int-int-byte---) | 向图表添加形状。所有单位为图表区域的 1/4000。 |
| [addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom)](#addShapeInChartByScale-int-int-double-double-double-double-) | 向图表添加形状。 |
| [addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom, byte[] imageData)](#addShapeInChartByScale-int-int-double-double-double-double-byte---) | 向图表添加形状。所有单位为图表区域的 1/4000。 |
| [addSignatureLine(int topRow, int leftColumn, SignatureLine signatureLine)](#addSignatureLine-int-int-com.aspose.cells.SignatureLine-) | 向工作表添加一个签名线。 |
| [addSpinner(int topRow, int top, int leftColumn, int left, int height, int width)](#addSpinner-int-int-int-int-int-int-) | 向工作表添加一个微调框。 |
| [addSvg(int topRow, int top, int leftColumn, int left, int height, int width, byte[] svgData, byte[] compatibleImageData)](#addSvg-int-int-int-int-int-int-byte---byte---) | 添加 svg 图像。 |
| [addTextBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addTextBox-int-int-int-int-int-int-) | 向工作表添加文本框。 |
| [addTextBoxInChart(int top, int left, int height, int width)](#addTextBoxInChart-int-int-int-int-) | 向图表添加文本框。 |
| [addTextEffect(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int topRow, int top, int leftColumn, int left, int height, int width)](#addTextEffect-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-int-int-) | 插入 WordArt 对象。 |
| [addTextEffectInChart(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int top, int left, int height, int width)](#addTextEffectInChart-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-) | 向图表插入 WordArt 对象 |
| [addWordArt(int style, String text, int topRow, int top, int leftColumn, int left, int height, int width)](#addWordArt-int-java.lang.String-int-int-int-int-int-int-) | 自 Excel 2007 起添加预设 WordArt。 |
| [clear()](#clear--) | 清除工作表中的所有形状。 |
| [contains(Object o)](#contains-java.lang.Object-) | 返回实例是否包含此对象 |
| [copyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn)](#copyCommentsInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-) | 复制范围内的所有批注。 |
| [copyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, boolean isContained)](#copyInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-boolean-) | 将范围内的形状复制到目标范围。 |
| [deleteInRange(CellArea ca)](#deleteInRange-com.aspose.cells.CellArea-) | 删除范围内的形状。注释形状将不会被删除。 |
| [deleteShape(Shape shape)](#deleteShape-com.aspose.cells.Shape-) | 删除形状。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [find(String what, int previous, FindOptions findOptions)](#find-java.lang.String-int-com.aspose.cells.FindOptions-) | 按文本查找形状 |
| [get(int index)](#get-int-) | 获取列表中特定索引的 [Shape](../../com.aspose.cells/shape) 对象。 |
| [get(String name)](#get-java.lang.String-) | 通过形状名称获取 [Shape](../../com.aspose.cells/shape) 对象。 |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | 获取 CollectionBase 实例中包含的元素数量。 |
| [group(Shape[] groupItems)](#group-com.aspose.cells.Shape---) | 对形状进行分组。 |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | 确定 CollectionBase 实例中特定项的索引。 |
| [iterator()](#iterator--) | 返回遍历 CollectionBase 实例的枚举器。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Shape shape)](#remove-com.aspose.cells.Shape-) | 移除形状。 |
| [removeAt(int index)](#removeAt-int-) | 移除形状。 |
| [toString()](#toString--) |  |
| [ungroup(GroupShape group)](#ungroup-com.aspose.cells.GroupShape-) | 取消形状项的分组。 |
| [updateSelectedValue()](#updateSelectedValue--) | 通过链接单元格或形状范围的值更新所选值。 |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


向 CollectionBase 实例添加一个项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| o | java.lang.Object | 要添加到 CollectionBase 实例的对象。 |

**Returns:**
int - 新元素插入的位置。
### addActiveXControl(int type, int topRow, int top, int leftColumn, int left, int width, int height) {#addActiveXControl-int-int-int-int-int-int-int-}
```
public Shape addActiveXControl(int type, int topRow, int top, int leftColumn, int left, int width, int height)
```


创建一个 Activex 控件。

**Example**

```
         //add an ActiveX control
         Shape activeXControl = shapes.addActiveXControl(com.aspose.cells.ControlType.CHECK_BOX, 1, 0, 1, 0, 100, 50);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [ControlType](../../com.aspose.cells/controltype)。控件的类型。 |
| topRow | int | 左上行索引。 |
| 顶部 | int | 表示 Shape 相对于其左侧行的垂直偏移量，单位为像素。 |
| leftColumn | int | 左上列索引。 |
| 左侧 | int | 表示 Shape 相对于其左侧列的水平偏移量，单位为像素。 |
| 宽度 | int | 表示 Shape 的宽度，单位为像素。 |
| 高度 | int | 表示 Shape 的高度，单位为像素。 |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### addArc(int topRow, int top, int leftColumn, int left, int height, int width) {#addArc-int-int-int-int-int-int-}
```
public ArcShape addArc(int topRow, int top, int leftColumn, int left, int height, int width)
```


向工作表添加一个 ArcShape。

**Example**

```
         //add a arc
         ArcShape arcShape = shapes.addArc(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | int | 左上行索引。 |
| 顶部 | int | 表示 ArcShape 相对于其左侧行的垂直偏移量，单位为像素。 |
| leftColumn | int | 左上列索引。 |
| 左侧 | int | 表示 ArcShape 相对于其左列的水平偏移，单位为像素。 |
| 高度 | int | 表示 ArcShape 的高度，单位为像素。 |
| 宽度 | int | 表示 ArcShape 的宽度，单位为像素。 |

**Returns:**
[ArcShape](../../com.aspose.cells/arcshape) - A ArcShape object.
### addAutoShape(int type, int topRow, int top, int leftColumn, int left, int height, int width) {#addAutoShape-int-int-int-int-int-int-int-}
```
public Shape addAutoShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)
```


向工作表添加一个 AutoShape。

**Remarks**

类型不能是 Chart/Comment/Picture/OleObject/Polygon/DialogBox。

**Example**

```
         //Adds a AutoShape to the worksheet.
         Shape autoShape = shapes.addAutoShape(AutoShapeType.CUBE, 1, 0, 1, 0, 100, 50);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [AutoShapeType](../../com.aspose.cells/autoshapetype)。自动形状类型。 |
| topRow | int | 左上行索引。 |
| 顶部 | int | 表示 Shape 相对于其左侧行的垂直偏移量，单位为像素。 |
| leftColumn | int | 左上列索引。 |
| 左侧 | int | 表示 Shape 相对于其左侧列的水平偏移量，单位为像素。 |
| 高度 | int | 表示 Shape 的高度，单位为像素。 |
| 宽度 | int | 表示 Shape 的宽度，单位为像素。 |

**Returns:**
[Shape](../../com.aspose.cells/shape) - A Shape object.
### addAutoShapeInChart(int type, int top, int left, int height, int width) {#addAutoShapeInChart-int-int-int-int-int-}
```
public Shape addAutoShapeInChart(int type, int top, int left, int height, int width)
```


向图表添加一个 AutoShape。

**Remarks**

类型不能是 Chart/Comment/Picture/OleObject/Polygon/DialogBox。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [AutoShapeType](../../com.aspose.cells/autoshapetype)。自动形状类型。 |
| 顶部 | int | 表示 文本框 相对于图表区域左上角的垂直偏移，单位为图表区域的 1/4000。 |
| 左侧 | int | 表示 文本框 相对于图表区域左上角的垂直偏移，单位为图表区域的 1/4000。 |
| 高度 | int | 表示 文本框 的高度，单位为图表区域的 1/4000。 |
| 宽度 | int | 表示 文本框 的宽度，单位为图表区域的 1/4000。 |

**Returns:**
[Shape](../../com.aspose.cells/shape) - Returns a shape object.
### addButton(int topRow, int top, int leftColumn, int left, int height, int width) {#addButton-int-int-int-int-int-int-}
```
public Button addButton(int topRow, int top, int leftColumn, int left, int height, int width)
```


向工作表添加一个 Button。

**Example**

```
         //add a button
         Button button = shapes.addButton(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | int | 左上行索引。 |
| 顶部 | int | 表示 Button 相对于其左行的垂直偏移，单位为像素。 |
| leftColumn | int | 左上列索引。 |
| 左侧 | int | 表示 Button 相对于其左列的水平偏移，单位为像素。 |
| 高度 | int | 表示 Button 的高度，单位为像素。 |
| 宽度 | int | 表示 Button 的宽度，单位为像素。 |

**Returns:**
[Button](../../com.aspose.cells/button) - A Button object.
### addCheckBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addCheckBox-int-int-int-int-int-int-}
```
public CheckBox addCheckBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


向工作表添加一个复选框。

**Example**

```
         //add a CheckBox
         CheckBox checkBox = shapes.addCheckBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | int | 左上行索引。 |
| 顶部 | int | 表示 复选框 相对于其顶部行的垂直偏移，单位为像素。 |
| leftColumn | int | 左上列索引。 |
| 左侧 | int | 表示 文本框 相对于其左列的水平偏移，单位为像素。 |
| 高度 | int | 文本框的高度，单位为像素。 |
| 宽度 | int | 文本框的宽度，单位为像素。 |

**Returns:**
[CheckBox](../../com.aspose.cells/checkbox) - The new CheckBox object index.
### addComboBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addComboBox-int-int-int-int-int-int-}
```
public ComboBox addComboBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


向工作表添加一个 ComboBox。

**Example**

```
         //add a combo box
         ComboBox comboBox = shapes.addComboBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | int | 左上行索引。 |
| 顶部 | int | 表示 ComboBox 相对于其左行的垂直偏移，单位为像素。 |
| leftColumn | int | 左上列索引。 |
| 左侧 | int | 表示 ComboBox 相对于其左列的水平偏移，单位为像素。 |
| 高度 | int | 表示 ComboBox 的高度，单位为像素。 |
| 宽度 | int | 表示 ComboBox 的宽度，单位为像素。 |

**Returns:**
[ComboBox](../../com.aspose.cells/combobox) - A ComboBox object.
### addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left) {#addCopy-com.aspose.cells.Shape-int-int-int-int-}
```
public Shape addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left)
```


向工作表添加并复制一个形状。

**Example**

```
         //add a shape
         RectangleShape rectangle = shapes.addRectangle(2, 0, 2, 0, 130, 130);
         //Adds and copies a shape.
         shapes.addCopy(rectangle, 7, 0, 7, 0);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceShape | [Shape](../../com.aspose.cells/shape) | 源形状。 |
| topRow | int | 顶部行索引。 |
| 顶部 | int | 表示 相对于其顶部行的垂直偏移，单位为像素。 |
| leftColumn | int | 左列索引。 |
| 左侧 | int | 表示 相对于其左列的水平偏移，单位为像素。 |

**Returns:**
[Shape](../../com.aspose.cells/shape) - The new [Shape](../../com.aspose.cells/shape) object.
### addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left, CopyOptions copyOptions) {#addCopy-com.aspose.cells.Shape-int-int-int-int-com.aspose.cells.CopyOptions-}
```
public Shape addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left, CopyOptions copyOptions)
```


向工作表添加并复制一个形状。

**Example**

```
         //add a shape
         RectangleShape rectangle = shapes.addRectangle(2, 0, 2, 0, 130, 130);
         //Adds and copies a shape.
         shapes.addCopy(rectangle, 7, 0, 7, 0);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceShape | [Shape](../../com.aspose.cells/shape) | 源形状。 |
| topRow | int | 顶部行索引。 |
| 顶部 | int | 表示 相对于其顶部行的垂直偏移，单位为像素。 |
| leftColumn | int | 左列索引。 |
| 左侧 | int | 表示 相对于其左列的水平偏移，单位为像素。 |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | 复制形状的选项。 |

**Returns:**
[Shape](../../com.aspose.cells/shape) - The new [Shape](../../com.aspose.cells/shape) object.
### addEquation(int topRow, int top, int leftColumn, int left, int height, int width) {#addEquation-int-int-int-int-int-int-}
```
public TextBox addEquation(int topRow, int top, int leftColumn, int left, int height, int width)
```


向工作表添加一个公式对象。

**Example**

```
         // Adds an equation object to the worksheet.
         TextBox textBox = shapes.addEquation(1, 0, 1, 0, 100, 300);
 
         // Gets the starting node of the equation object
         EquationNode mathNode = textBox.getEquationParagraph().getChild(0);
 
         // Inserts a fractional equation.
         FractionEquationNode node = (FractionEquationNode)mathNode.addChild(EquationNodeType.FRACTION);
         node.setFractionType(EquationFractionType.SKEWED);
 
         String str1 = "A";
         EquationComponentNode numerator = (EquationComponentNode)node.addChild(EquationNodeType.NUMERATOR);
         TextRunEquationNode TR = (TextRunEquationNode)(numerator.addChild(EquationNodeType.TEXT));
         TR.setText(str1);
 
         String str2 = "B";
         EquationComponentNode denominator = (EquationComponentNode)node.addChild(EquationNodeType.DENOMINATOR);
         TR = (TextRunEquationNode) (denominator.addChild(EquationNodeType.TEXT));
         TR.setText(str2);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | int | 顶部行索引。 |
| 顶部 | int | 其顶部行的垂直偏移，以像素为单位。 |
| leftColumn | int | 左列索引。 |
| 左侧 | int | 其左侧列的水平偏移，以像素为单位。 |
| 高度 | int | 公式的高度，以像素为单位。 |
| 宽度 | int | 公式的宽度，以像素为单位。 |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - 
### addFreeFloatingShape(int type, int top, int left, int height, int width, byte[] imageData, boolean isOriginalSize) {#addFreeFloatingShape-int-int-int-int-int-byte---boolean-}
```
public Shape addFreeFloatingShape(int type, int top, int left, int height, int width, byte[] imageData, boolean isOriginalSize)
```


向工作表添加一个自由浮动形状。仅适用于线条/图像形状。

**Example**

```
         //add a line
         Shape floatingShape_Line = shapes.addFreeFloatingShape(MsoDrawingType.LINE, 100, 100, 100, 50, null, false);
         //add a picture
         byte[] imageData = null;
         FileInputStream fs = new FileInputStream("image.jpg");
         try //JAVA: was using
         {
             int len = (int)fs.available();
             imageData = new byte[len];
             fs.read(imageData, 0, len);
         }
         finally { if (fs != null) fs.close(); }
         Shape floatingShape_Picture = shapes.addFreeFloatingShape(MsoDrawingType.PICTURE, 200, 100, 100, 50, imageData, false);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). 形状类型。 |
| 顶部 | int | 表示形状相对于工作表顶部行的垂直偏移，以像素为单位。 |
| 左侧 | int | 表示形状相对于工作表左侧列的水平偏移，以像素为单位。 |
| 高度 | int | 表示 LineShape 的高度，以像素为单位。 |
| 宽度 | int | 表示 LineShape 的宽度，以像素为单位。 |
| imageData | byte[] | 图像数据，仅适用于图片。 |
| isOriginalSize | boolean | 如果形状是图像，是否使用原始大小。 |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### addFreeform(int topRow, int top, int leftColumn, int left, int height, int width, ShapePath[] paths) {#addFreeform-int-int-int-int-int-int-com.aspose.cells.ShapePath---}
```
public Shape addFreeform(int topRow, int top, int leftColumn, int left, int height, int width, ShapePath[] paths)
```


向工作表添加一个自由形状。

**Remarks**

注意：参数中的宽度和高度可以是任意正整数，而不是由 \\u9225\\u6a96aths 指定的 ShapePath 数组的总宽度和高度。它们之间的关系是比例填充关系，即每个 ShapePath 对象将根据宽度和高度进行缩放。因此，当 'paths' 中有多个对象时，需要合理设计每个 ShapePath 对象以满足预期。当只有一个 ShapePath 对象且没有其他要求时，将对象的宽度和高度作为参数值传入 \\u9225\\u5b27\\u20ac\\u5a94s 是一个好的解决方案。

**Example**

```
         //Custom figure
         ShapePath shapePath = new ShapePath();
         shapePath.moveTo(60, 45);
         shapePath.arcTo(25, 25, 0, 270);
         shapePath.close();
 
         shapePath.moveTo(60, 20);
         shapePath.lineTo(110, 70);
         shapePath.lineTo(125, 155.5f);
         shapePath.arcTo(35.5f, 35.5f, 0, 270);
         shapePath.close();
 
         shapePath.moveTo(150, 45);
         shapePath.arcTo(25, 25, 0, 270);
 
         int shapePathW = shapePath.getWidthPixel();
         int shapePathH = shapePath.getHeightPixel();
 
         ShapePath shapePath1 = new ShapePath();
         shapePath1.moveTo(0, 0);
         shapePath1.cubicBezierTo(48.24997f, 0.6844f,
                             96.5f, -7.148871f,
                             130, 11.517795f);
         shapePath1.cubicBezierTo(163.5f, 30.18446f,
                             182.24997f, 75.351f,
                             201, 120.517795f);
         shapePath1.moveTo(150, 80);
         shapePath1.arcTo(25, 25, 0, 270);
 
         if (shapePath1.getWidthPixel() > shapePathW)
             {
         shapePathW = shapePath1.getWidthPixel();
         }
 
         if (shapePath1.getHeightPixel() > shapePathH)
         {
         shapePathH = shapePath1.getHeightPixel();
         }
 
         //Notice: shapePathH and shapePathH can be any positive integer values, here we just simply set them.
 
         //Insert custom figure into worksheet
         shapes.addFreeform(1, 0, 1, 0, shapePathH, shapePathW, new ShapePath[] { shapePath, shapePath1});
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | int | 左上行索引。 |
| 顶部 | int | 表示自由形状相对于其左侧行的垂直偏移，以像素为单位。 |
| leftColumn | int | 左上列索引。 |
| 左侧 | int | 表示自由形状相对于其左侧列的水平偏移，以像素为单位。 |
| 高度 | int | 表示自由形状的高度，以像素为单位。 |
| 宽度 | int | 表示自由形状的宽度，以像素为单位。 |
| paths | [ShapePath\[\]](../../com.aspose.cells/shapepath) | 表示用户定义的路径 |

**Returns:**
[Shape](../../com.aspose.cells/shape) - A freeform shape.
### addGroupBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addGroupBox-int-int-int-int-int-int-}
```
public GroupBox addGroupBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


向工作表添加一个 GroupBox。

**Example**

```
         //add a group box
         GroupBox groupBox = shapes.addGroupBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | int | 左上行索引。 |
| 顶部 | int | 表示 GroupBox 相对于其左侧行的垂直偏移，以像素为单位。 |
| leftColumn | int | 左上列索引。 |
| 左侧 | int | 表示 GroupBox 相对于其左侧列的水平偏移，以像素为单位。 |
| 高度 | int | 表示 GroupBox 的高度，以像素为单位。 |
| 宽度 | int | 表示 GroupBox 的宽度，以像素为单位。 |

**Returns:**
[GroupBox](../../com.aspose.cells/groupbox) - A GroupBox object.
### addIcons(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageByteData, byte[] compatibleImageData) {#addIcons-int-int-int-int-int-int-byte---byte---}
```
public Picture addIcons(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageByteData, byte[] compatibleImageData)
```


添加 svg 图像。

**Example**

```
         //add icon
         FileInputStream fs = new FileInputStream("icon.svg");
         try //JAVA: was using
         {
             int len = (int)fs.available();
             byte[] imageData = new byte[len];
             fs.read(imageData, 0, len);
             Picture picture = shapes.addIcons(4, 0, 5, 0, -1, -1, imageData, null);
         }
         finally { if (fs != null) fs.close(); }
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | int | 左上行索引。 |
| 顶部 | int | 表示形状相对于其左侧行的垂直偏移，以像素为单位。 |
| leftColumn | int | 左上列索引。 |
| 左侧 | int | 形状相对于其左侧列的水平偏移，以像素为单位。 |
| 高度 | int | 形状的高度，以像素为单位。 |
| 宽度 | int | 形状的宽度，以像素为单位。 |
| imageByteData | byte[] | 图像字节数据。 |
| compatibleImageData | byte[] | 从 SVG 转换的图像数据，以兼容 Excel 2016 或更低版本。 |

**Returns:**
[Picture](../../com.aspose.cells/picture) - 
### addLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, int width, String latex) {#addLaTeXEquation-int-int-int-int-int-int-java.lang.String-}
```
public TextBox addLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, int width, String latex)
```


使用 LaTeX 格式字符串向工作表添加一个公式对象。

**Example**

```
         // LaTeX format string.
         String latex = "\\alpha +  \\frac{\\partial^2}{\\partial x_1\\partial x_2}y - \\left ( a + b \\right )+_{a}^{b}\\beta";
         // Adds an equation object to the worksheet.
         TextBox textBox = shapes.addLaTeXEquation(1, 0, 1, 0, 100, 300, latex);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | int | 顶部行索引。 |
| 顶部 | int | 其顶部行的垂直偏移，以像素为单位。 |
| leftColumn | int | 左列索引。 |
| 左侧 | int | 其左侧列的水平偏移，以像素为单位。 |
| 高度 | int | 公式的高度，以像素为单位。 |
| 宽度 | int | 公式的宽度，以像素为单位。 |
| latex | java.lang.String | LaTeX 格式字符串 |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - 
### addLabel(int topRow, int top, int leftColumn, int left, int height, int width) {#addLabel-int-int-int-int-int-int-}
```
public Label addLabel(int topRow, int top, int leftColumn, int left, int height, int width)
```


向工作表添加一个标签。

**Example**

```
         //add a label
         Label label = shapes.addLabel(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | int | 左上行索引。 |
| 顶部 | int | 表示 Label 相对于其左侧行的垂直偏移，以像素为单位。 |
| leftColumn | int | 左上列索引。 |
| 左侧 | int | 表示 Label 相对于其左侧列的水平偏移，以像素为单位。 |
| 高度 | int | 表示 Label 的高度，以像素为单位。 |
| 宽度 | int | 表示 Label 的宽度，以像素为单位。 |

**Returns:**
[Label](../../com.aspose.cells/label) - A Label object.
### addLabelInChart(int top, int left, int height, int width) {#addLabelInChart-int-int-int-int-}
```
public Label addLabelInChart(int top, int left, int height, int width)
```


向图表添加一个标签。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 顶部 | int | 表示标签相对于左上角的垂直偏移，单位为图表区域的 1/4000。 |
| 左侧 | int | 表示标签相对于左上角的垂直偏移，单位为图表区域的 1/4000。 |
| 高度 | int | 表示标签的高度，单位为图表区域的 1/4000。 |
| 宽度 | int | 表示标签的宽度，单位为图表区域的 1/4000。 |

**Returns:**
[Label](../../com.aspose.cells/label) - A new Label object.
### addLine(int topRow, int top, int leftColumn, int left, int height, int width) {#addLine-int-int-int-int-int-int-}
```
public LineShape addLine(int topRow, int top, int leftColumn, int left, int height, int width)
```


向工作表添加一个线形状。

**Example**

```
         // add a line object
         LineShape lineShape = shapes.addLine(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | int | 左上行索引。 |
| 顶部 | int | 表示 LineShape 相对于其左侧行的垂直偏移，以像素为单位。 |
| leftColumn | int | 左上列索引。 |
| 左侧 | int | 表示 LineShape 相对于其左侧列的水平偏移，以像素为单位。 |
| 高度 | int | 表示 LineShape 的高度，以像素为单位。 |
| 宽度 | int | 表示 LineShape 的宽度，以像素为单位。 |

**Returns:**
[LineShape](../../com.aspose.cells/lineshape) - A LineShape object.
### addLinkedPicture(int topRow, int leftColumn, int height, int width, String sourceFullName) {#addLinkedPicture-int-int-int-int-java.lang.String-}
```
public Picture addLinkedPicture(int topRow, int leftColumn, int height, int width, String sourceFullName)
```


添加一个链接图片。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | int | 左上行索引。 |
| leftColumn | int | 左上列索引。 |
| 高度 | int | 形状的高度。以像素为单位 |
| 宽度 | int | 形状的宽度。以像素为单位 |
| sourceFullName | java.lang.String | 链接图像的源文件路径和名称 |

**Returns:**
[Picture](../../com.aspose.cells/picture) - [Picture](../../com.aspose.cells/picture) Picture object.
### addListBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addListBox-int-int-int-int-int-int-}
```
public ListBox addListBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


向工作表添加一个 ListBox。

**Example**

```
         //add a list box
         ListBox listBox = shapes.addListBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | int | 左上行索引。 |
| 顶部 | int | 表示 ListBox 相对于其左侧行的垂直偏移，以像素为单位。 |
| leftColumn | int | 左上列索引。 |
| 左侧 | int | 表示 ListBox 相对于其左侧列的水平偏移，以像素为单位。 |
| 高度 | int | 表示 ListBox 的高度，以像素为单位。 |
| 宽度 | int | 表示 ListBox 的宽度，以像素为单位。 |

**Returns:**
[ListBox](../../com.aspose.cells/listbox) - A ListBox object.
### addOleObject(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageData) {#addOleObject-int-int-int-int-int-int-byte---}
```
public OleObject addOleObject(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageData)
```


添加一个 OleObject。

**Example**

```
         FileInputStream fs = new FileInputStream("image.jpg");
         try //JAVA: was using
         {
             int len = (int)fs.available();
             byte[] imageData = new byte[len];
             fs.read(imageData, 0, len);
             OleObject oleObject = shapes.addOleObject(4, 0, 5, 0, 300, 500, imageData);
         }
         finally { if (fs != null) fs.close(); }
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | int |  |
| 顶部 | int |  |
| leftColumn | int |  |
| 左侧 | int |  |
| 高度 | int |  |
| 宽度 | int |  |
| imageData | byte[] |  |

**Returns:**
[OleObject](../../com.aspose.cells/oleobject) - 
### addOleObjectWithLinkedImage(int topRow, int leftColumn, int height, int width, String sourceFullName) {#addOleObjectWithLinkedImage-int-int-int-int-java.lang.String-}
```
public OleObject addOleObjectWithLinkedImage(int topRow, int leftColumn, int height, int width, String sourceFullName)
```


添加一个链接图片。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | int | 左上行索引。 |
| leftColumn | int | 左上列索引。 |
| 高度 | int | 形状的高度。以像素为单位 |
| 宽度 | int | 形状的宽度。以像素为单位 |
| sourceFullName | java.lang.String | 链接图像的源文件路径和名称 |

**Returns:**
[OleObject](../../com.aspose.cells/oleobject) - [Picture](../../com.aspose.cells/picture) Picture object.
### addOval(int topRow, int top, int leftColumn, int left, int height, int width) {#addOval-int-int-int-int-int-int-}
```
public Oval addOval(int topRow, int top, int leftColumn, int left, int height, int width)
```


向工作表添加一个椭圆。

**Example**

```
         //add a oval
         Oval oval = shapes.addOval(1, 0, 1, 0, 50, 50);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | int | 左上行索引。 |
| 顶部 | int | 表示 Oval 从其左侧行的垂直偏移，单位为像素。 |
| leftColumn | int | 左上列索引。 |
| 左侧 | int | 表示 Oval 从其左侧列的水平偏移，单位为像素。 |
| 高度 | int | 表示 Oval 的高度，单位为像素。 |
| 宽度 | int | 表示 Oval 的宽度，单位为像素。 |

**Returns:**
[Oval](../../com.aspose.cells/oval) - A Oval object.
### addPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream) {#addPicture-int-int-int-int-java.io.InputStream-}
```
public Picture addPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream)
```


向集合中添加一张图片。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | int | 左上行索引。 |
| leftColumn | int | 左上列索引。 |
| bottomRow | int | 右下行索引 |
| rightColumn | int | 右下列索引 |
| stream | java.io.InputStream | 包含图像数据的流对象。 |

**Returns:**
[Picture](../../com.aspose.cells/picture) - [Picture](../../com.aspose.cells/picture) Picture object.
### addPicture(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale) {#addPicture-int-int-java.io.InputStream-int-int-}
```
public Picture addPicture(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale)
```


向集合中添加一张图片。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | int | 左上行索引。 |
| leftColumn | int | 左上列索引。 |
| stream | java.io.InputStream | 包含图像数据的流对象。 |
| widthScale | int | 图像宽度的比例，百分比。 |
| heightScale | int | 图像高度的比例，百分比。 |

**Returns:**
[Picture](../../com.aspose.cells/picture) - [Picture](../../com.aspose.cells/picture) Picture object.
### addPictureInChart(int top, int left, InputStream stream, int widthScale, int heightScale) {#addPictureInChart-int-int-java.io.InputStream-int-int-}
```
public Picture addPictureInChart(int top, int left, InputStream stream, int widthScale, int heightScale)
```


向图表中添加一张图片。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 顶部 | int | 表示形状相对于图表区域左上角的垂直偏移，单位为图表区域的 1/4000。 |
| 左侧 | int | 表示形状相对于图表区域左上角的水平偏移，单位为图表区域的 1/4000。 |
| stream | java.io.InputStream | 包含图像数据的流对象。 |
| widthScale | int | 图像宽度的比例，百分比。 |
| heightScale | int | 图像高度的比例，百分比。 |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns a Picture object.
### addRadioButton(int topRow, int top, int leftColumn, int left, int height, int width) {#addRadioButton-int-int-int-int-int-int-}
```
public RadioButton addRadioButton(int topRow, int top, int leftColumn, int left, int height, int width)
```


向工作表添加一个 RadioButton。

**Example**

```
         //add a radio button
         RadioButton radioButton = shapes.addRadioButton(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | int | 左上行索引。 |
| 顶部 | int | 表示 RadioButton 从其左侧行的垂直偏移，单位为像素。 |
| leftColumn | int | 左上列索引。 |
| 左侧 | int | 表示 RadioButton 从其左侧列的水平偏移，单位为像素。 |
| 高度 | int | 表示 RadioButton 的高度，单位为像素。 |
| 宽度 | int | 表示 RadioButton 的宽度，单位为像素。 |

**Returns:**
[RadioButton](../../com.aspose.cells/radiobutton) - A RadioButton object.
### addRectangle(int topRow, int top, int leftColumn, int left, int height, int width) {#addRectangle-int-int-int-int-int-int-}
```
public RectangleShape addRectangle(int topRow, int top, int leftColumn, int left, int height, int width)
```


向工作表添加一个矩形形状。

**Example**

```
         // add a rectangle
         RectangleShape rectangleShape = shapes.addRectangle(2, 0, 2, 0, 130, 130);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | int | 左上行索引。 |
| 顶部 | int | 表示 RectangleShape 从其左侧行的垂直偏移，单位为像素。 |
| leftColumn | int | 左上列索引。 |
| 左侧 | int | 表示 RectangleShape 从其左侧列的水平偏移，单位为像素。 |
| 高度 | int | 表示 RectangleShape 的高度，单位为像素。 |
| 宽度 | int | 表示 RectangleShape 的宽度，单位为像素。 |

**Returns:**
[RectangleShape](../../com.aspose.cells/rectangleshape) - A RectangleShape object.
### addScrollBar(int topRow, int top, int leftColumn, int left, int height, int width) {#addScrollBar-int-int-int-int-int-int-}
```
public ScrollBar addScrollBar(int topRow, int top, int leftColumn, int left, int height, int width)
```


向工作表添加一个滚动条。

**Example**

```
         //add a scroll bar
         ScrollBar scrollBar = shapes.addScrollBar(1, 0, 1, 0, 100, 20);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | int | 左上行索引。 |
| 顶部 | int | 表示 ScrollBar 从其左侧行的垂直偏移，单位为像素。 |
| leftColumn | int | 左上列索引。 |
| 左侧 | int | 表示 ScrollBar 从其左侧列的水平偏移，单位为像素。 |
| 高度 | int | 表示 ScrollBar 的高度，单位为像素。 |
| 宽度 | int | 表示 ScrollBar 的宽度，单位为像素。 |

**Returns:**
[ScrollBar](../../com.aspose.cells/scrollbar) - A ScrollBar object.
### addShape(int type, int topRow, int top, int leftColumn, int left, int height, int width) {#addShape-int-int-int-int-int-int-int-}
```
public Shape addShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)
```


向工作表添加一个形状。

**Remarks**

类型不能是 Chart/Comment/Picture/OleObject/Polygon/DialogBox。

**Example**

```
         //Add a shape of the specified type
         Shape shapeByType = shapes.addShape(MsoDrawingType.CELLS_DRAWING, 1, 0, 1, 0, 100, 50);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Mso 绘图类型。 |
| topRow | int | 左上行索引。 |
| 顶部 | int | 表示 Shape 相对于其左侧行的垂直偏移量，单位为像素。 |
| leftColumn | int | 左上列索引。 |
| 左侧 | int | 表示 Shape 相对于其左侧列的水平偏移量，单位为像素。 |
| 高度 | int | 表示 Shape 的高度，单位为像素。 |
| 宽度 | int | 表示 Shape 的宽度，单位为像素。 |

**Returns:**
[Shape](../../com.aspose.cells/shape) - A Shape object.
### addShapeInChart(int type, int placement, int left, int top, int right, int bottom) {#addShapeInChart-int-int-int-int-int-int-}
```
public Shape addShapeInChart(int type, int placement, int left, int top, int right, int bottom)
```


向图表添加形状。所有单位为图表区域的 1/4000。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype)。绘图类型。 |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype)。放置类型。 |
| 左侧 | int | 以图表区域宽度的 1/4000 为单位。 |
| 顶部 | int | 以图表区域高度的 1/4000 为单位。 |
| 右 | int | 以图表区域宽度的 1/4000 为单位。 |
| 底部 | int | 以图表区域高度的 1/4000 为单位。 |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addShapeInChart(int type, int placement, int left, int top, int right, int bottom, byte[] imageData) {#addShapeInChart-int-int-int-int-int-int-byte---}
```
public Shape addShapeInChart(int type, int placement, int left, int top, int right, int bottom, byte[] imageData)
```


向图表添加形状。所有单位为图表区域的 1/4000。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype)。绘图类型。 |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype)。放置类型。 |
| 左侧 | int | 以图表区域宽度的 1/4000 为单位。 |
| 顶部 | int | 以图表区域高度的 1/4000 为单位。 |
| 右 | int | 以图表区域宽度的 1/4000 为单位。 |
| 底部 | int | 以图表区域高度的 1/4000 为单位。 |
| imageData | byte[] | 如果形状不是图片或 ole 对象，imageData 应为 null。 |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom) {#addShapeInChartByScale-int-int-double-double-double-double-}
```
public Shape addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom)
```


向图表添加形状。所有单位是图表区域的百分比比例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype)。绘图类型。 |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype)。放置类型。 |
| 左侧 | double | 单位是图表区域宽度的百分比比例。 |
| 顶部 | double | 单位是图表区域高度的百分比比例。 |
| 右 | double | 单位是图表区域宽度的百分比比例。 |
| 底部 | double | 单位是图表区域高度的百分比比例。 |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom, byte[] imageData) {#addShapeInChartByScale-int-int-double-double-double-double-byte---}
```
public Shape addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom, byte[] imageData)
```


向图表添加形状。所有单位为图表区域的 1/4000。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype)。绘图类型。 |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype)。放置类型。 |
| 左侧 | double | 单位是图表区域宽度的百分比比例。 |
| 顶部 | double | 单位是图表区域高度的百分比比例。 |
| 右 | double | 单位是图表区域宽度的百分比比例。 |
| 底部 | double | 单位是图表区域高度的百分比比例。 |
| imageData | byte[] | 如果形状不是图片或 ole 对象，imageData 应为 null。 |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addSignatureLine(int topRow, int leftColumn, SignatureLine signatureLine) {#addSignatureLine-int-int-com.aspose.cells.SignatureLine-}
```
public Picture addSignatureLine(int topRow, int leftColumn, SignatureLine signatureLine)
```


向工作表添加一个签名线。

**Example**

```
         SignatureLine wSignatureLine = new SignatureLine();
         wSignatureLine.setAllowComments(true);
         wSignatureLine.setEmail("example@example.com");
         wSignatureLine.setInstructions("Sign to confirm the excel content.");
         wSignatureLine.setLine(true);
         wSignatureLine.setShowSignedDate(true);
         wSignatureLine.setSigner("User");
         wSignatureLine.setTitle("tester");
         //wSignatureLine.SignatureLineType = SignatureType.Stamp;
         Picture signatureLine1 = shapes.addSignatureLine(0, 0, wSignatureLine);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | int | 左上行索引。 |
| leftColumn | int | 左上列索引。 |
| signatureLine | [SignatureLine](../../com.aspose.cells/signatureline) | 表示签名线对象。 |

**Returns:**
[Picture](../../com.aspose.cells/picture) - 
### addSpinner(int topRow, int top, int leftColumn, int left, int height, int width) {#addSpinner-int-int-int-int-int-int-}
```
public Spinner addSpinner(int topRow, int top, int leftColumn, int left, int height, int width)
```


向工作表添加一个微调框。

**Example**

```
         //add a spinner
         Spinner spinner = shapes.addSpinner(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | int | 左上行索引。 |
| 顶部 | int | 表示 Spinner 相对于其左侧行的垂直偏移量，单位为像素。 |
| leftColumn | int | 左上列索引。 |
| 左侧 | int | 表示 Spinner 相对于其左侧列的水平偏移量，单位为像素。 |
| 高度 | int | 表示 Spinner 的高度，单位为像素。 |
| 宽度 | int | 表示 Spinner 的宽度，单位为像素。 |

**Returns:**
[Spinner](../../com.aspose.cells/spinner) - A Spinner object.
### addSvg(int topRow, int top, int leftColumn, int left, int height, int width, byte[] svgData, byte[] compatibleImageData) {#addSvg-int-int-int-int-int-int-byte---byte---}
```
public Picture addSvg(int topRow, int top, int leftColumn, int left, int height, int width, byte[] svgData, byte[] compatibleImageData)
```


添加 svg 图像。

**Example**

```
         // add a svg
         FileInputStream fs = new FileInputStream("image.svg");
         try //JAVA: was using
         {
             int len = (int)fs.available();
             byte[] imageData = new byte[len];
             fs.read(imageData, 0, len);
             Picture picture = shapes.addSvg(4, 0, 5, 0, -1, -1, imageData, null);
         }
         finally { if (fs != null) fs.close(); }
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | int | 左上行索引。 |
| 顶部 | int | 表示形状相对于其左侧行的垂直偏移，以像素为单位。 |
| leftColumn | int | 左上列索引。 |
| 左侧 | int | 形状相对于其左侧列的水平偏移，以像素为单位。 |
| 高度 | int | 形状的高度，以像素为单位。 |
| 宽度 | int | 形状的宽度，以像素为单位。 |
| svgData | byte[] | svg 图像数据。 |
| compatibleImageData | byte[] | 从 SVG 转换的图像数据，以兼容 Excel 2016 或更低版本。 |

**Returns:**
[Picture](../../com.aspose.cells/picture) - 
### addTextBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addTextBox-int-int-int-int-int-int-}
```
public TextBox addTextBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


向工作表添加文本框。

**Example**

```
         //add a TextBox
         TextBox textBox = shapes.addTextBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | int | 左上行索引。 |
| 顶部 | int | 表示文本框相对于其顶部行的垂直偏移量，单位为像素。 |
| leftColumn | int | 左上列索引。 |
| 左侧 | int | 表示 文本框 相对于其左列的水平偏移，单位为像素。 |
| 高度 | int | 表示文本框的高度，单位为像素。 |
| 宽度 | int | 表示文本框的宽度，单位为像素。 |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - A [TextBox](../../com.aspose.cells/textbox) object.
### addTextBoxInChart(int top, int left, int height, int width) {#addTextBoxInChart-int-int-int-int-}
```
public TextBox addTextBoxInChart(int top, int left, int height, int width)
```


向图表添加文本框。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 顶部 | int | 表示 文本框 相对于图表区域左上角的垂直偏移，单位为图表区域的 1/4000。 |
| 左侧 | int | 表示 文本框 相对于图表区域左上角的垂直偏移，单位为图表区域的 1/4000。 |
| 高度 | int | 表示 文本框 的高度，单位为图表区域的 1/4000。 |
| 宽度 | int | 表示 文本框 的宽度，单位为图表区域的 1/4000。 |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - A TextBox object.
### addTextEffect(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int topRow, int top, int leftColumn, int left, int height, int width) {#addTextEffect-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-int-int-}
```
public Shape addTextEffect(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int topRow, int top, int leftColumn, int left, int height, int width)
```


插入 WordArt 对象。

**Example**

```
         //add a WordArt
         Shape wordArt1 = shapes.addTextEffect(MsoPresetTextEffect.TEXT_EFFECT_10, "WordArt", "arial", 18, false, false, 3, 0, 3, 0, 200, 50);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| effect | int | [MsoPresetTextEffect](../../com.aspose.cells/msopresettexteffect)。mso 预设文本效果类型。 |
| 文本 | java.lang.String | WordArt 文本。 |
| fontName | java.lang.String | 字体名称。 |
| 大小 | int | 字体大小 |
| fontBold | boolean | 指示字体是否为粗体。 |
| fontItalic | boolean | 指示字体是否为斜体。 |
| topRow | int | 左上行索引。 |
| 顶部 | int | 表示形状相对于其左侧行的垂直偏移，以像素为单位。 |
| leftColumn | int | 左上列索引。 |
| 左侧 | int | 表示形状相对于左列的水平偏移量，单位为像素。 |
| 高度 | int | 表示形状的高度，单位为像素。 |
| 宽度 | int | 表示形状的宽度，单位为像素。 |

**Returns:**
[Shape](../../com.aspose.cells/shape) - Returns a Shape object that represents the new WordArt object.
### addTextEffectInChart(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int top, int left, int height, int width) {#addTextEffectInChart-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-}
```
public Shape addTextEffectInChart(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int top, int left, int height, int width)
```


向图表插入 WordArt 对象

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| effect | int | [MsoPresetTextEffect](../../com.aspose.cells/msopresettexteffect)。mso 预设文本效果类型。 |
| 文本 | java.lang.String | WordArt 文本。 |
| fontName | java.lang.String | 字体名称。 |
| 大小 | int | 字体大小 |
| fontBold | boolean | 指示字体是否为粗体。 |
| fontItalic | boolean | 指示字体是否为斜体。 |
| 顶部 | int | 表示形状相对于图表区域左上角的垂直偏移，单位为图表区域的 1/4000。 |
| 左侧 | int | 表示形状相对于图表区域左上角的垂直偏移，单位为图表区域的 1/4000。 |
| 高度 | int | 表示形状的高度，单位为图表区域的 1/4000。 |
| 宽度 | int | 表示形状的宽度，单位为图表区域的 1/4000。 |

**Returns:**
[Shape](../../com.aspose.cells/shape) - Returns a Shape object that represents the new WordArt object.
### addWordArt(int style, String text, int topRow, int top, int leftColumn, int left, int height, int width) {#addWordArt-int-java.lang.String-int-int-int-int-int-int-}
```
public Shape addWordArt(int style, String text, int topRow, int top, int leftColumn, int left, int height, int width)
```


自 Excel 2007 起添加预设 WordArt。

**Example**

```
         //add a WordArt
         Shape wordArt2 = shapes.addWordArt(PresetWordArtStyle.WORD_ART_STYLE_1, "WordArt", 3, 0, 3, 0, 50, 200);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). 预设的 WordArt 样式。 |
| 文本 | java.lang.String | 文本。 |
| topRow | int | 左上行索引。 |
| 顶部 | int | 表示形状相对于其左侧行的垂直偏移，以像素为单位。 |
| leftColumn | int | 左上列索引。 |
| 左侧 | int | 表示形状相对于左列的水平偏移量，单位为像素。 |
| 高度 | int | 表示形状的高度，单位为像素。 |
| 宽度 | int | 表示形状的宽度，单位为像素。 |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### clear() {#clear--}
```
public void clear()
```


清除工作表中的所有形状。

**Example**

```
         if (shapes.getCount() > 0)
         {
             shapes.clear();
         }
```

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


返回实例是否包含此对象

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| o | java.lang.Object | 测试对象 |

**Returns:**
boolean - 实例是否包含此对象
### copyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn) {#copyCommentsInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-}
```
public void copyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn)
```


复制范围内的所有批注。

**Example**

```
         CommentCollection comments = workbook.getWorksheets().get(0).getComments();
 
         //Add comment to cell A1
         int commentIndex = comments.add(0, 0);
         Comment comment = comments.get(commentIndex);
         comment.setNote("First note.");
         comment.getFont().setName("Times New Roman");
 
         //Add comment to cell B2
         comments.add("B2");
         comment = comments.get("B2");
         comment.setNote("Second note.");
 
         CellArea area1 = new CellArea();
         area1.StartColumn = 1;
         area1.StartRow = 1;
         area1.EndColumn = 5;
         area1.EndRow = 4;
 
         //copy
         shapes.copyCommentsInRange(shapes, area1, 5, 1);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| shapes | [ShapeCollection](../../com.aspose.cells/shapecollection) | 源形状。 |
| ca | [CellArea](../../com.aspose.cells/cellarea) | 源范围。 |
| destRow | int | 目标范围起始行。 |
| destColumn | int | 目标范围起始列。 |

### copyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, boolean isContained) {#copyInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-boolean-}
```
public void copyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, boolean isContained)
```


将范围内的形状复制到目标范围。

**Example**

```
         //add a shape
         shapes.addRectangle(2, 0, 2, 0, 130, 130);
         CellArea area2 = new CellArea();
         area2.StartColumn = 1;
         area2.StartRow = 1;
         area2.EndColumn = 5;
         area2.EndRow = 11;
 
         //copy
         shapes.copyInRange(shapes, area2, 12, 1, false);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceShapes | [ShapeCollection](../../com.aspose.cells/shapecollection) | 源形状。 |
| ca | [CellArea](../../com.aspose.cells/cellarea) | 源范围。 |
| destRow | int | 目标范围的目标行索引。 |
| destColumn | int | 目标范围的目标列。 |
| isContained | boolean | 是否仅复制位于范围内的形状。如果为 true，只复制范围内的形状。否则，行为与 MS Office 相同。 |

### deleteInRange(CellArea ca) {#deleteInRange-com.aspose.cells.CellArea-}
```
public void deleteInRange(CellArea ca)
```


删除范围内的形状。注释形状将不会被删除。

**Example**

```
         //add first shape
         shapes.addRectangle(2, 0, 2, 0, 50, 50);
         //add second shape
         shapes.addRectangle(6, 0, 2, 0, 30, 30);
 
         CellArea area3 = new CellArea();
         area3.StartColumn = 0;
         area3.StartRow = 5;
         area3.EndColumn = 5;
         area3.EndRow = 8;
 
         //del
         shapes.deleteInRange(area3);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | 范围。如果形状位于该范围内，它们将被移除。 |

### deleteShape(Shape shape) {#deleteShape-com.aspose.cells.Shape-}
```
public void deleteShape(Shape shape)
```


删除形状。如果形状位于组中或是注释形状，则不会被删除。

**Example**

```
         //add first shape
         Shape firstShape = shapes.addRectangle(2, 0, 2, 0, 50, 50);
         //add second shape
         Shape secondShape = shapes.addRectangle(6, 0, 2, 0, 30, 30);
         //del
         shapes.deleteShape(firstShape);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| shape | [Shape](../../com.aspose.cells/shape) |  |

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
### find(String what, int previous, FindOptions findOptions) {#find-java.lang.String-int-com.aspose.cells.FindOptions-}
```
public int find(String what, int previous, FindOptions findOptions)
```


按文本查找形状

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 什么 | java.lang.String | 要搜索的文本。 |
| 上一个 | int | 前一个形状的索引包含相同的文本。若从开始搜索则为 -1。 |
| findOptions | [FindOptions](../../com.aspose.cells/findoptions) | 查找选项 |

**Returns:**
int - 找到的形状索引，如果未找到形状则为 -1。
### get(int index) {#get-int-}
```
public Shape get(int index)
```


获取列表中特定索引的 [Shape](../../com.aspose.cells/shape) 对象。

**Example**

```
         //get the first shape
         Shape shape = shapes.get(0);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 索引。 |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### get(String name) {#get-java.lang.String-}
```
public Shape get(String name)
```


通过形状名称获取 [Shape](../../com.aspose.cells/shape) 对象。

**Example**

```
         //add a shape
         shapes.addRectangle(2, 0, 2, 0, 130, 130);
         //get the shape by the name.
         Shape shape1 = shapes.get("Rectangle 1");
         if(shape1 != null)
         {
             //Got the shape named 'Rectangle 1'.
         }
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 形状的名称。 |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
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


获取 CollectionBase 实例中包含的元素数量。

**Returns:**
int - CollectionBase 实例中包含的元素数量。
### group(Shape[] groupItems) {#group-com.aspose.cells.Shape---}
```
public GroupShape group(Shape[] groupItems)
```


对形状进行分组。

**Remarks**

groupItems 中的形状不应被分组。该形状必须位于此 Shapes 集合中。

**Example**

```
         //add first shape
         shapes.addRectangle(2, 0, 2, 0, 50, 50);
         //add second shape
         shapes.addRectangle(6, 0, 2, 0, 30, 30);
 
         Shape[] shapesArr = new Shape[] { shapes.get(0), shapes.get(1) };
         GroupShape groupShape = shapes.group(shapesArr);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| groupItems | [Shape\[\]](../../com.aspose.cells/shape) | 组项目。 |

**Returns:**
[GroupShape](../../com.aspose.cells/groupshape) - Returns the group shape.
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


确定 CollectionBase 实例中特定项的索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| o | java.lang.Object | 确定 CollectionBase 实例中特定项的索引。 |

**Returns:**
int - 如果在列表中找到该值则返回其索引；否则返回 -1。
### iterator() {#iterator--}
```
public Iterator iterator()
```


返回遍历 CollectionBase 实例的枚举器。

**Returns:**
java.util.Iterator - 用于遍历 CollectionBase 实例的迭代器。
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### remove(Shape shape) {#remove-com.aspose.cells.Shape-}
```
public void remove(Shape shape)
```


移除形状。

**Example**

```
         //add first shape
         shapes.addRectangle(2, 0, 2, 0, 50, 50);
         //add second shape
         shapes.addRectangle(6, 0, 2, 0, 30, 30);
 
         //get the shape
         Shape s = shapes.get("Rectangle 1");// or shapes[0];
         if (s != null)
         {
             //remove 
             shapes.remove(s);
         }
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| shape | [Shape](../../com.aspose.cells/shape) |  |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


移除形状。

**Example**

```
         //add first shape
         shapes.addRectangle(2, 0, 2, 0, 50, 50);
         //add second shape
         shapes.addRectangle(6, 0, 2, 0, 30, 30);
 
         //remove 
         shapes.removeAt(0);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 形状的索引。 |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### ungroup(GroupShape group) {#ungroup-com.aspose.cells.GroupShape-}
```
public void ungroup(GroupShape group)
```


取消形状项的分组。

**Remarks**

如果组形状被另一个组形状分组，则不执行任何操作。

**Example**

```
         //add first shape
         shapes.addRectangle(2, 0, 2, 0, 50, 50);
         //add second shape
         shapes.addRectangle(6, 0, 2, 0, 30, 30);
 
         //group
         Shape[] shapesArr = new Shape[] { shapes.get(0), shapes.get(1) };
         GroupShape groupShape = shapes.group(shapesArr);
 
         //ungroup
         shapes.ungroup(groupShape);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| group | [GroupShape](../../com.aspose.cells/groupshape) | 组形状。 |

### updateSelectedValue() {#updateSelectedValue--}
```
public void updateSelectedValue()
```


通过链接单元格或形状范围的值更新所选值。

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

