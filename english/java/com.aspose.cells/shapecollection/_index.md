---
title: ShapeCollection
second_title: Aspose.Cells for Java API Reference
description: Represents all the shape in a worksheet/chart.
type: docs
url: /java/com.aspose.cells/shapecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ShapeCollection extends CollectionBase
```

Represents all the shape in a worksheet/chart.

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
## Methods

| Method | Description |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Adds an item to the CollectionBase instance. |
| [addActiveXControl(int type, int topRow, int top, int leftColumn, int left, int width, int height)](#addActiveXControl-int-int-int-int-int-int-int-) | Creates an Activex Control. |
| [addArc(int topRow, int top, int leftColumn, int left, int height, int width)](#addArc-int-int-int-int-int-int-) | Adds a ArcShape to the worksheet. |
| [addAutoShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)](#addAutoShape-int-int-int-int-int-int-int-) | Adds a AutoShape to the worksheet. |
| [addAutoShapeInChart(int type, int top, int left, int height, int width)](#addAutoShapeInChart-int-int-int-int-int-) | Adds a AutoShape to the chart. |
| [addButton(int topRow, int top, int leftColumn, int left, int height, int width)](#addButton-int-int-int-int-int-int-) | Adds a Button to the worksheet. |
| [addCheckBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addCheckBox-int-int-int-int-int-int-) | Adds a checkbox to the worksheet. |
| [addComboBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addComboBox-int-int-int-int-int-int-) | Adds a ComboBox to the worksheet. |
| [addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left)](#addCopy-com.aspose.cells.Shape-int-int-int-int-) | Adds and copy a shape to the worksheet. |
| [addEquation(int topRow, int top, int leftColumn, int left, int height, int width)](#addEquation-int-int-int-int-int-int-) | Adds an equation object to the worksheet. |
| [addFreeFloatingShape(int type, int top, int left, int height, int width, byte[] imageData, boolean isOriginalSize)](#addFreeFloatingShape-int-int-int-int-int-byte---boolean-) | Adds a free floating shape to the worksheet.Only applies for line/image shape. |
| [addFreeform(int topRow, int top, int leftColumn, int left, int height, int width, ShapePath[] paths)](#addFreeform-int-int-int-int-int-int-com.aspose.cells.ShapePath---) | Adds a freeform shape to the worksheet. |
| [addGroupBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addGroupBox-int-int-int-int-int-int-) | Adds a GroupBox to the worksheet. |
| [addIcons(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageByteData, byte[] compatibleImageData)](#addIcons-int-int-int-int-int-int-byte---byte---) | Adds svg image. |
| [addLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, int width, String latex)](#addLaTeXEquation-int-int-int-int-int-int-java.lang.String-) | Adds an equation object to the worksheet using LaTeX format strings. |
| [addLabel(int topRow, int top, int leftColumn, int left, int height, int width)](#addLabel-int-int-int-int-int-int-) | Adds a Label to the worksheet. |
| [addLabelInChart(int top, int left, int height, int width)](#addLabelInChart-int-int-int-int-) | Adds a label to the chart. |
| [addLine(int topRow, int top, int leftColumn, int left, int height, int width)](#addLine-int-int-int-int-int-int-) | Adds a LineShape to the worksheet. |
| [addLinkedPicture(int topRow, int leftColumn, int height, int width, String sourceFullName)](#addLinkedPicture-int-int-int-int-java.lang.String-) | Add a linked picture. |
| [addListBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addListBox-int-int-int-int-int-int-) | Adds a ListBox to the worksheet. |
| [addOleObject(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageData)](#addOleObject-int-int-int-int-int-int-byte---) | Adds an OleObject. |
| [addOleObjectWithLinkedImage(int topRow, int leftColumn, int height, int width, String sourceFullName)](#addOleObjectWithLinkedImage-int-int-int-int-java.lang.String-) | Add a linked picture. |
| [addOval(int topRow, int top, int leftColumn, int left, int height, int width)](#addOval-int-int-int-int-int-int-) | Adds a Oval to the worksheet. |
| [addPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream)](#addPicture-int-int-int-int-java.io.InputStream-) | Adds a picture to the collection. |
| [addPicture(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale)](#addPicture-int-int-java.io.InputStream-int-int-) | Adds a picture to the collection. |
| [addPictureInChart(int top, int left, InputStream stream, int widthScale, int heightScale)](#addPictureInChart-int-int-java.io.InputStream-int-int-) | Adds a picture to the chart. |
| [addRadioButton(int topRow, int top, int leftColumn, int left, int height, int width)](#addRadioButton-int-int-int-int-int-int-) | Adds a RadioButton to the worksheet. |
| [addRectangle(int topRow, int top, int leftColumn, int left, int height, int width)](#addRectangle-int-int-int-int-int-int-) | Adds a RectangleShape to the worksheet. |
| [addScrollBar(int topRow, int top, int leftColumn, int left, int height, int width)](#addScrollBar-int-int-int-int-int-int-) | Adds a ScrollBar to the worksheet. |
| [addShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)](#addShape-int-int-int-int-int-int-int-) | Adds a Shape to the worksheet. |
| [addShapeInChart(int type, int placement, int left, int top, int right, int bottom)](#addShapeInChart-int-int-int-int-int-int-) | Add a shape to chart .All unit is 1/4000 of chart area. |
| [addShapeInChart(int type, int placement, int left, int top, int right, int bottom, byte[] imageData)](#addShapeInChart-int-int-int-int-int-int-byte---) | Add a shape to chart .All unit is 1/4000 of chart area. |
| [addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom)](#addShapeInChartByScale-int-int-double-double-double-double-) | Add a shape to chart. |
| [addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom, byte[] imageData)](#addShapeInChartByScale-int-int-double-double-double-double-byte---) | Add a shape to chart .All unit is 1/4000 of chart area. |
| [addSignatureLine(int topRow, int leftColumn, SignatureLine signatureLine)](#addSignatureLine-int-int-com.aspose.cells.SignatureLine-) | Adds a Signature Line to the worksheet. |
| [addSpinner(int topRow, int top, int leftColumn, int left, int height, int width)](#addSpinner-int-int-int-int-int-int-) | Adds a Spinner to the worksheet. |
| [addSvg(int topRow, int top, int leftColumn, int left, int height, int width, byte[] svgData, byte[] compatibleImageData)](#addSvg-int-int-int-int-int-int-byte---byte---) | Adds svg image. |
| [addTextBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addTextBox-int-int-int-int-int-int-) | Adds a text box to the worksheet. |
| [addTextBoxInChart(int top, int left, int height, int width)](#addTextBoxInChart-int-int-int-int-) | Adds a textbox to the chart. |
| [addTextEffect(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int topRow, int top, int leftColumn, int left, int height, int width)](#addTextEffect-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-int-int-) | Inserts a WordArt object. |
| [addTextEffectInChart(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int top, int left, int height, int width)](#addTextEffectInChart-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-) | Inserts a WordArt object to the chart |
| [addWordArt(int style, String text, int topRow, int top, int leftColumn, int left, int height, int width)](#addWordArt-int-java.lang.String-int-int-int-int-int-int-) | Adds preset WordArt since Excel 2007.s |
| [clear()](#clear--) | Clear all shapes in the worksheet. |
| [contains(Object o)](#contains-java.lang.Object-) | Return whether instance contains this object |
| [copyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn)](#copyCommentsInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-) | Copy all comments in the range. |
| [copyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, boolean isContained)](#copyInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-boolean-) | Copy shapes in the range to destination range. |
| [deleteInRange(CellArea ca)](#deleteInRange-com.aspose.cells.CellArea-) | Delete shapes in the range.Comment shapes will not be deleted. |
| [deleteShape(Shape shape)](#deleteShape-com.aspose.cells.Shape-) | Delete a shape. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gets the [Shape](../../com.aspose.cells/shape) object at the specific index in the list. |
| [get(String name)](#get-java.lang.String-) | Gets the [Shape](../../com.aspose.cells/shape) object by the name of the shape. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Gets the number of elements contained in the CollectionBase instance. |
| [group(Shape[] groupItems)](#group-com.aspose.cells.Shape---) | Group the shapes. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determines the index of a specific item in the CollectionBase instance. |
| [iterator()](#iterator--) | Returns an enumerator that iterates through the CollectionBase instance. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Shape shape)](#remove-com.aspose.cells.Shape-) | Remove the shape. |
| [removeAt(int index)](#removeAt-int-) | Remove the shape. |
| [toString()](#toString--) |  |
| [ungroup(GroupShape group)](#ungroup-com.aspose.cells.GroupShape-) | Ungroups the shape items. |
| [updateSelectedValue()](#updateSelectedValue--) | Update the selected value by the value of the linked cell or range of the shape. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Adds an item to the CollectionBase instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | The Object to add to the CollectionBase instance. |

**Returns:**
int - The position into which the new element was inserted.
### addActiveXControl(int type, int topRow, int top, int leftColumn, int left, int width, int height) {#addActiveXControl-int-int-int-int-int-int-int-}
```
public Shape addActiveXControl(int type, int topRow, int top, int leftColumn, int left, int width, int height)
```


Creates an Activex Control.

**Example**

```
         //add an ActiveX control
         Shape activeXControl = shapes.addActiveXControl(com.aspose.cells.ControlType.CHECK_BOX, 1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | [ControlType](../../com.aspose.cells/controltype). The type of the control. |
| topRow | int | Upper left row index. |
| top | int | Represents the vertical offset of Shape from its left row, in unit of pixel. |
| leftColumn | int | Upper left column index. |
| left | int | Represents the horizontal offset of Shape from its left column, in unit of pixel. |
| width | int | Represents the width of Shape, in unit of pixel. |
| height | int | Represents the height of Shape, in unit of pixel. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### addArc(int topRow, int top, int leftColumn, int left, int height, int width) {#addArc-int-int-int-int-int-int-}
```
public ArcShape addArc(int topRow, int top, int leftColumn, int left, int height, int width)
```


Adds a ArcShape to the worksheet.

**Example**

```
         //add a arc
         ArcShape arcShape = shapes.addArc(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int | Upper left row index. |
| top | int | Represents the vertical offset of ArcShape from its left row, in unit of pixel. |
| leftColumn | int | Upper left column index. |
| left | int | Represents the horizontal offset of ArcShape from its left column, in unit of pixel. |
| height | int | Represents the height of ArcShape, in unit of pixel. |
| width | int | Represents the width of ArcShape, in unit of pixel. |

**Returns:**
[ArcShape](../../com.aspose.cells/arcshape) - A ArcShape object.
### addAutoShape(int type, int topRow, int top, int leftColumn, int left, int height, int width) {#addAutoShape-int-int-int-int-int-int-int-}
```
public Shape addAutoShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)
```


Adds a AutoShape to the worksheet.

**Remarks**

The type could not be Chart/Comment/Picture/OleObject/Polygon/DialogBox

**Example**

```
         //Adds a AutoShape to the worksheet.
         Shape autoShape = shapes.addAutoShape(AutoShapeType.CUBE, 1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | [AutoShapeType](../../com.aspose.cells/autoshapetype). Auto shape type. |
| topRow | int | Upper left row index. |
| top | int | Represents the vertical offset of Shape from its left row, in unit of pixel. |
| leftColumn | int | Upper left column index. |
| left | int | Represents the horizontal offset of Shape from its left column, in unit of pixel. |
| height | int | Represents the height of Shape, in unit of pixel. |
| width | int | Represents the width of Shape, in unit of pixel. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - A Shape object.
### addAutoShapeInChart(int type, int top, int left, int height, int width) {#addAutoShapeInChart-int-int-int-int-int-}
```
public Shape addAutoShapeInChart(int type, int top, int left, int height, int width)
```


Adds a AutoShape to the chart.

**Remarks**

The type could not be Chart/Comment/Picture/OleObject/Polygon/DialogBox

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | [AutoShapeType](../../com.aspose.cells/autoshapetype). Auto shape type. |
| top | int | Represents the vertical offset of textbox from the upper left corner in units of 1/4000 of the chart area. |
| left | int | Represents the vertical offset of textbox from the upper left corner in units of 1/4000 of the chart area. |
| height | int | Represents the height of textbox, in units of 1/4000 of the chart area. |
| width | int | Represents the width of textbox, in units of 1/4000 of the chart area. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - Returns a shape object.
### addButton(int topRow, int top, int leftColumn, int left, int height, int width) {#addButton-int-int-int-int-int-int-}
```
public Button addButton(int topRow, int top, int leftColumn, int left, int height, int width)
```


Adds a Button to the worksheet.

**Example**

```
         //add a button
         Button button = shapes.addButton(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int | Upper left row index. |
| top | int | Represents the vertical offset of Button from its left row, in unit of pixel. |
| leftColumn | int | Upper left column index. |
| left | int | Represents the horizontal offset of Button from its left column, in unit of pixel. |
| height | int | Represents the height of Button, in unit of pixel. |
| width | int | Represents the width of Button, in unit of pixel. |

**Returns:**
[Button](../../com.aspose.cells/button) - A Button object.
### addCheckBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addCheckBox-int-int-int-int-int-int-}
```
public CheckBox addCheckBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Adds a checkbox to the worksheet.

**Example**

```
         //add a CheckBox
         CheckBox checkBox = shapes.addCheckBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int | Upper left row index. |
| top | int | Represents the vertical offset of checkbox from its top row, in unit of pixel. |
| leftColumn | int | Upper left column index. |
| left | int | Represents the horizontal offset of textbox from its left column, in unit of pixel. |
| height | int | Height of textbox, in unit of pixel. |
| width | int | Width of textbox, in unit of pixel. |

**Returns:**
[CheckBox](../../com.aspose.cells/checkbox) - The new CheckBox object index.
### addComboBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addComboBox-int-int-int-int-int-int-}
```
public ComboBox addComboBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Adds a ComboBox to the worksheet.

**Example**

```
         //add a combo box
         ComboBox comboBox = shapes.addComboBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int | Upper left row index. |
| top | int | Represents the vertical offset of ComboBox from its left row, in unit of pixel. |
| leftColumn | int | Upper left column index. |
| left | int | Represents the horizontal offset of ComboBox from its left column, in unit of pixel. |
| height | int | Represents the height of ComboBox, in unit of pixel. |
| width | int | Represents the width of ComboBox, in unit of pixel. |

**Returns:**
[ComboBox](../../com.aspose.cells/combobox) - A ComboBox object.
### addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left) {#addCopy-com.aspose.cells.Shape-int-int-int-int-}
```
public Shape addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left)
```


Adds and copy a shape to the worksheet.

**Example**

```
         //add a shape
         RectangleShape rectangle = shapes.addRectangle(2, 0, 2, 0, 130, 130);
         //Adds and copies a shape.
         shapes.addCopy(rectangle, 7, 0, 7, 0);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceShape | [Shape](../../com.aspose.cells/shape) | Source shape. |
| topRow | int | The top row index. |
| top | int | Represents the vertical offset from its top row, in unit of pixel. |
| leftColumn | int | The left column index. |
| left | int | Represents the horizontal offset from its left column, in unit of pixel. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - The new [Shape](../../com.aspose.cells/shape) object.
### addEquation(int topRow, int top, int leftColumn, int left, int height, int width) {#addEquation-int-int-int-int-int-int-}
```
public TextBox addEquation(int topRow, int top, int leftColumn, int left, int height, int width)
```


Adds an equation object to the worksheet.

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
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int | The top row index. |
| top | int | The vertical offset its top row, in unit of pixel. |
| leftColumn | int | The left column index. |
| left | int | The horizontal offset from its left column, in unit of pixel. |
| height | int | The height of equation, in unit of pixel. |
| width | int | The width of equation, in unit of pixel. |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - 
### addFreeFloatingShape(int type, int top, int left, int height, int width, byte[] imageData, boolean isOriginalSize) {#addFreeFloatingShape-int-int-int-int-int-byte---boolean-}
```
public Shape addFreeFloatingShape(int type, int top, int left, int height, int width, byte[] imageData, boolean isOriginalSize)
```


Adds a free floating shape to the worksheet.Only applies for line/image shape.

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
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). The shape type. |
| top | int | Represents the vertical offset of shape from the worksheet's top row, in unit of pixel. |
| left | int | Represents the horizontal offset of shape from the worksheet's left column, in unit of pixel. |
| height | int | Represents the height of LineShape, in unit of pixel. |
| width | int | Represents the width of LineShape, in unit of pixel. |
| imageData | byte[] | The image data,only applies for the picture. |
| isOriginalSize | boolean | Whether the shape use original size if the shape is image. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### addFreeform(int topRow, int top, int leftColumn, int left, int height, int width, ShapePath[] paths) {#addFreeform-int-int-int-int-int-int-com.aspose.cells.ShapePath---}
```
public Shape addFreeform(int topRow, int top, int leftColumn, int left, int height, int width, ShapePath[] paths)
```


Adds a freeform shape to the worksheet.

**Remarks**

Notice: That the width and height in the parameters can be any positive integer values, not the total width and height of the ShapePath array specified by \\u9225\\u6a96aths'. The relationship between them is a scale-fill relationship, that is, each ShapePath object will be scaled according to the width and height. Therefore, when there are multiple objects in the 'paths', each ShapePath object needs to be designed reasonably to meet expectations. When there is only one ShapePath object and there are no other requirements, passing the object's width and height as parameter values \\u9225\\u5b27\\u20ac\\u5a94s a good solution.

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
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int | Upper left row index. |
| top | int | Represents the vertical offset of freeform shape from its left row, in unit of pixel. |
| leftColumn | int | Upper left column index. |
| left | int | Represents the horizontal offset of freeform shape from its left column, in unit of pixel. |
| height | int | Represents the height of freeform shape, in unit of pixel. |
| width | int | Represents the width of freeform shape, in unit of pixel. |
| paths | [ShapePath\[\]](../../com.aspose.cells/shapepath) | Represents a user-defined path |

**Returns:**
[Shape](../../com.aspose.cells/shape) - A freeform shape.
### addGroupBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addGroupBox-int-int-int-int-int-int-}
```
public GroupBox addGroupBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Adds a GroupBox to the worksheet.

**Example**

```
         //add a group box
         GroupBox groupBox = shapes.addGroupBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int | Upper left row index. |
| top | int | Represents the vertical offset of GroupBox from its left row, in unit of pixel. |
| leftColumn | int | Upper left column index. |
| left | int | Represents the horizontal offset of GroupBox from its left column, in unit of pixel. |
| height | int | Represents the height of GroupBox, in unit of pixel. |
| width | int | Represents the width of GroupBox, in unit of pixel. |

**Returns:**
[GroupBox](../../com.aspose.cells/groupbox) - A GroupBox object.
### addIcons(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageByteData, byte[] compatibleImageData) {#addIcons-int-int-int-int-int-int-byte---byte---}
```
public Picture addIcons(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageByteData, byte[] compatibleImageData)
```


Adds svg image.

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
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int | Upper left row index. |
| top | int | Represents the vertical offset of shape from its left row, in unit of pixel. |
| leftColumn | int | Upper left column index. |
| left | int | The horizontal offset of shape from its left column, in unit of pixel. |
| height | int | The height of shape, in unit of pixel. |
| width | int | The width of shape, in unit of pixel. |
| imageByteData | byte[] | The image byte data. |
| compatibleImageData | byte[] | Converted image data from svg in order to be compatible with Excel 2016 or lower versions. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - 
### addLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, int width, String latex) {#addLaTeXEquation-int-int-int-int-int-int-java.lang.String-}
```
public TextBox addLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, int width, String latex)
```


Adds an equation object to the worksheet using LaTeX format strings.

**Example**

```
         // LaTeX format string.
         String latex = "\\alpha +  \\frac{\\partial^2}{\\partial x_1\\partial x_2}y - \\left ( a + b \\right )+_{a}^{b}\\beta";
         // Adds an equation object to the worksheet.
         TextBox textBox = shapes.addLaTeXEquation(1, 0, 1, 0, 100, 300, latex);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int | The top row index. |
| top | int | The vertical offset its top row, in unit of pixel. |
| leftColumn | int | The left column index. |
| left | int | The horizontal offset from its left column, in unit of pixel. |
| height | int | The height of equation, in unit of pixel. |
| width | int | The width of equation, in unit of pixel. |
| latex | java.lang.String | LaTeX format string |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - 
### addLabel(int topRow, int top, int leftColumn, int left, int height, int width) {#addLabel-int-int-int-int-int-int-}
```
public Label addLabel(int topRow, int top, int leftColumn, int left, int height, int width)
```


Adds a Label to the worksheet.

**Example**

```
         //add a label
         Label label = shapes.addLabel(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int | Upper left row index. |
| top | int | Represents the vertical offset of Label from its left row, in unit of pixel. |
| leftColumn | int | Upper left column index. |
| left | int | Represents the horizontal offset of Label from its left column, in unit of pixel. |
| height | int | Represents the height of Label, in unit of pixel. |
| width | int | Represents the width of Label, in unit of pixel. |

**Returns:**
[Label](../../com.aspose.cells/label) - A Label object.
### addLabelInChart(int top, int left, int height, int width) {#addLabelInChart-int-int-int-int-}
```
public Label addLabelInChart(int top, int left, int height, int width)
```


Adds a label to the chart.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| top | int | Represents the vertical offset of label from the upper left corner in units of 1/4000 of the chart area. |
| left | int | Represents the vertical offset of label from the upper left corner in units of 1/4000 of the chart area. |
| height | int | Represents the height of label, in units of 1/4000 of the chart area. |
| width | int | Represents the width of label, in units of 1/4000 of the chart area. |

**Returns:**
[Label](../../com.aspose.cells/label) - A new Label object.
### addLine(int topRow, int top, int leftColumn, int left, int height, int width) {#addLine-int-int-int-int-int-int-}
```
public LineShape addLine(int topRow, int top, int leftColumn, int left, int height, int width)
```


Adds a LineShape to the worksheet.

**Example**

```
         // add a line object
         LineShape lineShape = shapes.addLine(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int | Upper left row index. |
| top | int | Represents the vertical offset of LineShape from its left row, in unit of pixel. |
| leftColumn | int | Upper left column index. |
| left | int | Represents the horizontal offset of LineShape from its left column, in unit of pixel. |
| height | int | Represents the height of LineShape, in unit of pixel. |
| width | int | Represents the width of LineShape, in unit of pixel. |

**Returns:**
[LineShape](../../com.aspose.cells/lineshape) - A LineShape object.
### addLinkedPicture(int topRow, int leftColumn, int height, int width, String sourceFullName) {#addLinkedPicture-int-int-int-int-java.lang.String-}
```
public Picture addLinkedPicture(int topRow, int leftColumn, int height, int width, String sourceFullName)
```


Add a linked picture.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int | Upper left row index. |
| leftColumn | int | Upper left column index. |
| height | int | The height of the shape. In unit of pixels |
| width | int | The width of the shape. In unit of pixels |
| sourceFullName | java.lang.String | The path and name of the source file for the linked image |

**Returns:**
[Picture](../../com.aspose.cells/picture) - [Picture](../../com.aspose.cells/picture) Picture object.
### addListBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addListBox-int-int-int-int-int-int-}
```
public ListBox addListBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Adds a ListBox to the worksheet.

**Example**

```
         //add a list box
         ListBox listBox = shapes.addListBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int | Upper left row index. |
| top | int | Represents the vertical offset of ListBox from its left row, in unit of pixel. |
| leftColumn | int | Upper left column index. |
| left | int | Represents the horizontal offset of ListBox from its left column, in unit of pixel. |
| height | int | Represents the height of ListBox, in unit of pixel. |
| width | int | Represents the width of ListBox, in unit of pixel. |

**Returns:**
[ListBox](../../com.aspose.cells/listbox) - A ListBox object.
### addOleObject(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageData) {#addOleObject-int-int-int-int-int-int-byte---}
```
public OleObject addOleObject(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageData)
```


Adds an OleObject.

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
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int |  |
| top | int |  |
| leftColumn | int |  |
| left | int |  |
| height | int |  |
| width | int |  |
| imageData | byte[] |  |

**Returns:**
[OleObject](../../com.aspose.cells/oleobject) - 
### addOleObjectWithLinkedImage(int topRow, int leftColumn, int height, int width, String sourceFullName) {#addOleObjectWithLinkedImage-int-int-int-int-java.lang.String-}
```
public OleObject addOleObjectWithLinkedImage(int topRow, int leftColumn, int height, int width, String sourceFullName)
```


Add a linked picture.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int | Upper left row index. |
| leftColumn | int | Upper left column index. |
| height | int | The height of the shape. In unit of pixels |
| width | int | The width of the shape. In unit of pixels |
| sourceFullName | java.lang.String | The path and name of the source file for the linked image |

**Returns:**
[OleObject](../../com.aspose.cells/oleobject) - [Picture](../../com.aspose.cells/picture) Picture object.
### addOval(int topRow, int top, int leftColumn, int left, int height, int width) {#addOval-int-int-int-int-int-int-}
```
public Oval addOval(int topRow, int top, int leftColumn, int left, int height, int width)
```


Adds a Oval to the worksheet.

**Example**

```
         //add a oval
         Oval oval = shapes.addOval(1, 0, 1, 0, 50, 50);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int | Upper left row index. |
| top | int | Represents the vertical offset of Oval from its left row, in unit of pixel. |
| leftColumn | int | Upper left column index. |
| left | int | Represents the horizontal offset of Oval from its left column, in unit of pixel. |
| height | int | Represents the height of Oval, in unit of pixel. |
| width | int | Represents the width of Oval, in unit of pixel. |

**Returns:**
[Oval](../../com.aspose.cells/oval) - A Oval object.
### addPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream) {#addPicture-int-int-int-int-java.io.InputStream-}
```
public Picture addPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream)
```


Adds a picture to the collection.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int | Upper left row index. |
| leftColumn | int | Upper left column index. |
| bottomRow | int | Lower right row index |
| rightColumn | int | Lower right column index |
| stream | java.io.InputStream | Stream object which contains the image data. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - [Picture](../../com.aspose.cells/picture) Picture object.
### addPicture(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale) {#addPicture-int-int-java.io.InputStream-int-int-}
```
public Picture addPicture(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale)
```


Adds a picture to the collection.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int | Upper left row index. |
| leftColumn | int | Upper left column index. |
| stream | java.io.InputStream | Stream object which contains the image data. |
| widthScale | int | Scale of image width, a percentage. |
| heightScale | int | Scale of image height, a percentage. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - [Picture](../../com.aspose.cells/picture) Picture object.
### addPictureInChart(int top, int left, InputStream stream, int widthScale, int heightScale) {#addPictureInChart-int-int-java.io.InputStream-int-int-}
```
public Picture addPictureInChart(int top, int left, InputStream stream, int widthScale, int heightScale)
```


Adds a picture to the chart.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| top | int | Represents the vertical offset of shape from the upper left corner in units of 1/4000 of the chart area. |
| left | int | Represents the horizontal offset of shape from the upper left corner in units of 1/4000 of the chart area. |
| stream | java.io.InputStream | Stream object which contains the image data. |
| widthScale | int | Scale of image width, a percentage. |
| heightScale | int | Scale of image height, a percentage. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns a Picture object.
### addRadioButton(int topRow, int top, int leftColumn, int left, int height, int width) {#addRadioButton-int-int-int-int-int-int-}
```
public RadioButton addRadioButton(int topRow, int top, int leftColumn, int left, int height, int width)
```


Adds a RadioButton to the worksheet.

**Example**

```
         //add a radio button
         RadioButton radioButton = shapes.addRadioButton(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int | Upper left row index. |
| top | int | Represents the vertical offset of RadioButton from its left row, in unit of pixel. |
| leftColumn | int | Upper left column index. |
| left | int | Represents the horizontal offset of RadioButton from its left column, in unit of pixel. |
| height | int | Represents the height of RadioButton, in unit of pixel. |
| width | int | Represents the width of RadioButton, in unit of pixel. |

**Returns:**
[RadioButton](../../com.aspose.cells/radiobutton) - A RadioButton object.
### addRectangle(int topRow, int top, int leftColumn, int left, int height, int width) {#addRectangle-int-int-int-int-int-int-}
```
public RectangleShape addRectangle(int topRow, int top, int leftColumn, int left, int height, int width)
```


Adds a RectangleShape to the worksheet.

**Example**

```
         // add a rectangle
         RectangleShape rectangleShape = shapes.addRectangle(2, 0, 2, 0, 130, 130);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int | Upper left row index. |
| top | int | Represents the vertical offset of RectangleShape from its left row, in unit of pixel. |
| leftColumn | int | Upper left column index. |
| left | int | Represents the horizontal offset of RectangleShape from its left column, in unit of pixel. |
| height | int | Represents the height of RectangleShape, in unit of pixel. |
| width | int | Represents the width of RectangleShape, in unit of pixel. |

**Returns:**
[RectangleShape](../../com.aspose.cells/rectangleshape) - A RectangleShape object.
### addScrollBar(int topRow, int top, int leftColumn, int left, int height, int width) {#addScrollBar-int-int-int-int-int-int-}
```
public ScrollBar addScrollBar(int topRow, int top, int leftColumn, int left, int height, int width)
```


Adds a ScrollBar to the worksheet.

**Example**

```
         //add a scroll bar
         ScrollBar scrollBar = shapes.addScrollBar(1, 0, 1, 0, 100, 20);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int | Upper left row index. |
| top | int | Represents the vertical offset of ScrollBar from its left row, in unit of pixel. |
| leftColumn | int | Upper left column index. |
| left | int | Represents the horizontal offset of ScrollBar from its left column, in unit of pixel. |
| height | int | Represents the height of ScrollBar, in unit of pixel. |
| width | int | Represents the width of ScrollBar, in unit of pixel. |

**Returns:**
[ScrollBar](../../com.aspose.cells/scrollbar) - A ScrollBar object.
### addShape(int type, int topRow, int top, int leftColumn, int left, int height, int width) {#addShape-int-int-int-int-int-int-int-}
```
public Shape addShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)
```


Adds a Shape to the worksheet.

**Remarks**

The type could not be Chart/Comment/Picture/OleObject/Polygon/DialogBox

**Example**

```
         //Add a shape of the specified type
         Shape shapeByType = shapes.addShape(MsoDrawingType.CELLS_DRAWING, 1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Mso drawing type. |
| topRow | int | Upper left row index. |
| top | int | Represents the vertical offset of Shape from its left row, in unit of pixel. |
| leftColumn | int | Upper left column index. |
| left | int | Represents the horizontal offset of Shape from its left column, in unit of pixel. |
| height | int | Represents the height of Shape, in unit of pixel. |
| width | int | Represents the width of Shape, in unit of pixel. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - A Shape object.
### addShapeInChart(int type, int placement, int left, int top, int right, int bottom) {#addShapeInChart-int-int-int-int-int-int-}
```
public Shape addShapeInChart(int type, int placement, int left, int top, int right, int bottom)
```


Add a shape to chart .All unit is 1/4000 of chart area.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). The drawing type. |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype). the placement type. |
| left | int | In unit of 1/4000 chart area width. |
| top | int | In unit of 1/4000 chart area height. |
| right | int | In unit of 1/4000 chart area width. |
| bottom | int | In unit of 1/4000 chart area height. |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addShapeInChart(int type, int placement, int left, int top, int right, int bottom, byte[] imageData) {#addShapeInChart-int-int-int-int-int-int-byte---}
```
public Shape addShapeInChart(int type, int placement, int left, int top, int right, int bottom, byte[] imageData)
```


Add a shape to chart .All unit is 1/4000 of chart area.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). The drawing type. |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype). the placement type. |
| left | int | In unit of 1/4000 chart area width. |
| top | int | In unit of 1/4000 chart area height. |
| right | int | In unit of 1/4000 chart area width. |
| bottom | int | In unit of 1/4000 chart area height. |
| imageData | byte[] | If the shape is not a picture or ole object,imageData should be null. |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom) {#addShapeInChartByScale-int-int-double-double-double-double-}
```
public Shape addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom)
```


Add a shape to chart. All unit is percent scale of chart area.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). The drawing type. |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype). the placement type. |
| left | double | Unit is percent scale of chart area width. |
| top | double | Unit is percent scale of chart area height. |
| right | double | Unit is percent scale of chart area width. |
| bottom | double | Unit is percent scale of chart area height. |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom, byte[] imageData) {#addShapeInChartByScale-int-int-double-double-double-double-byte---}
```
public Shape addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom, byte[] imageData)
```


Add a shape to chart .All unit is 1/4000 of chart area.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). The drawing type. |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype). the placement type. |
| left | double | Unit is percent scale of chart area width. |
| top | double | Unit is percent scale of chart area height. |
| right | double | Unit is percent scale of chart area width. |
| bottom | double | Unit is percent scale of chart area height. |
| imageData | byte[] | If the shape is not a picture or ole object,imageData should be null. |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addSignatureLine(int topRow, int leftColumn, SignatureLine signatureLine) {#addSignatureLine-int-int-com.aspose.cells.SignatureLine-}
```
public Picture addSignatureLine(int topRow, int leftColumn, SignatureLine signatureLine)
```


Adds a Signature Line to the worksheet.

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
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int | Upper left row index. |
| leftColumn | int | Upper left column index. |
| signatureLine | [SignatureLine](../../com.aspose.cells/signatureline) | Represents a signature line object. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - 
### addSpinner(int topRow, int top, int leftColumn, int left, int height, int width) {#addSpinner-int-int-int-int-int-int-}
```
public Spinner addSpinner(int topRow, int top, int leftColumn, int left, int height, int width)
```


Adds a Spinner to the worksheet.

**Example**

```
         //add a spinner
         Spinner spinner = shapes.addSpinner(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int | Upper left row index. |
| top | int | Represents the vertical offset of Spinner from its left row, in unit of pixel. |
| leftColumn | int | Upper left column index. |
| left | int | Represents the horizontal offset of Spinner from its left column, in unit of pixel. |
| height | int | Represents the height of Spinner, in unit of pixel. |
| width | int | Represents the width of Spinner, in unit of pixel. |

**Returns:**
[Spinner](../../com.aspose.cells/spinner) - A Spinner object.
### addSvg(int topRow, int top, int leftColumn, int left, int height, int width, byte[] svgData, byte[] compatibleImageData) {#addSvg-int-int-int-int-int-int-byte---byte---}
```
public Picture addSvg(int topRow, int top, int leftColumn, int left, int height, int width, byte[] svgData, byte[] compatibleImageData)
```


Adds svg image.

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
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int | Upper left row index. |
| top | int | Represents the vertical offset of shape from its left row, in unit of pixel. |
| leftColumn | int | Upper left column index. |
| left | int | The horizontal offset of shape from its left column, in unit of pixel. |
| height | int | The height of shape, in unit of pixel. |
| width | int | The width of shape, in unit of pixel. |
| svgData | byte[] | The svg image data. |
| compatibleImageData | byte[] | Converted image data from svg in order to be compatible with Excel 2016 or lower versions. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - 
### addTextBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addTextBox-int-int-int-int-int-int-}
```
public TextBox addTextBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Adds a text box to the worksheet.

**Example**

```
         //add a TextBox
         TextBox textBox = shapes.addTextBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int | Upper left row index. |
| top | int | Represents the vertical offset of textbox from its top row, in unit of pixel. |
| leftColumn | int | Upper left column index. |
| left | int | Represents the horizontal offset of textbox from its left column, in unit of pixel. |
| height | int | Represents the height of textbox, in unit of pixel. |
| width | int | Represents the width of textbox, in unit of pixel. |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - A [TextBox](../../com.aspose.cells/textbox) object.
### addTextBoxInChart(int top, int left, int height, int width) {#addTextBoxInChart-int-int-int-int-}
```
public TextBox addTextBoxInChart(int top, int left, int height, int width)
```


Adds a textbox to the chart.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| top | int | Represents the vertical offset of textbox from the upper left corner in units of 1/4000 of the chart area. |
| left | int | Represents the vertical offset of textbox from the upper left corner in units of 1/4000 of the chart area. |
| height | int | Represents the height of textbox, in units of 1/4000 of the chart area. |
| width | int | Represents the width of textbox, in units of 1/4000 of the chart area. |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - A TextBox object.
### addTextEffect(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int topRow, int top, int leftColumn, int left, int height, int width) {#addTextEffect-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-int-int-}
```
public Shape addTextEffect(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int topRow, int top, int leftColumn, int left, int height, int width)
```


Inserts a WordArt object.

**Example**

```
         //add a WordArt
         Shape wordArt1 = shapes.addTextEffect(MsoPresetTextEffect.TEXT_EFFECT_10, "WordArt", "arial", 18, false, false, 3, 0, 3, 0, 200, 50);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| effect | int | [MsoPresetTextEffect](../../com.aspose.cells/msopresettexteffect). The mso preset text effect type. |
| text | java.lang.String | The WordArt text. |
| fontName | java.lang.String | The font name. |
| size | int | The font size |
| fontBold | boolean | Indicates whether font is bold. |
| fontItalic | boolean | Indicates whether font is italic. |
| topRow | int | Upper left row index. |
| top | int | Represents the vertical offset of shape from its left row, in unit of pixel. |
| leftColumn | int | Upper left column index. |
| left | int | Represents the horizontal offset of shape from its left column, in unit of pixel. |
| height | int | Represents the height of shape, in unit of pixel. |
| width | int | Represents the width of shape, in unit of pixel. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - Returns a Shape object that represents the new WordArt object.
### addTextEffectInChart(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int top, int left, int height, int width) {#addTextEffectInChart-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-}
```
public Shape addTextEffectInChart(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int top, int left, int height, int width)
```


Inserts a WordArt object to the chart

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| effect | int | [MsoPresetTextEffect](../../com.aspose.cells/msopresettexteffect). The mso preset text effect type. |
| text | java.lang.String | The WordArt text. |
| fontName | java.lang.String | The font name. |
| size | int | The font size |
| fontBold | boolean | Indicates whether font is bold. |
| fontItalic | boolean | Indicates whether font is italic. |
| top | int | Represents the vertical offset of shape from the upper left corner in units of 1/4000 of the chart area. |
| left | int | Represents the vertical offset of shape from the upper left corner in units of 1/4000 of the chart area. |
| height | int | Represents the height of shape, in units of 1/4000 of the chart area. |
| width | int | Represents the width of shape, in units of 1/4000 of the chart area. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - Returns a Shape object that represents the new WordArt object.
### addWordArt(int style, String text, int topRow, int top, int leftColumn, int left, int height, int width) {#addWordArt-int-java.lang.String-int-int-int-int-int-int-}
```
public Shape addWordArt(int style, String text, int topRow, int top, int leftColumn, int left, int height, int width)
```


Adds preset WordArt since Excel 2007.s

**Example**

```
         //add a WordArt
         Shape wordArt2 = shapes.addWordArt(PresetWordArtStyle.WORD_ART_STYLE_1, "WordArt", 3, 0, 3, 0, 50, 200);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). The preset WordArt Style. |
| text | java.lang.String | The text. |
| topRow | int | Upper left row index. |
| top | int | Represents the vertical offset of shape from its left row, in unit of pixel. |
| leftColumn | int | Upper left column index. |
| left | int | Represents the horizontal offset of shape from its left column, in unit of pixel. |
| height | int | Represents the height of shape, in unit of pixel. |
| width | int | Represents the width of shape, in unit of pixel. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### clear() {#clear--}
```
public void clear()
```


Clear all shapes in the worksheet.

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


Return whether instance contains this object

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | test object |

**Returns:**
boolean - Whether instance contains this object
### copyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn) {#copyCommentsInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-}
```
public void copyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn)
```


Copy all comments in the range.

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
| Parameter | Type | Description |
| --- | --- | --- |
| shapes | [ShapeCollection](../../com.aspose.cells/shapecollection) | The source shapes. |
| ca | [CellArea](../../com.aspose.cells/cellarea) | The source range. |
| destRow | int | The dest range start row. |
| destColumn | int | The dest range start column. |

### copyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, boolean isContained) {#copyInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-boolean-}
```
public void copyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, boolean isContained)
```


Copy shapes in the range to destination range.

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
| Parameter | Type | Description |
| --- | --- | --- |
| sourceShapes | [ShapeCollection](../../com.aspose.cells/shapecollection) | Source shapes. |
| ca | [CellArea](../../com.aspose.cells/cellarea) | The source range. |
| destRow | int | The dest row index of the dest range. |
| destColumn | int | The dest column of the dest range. |
| isContained | boolean | Whether only copy the shapes which are contained in the range. If true,only copies the shapes in the range. Otherwise,it works as MS Office. |

### deleteInRange(CellArea ca) {#deleteInRange-com.aspose.cells.CellArea-}
```
public void deleteInRange(CellArea ca)
```


Delete shapes in the range.Comment shapes will not be deleted.

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
| Parameter | Type | Description |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | The range.If the shapes are contained in the range, they will be removed. |

### deleteShape(Shape shape) {#deleteShape-com.aspose.cells.Shape-}
```
public void deleteShape(Shape shape)
```


Delete a shape. If the shape is in the group or is a comment shape, it will not be deleted.

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
| Parameter | Type | Description |
| --- | --- | --- |
| shape | [Shape](../../com.aspose.cells/shape) |  |

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
### get(int index) {#get-int-}
```
public Shape get(int index)
```


Gets the [Shape](../../com.aspose.cells/shape) object at the specific index in the list.

**Example**

```
         //get the first shape
         Shape shape = shapes.get(0);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The index. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### get(String name) {#get-java.lang.String-}
```
public Shape get(String name)
```


Gets the [Shape](../../com.aspose.cells/shape) object by the name of the shape.

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
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the shape. |

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


Gets the number of elements contained in the CollectionBase instance.

**Returns:**
int - The number of elements contained in the CollectionBase instance.
### group(Shape[] groupItems) {#group-com.aspose.cells.Shape---}
```
public GroupShape group(Shape[] groupItems)
```


Group the shapes.

**Remarks**

The shape in the groupItems should not be grouped. The shape must be in this Shapes collection.

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
| Parameter | Type | Description |
| --- | --- | --- |
| groupItems | [Shape\[\]](../../com.aspose.cells/shape) | the group items. |

**Returns:**
[GroupShape](../../com.aspose.cells/groupshape) - Return the group shape.
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


Determines the index of a specific item in the CollectionBase instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | Determines the index of a specific item in the CollectionBase instance. |

**Returns:**
int - The index of value if found in the list; otherwise, -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Returns an enumerator that iterates through the CollectionBase instance.

**Returns:**
java.util.Iterator - An iterator for the CollectionBase instance.
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


Remove the shape.

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
| Parameter | Type | Description |
| --- | --- | --- |
| shape | [Shape](../../com.aspose.cells/shape) |  |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Remove the shape.

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
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The index of the shape. |

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


Ungroups the shape items.

**Remarks**

If the group shape is grouped by another group shape,nothing will be done.

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
| Parameter | Type | Description |
| --- | --- | --- |
| group | [GroupShape](../../com.aspose.cells/groupshape) | The group shape. |

### updateSelectedValue() {#updateSelectedValue--}
```
public void updateSelectedValue()
```


Update the selected value by the value of the linked cell or range of the shape.

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

