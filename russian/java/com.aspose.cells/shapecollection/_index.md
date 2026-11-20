---
title: "ShapeCollection"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет все формы в листе/диаграмме."
type: docs
url: /ru/java/com.aspose.cells/shapecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ShapeCollection extends CollectionBase
```

Представляет все формы в листе/диаграмме.

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
## Методы

| Метод | Описание |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Добавляет элемент в экземпляр CollectionBase. |
| [addActiveXControl(int type, int topRow, int top, int leftColumn, int left, int width, int height)](#addActiveXControl-int-int-int-int-int-int-int-) | Создает Activex Control. |
| [addArc(int topRow, int top, int leftColumn, int left, int height, int width)](#addArc-int-int-int-int-int-int-) | Добавляет ArcShape в лист. |
| [addAutoShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)](#addAutoShape-int-int-int-int-int-int-int-) | Добавляет AutoShape в лист. |
| [addAutoShapeInChart(int type, int top, int left, int height, int width)](#addAutoShapeInChart-int-int-int-int-int-) | Добавляет AutoShape в диаграмму. |
| [addButton(int topRow, int top, int leftColumn, int left, int height, int width)](#addButton-int-int-int-int-int-int-) | Добавляет Button в лист. |
| [addCheckBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addCheckBox-int-int-int-int-int-int-) | Добавляет checkbox в лист. |
| [addComboBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addComboBox-int-int-int-int-int-int-) | Добавляет ComboBox в лист. |
| [addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left)](#addCopy-com.aspose.cells.Shape-int-int-int-int-) | Добавляет и копирует shape в лист. |
| [addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left, CopyOptions copyOptions)](#addCopy-com.aspose.cells.Shape-int-int-int-int-com.aspose.cells.CopyOptions-) | Добавляет и копирует shape в лист. |
| [addEquation(int topRow, int top, int leftColumn, int left, int height, int width)](#addEquation-int-int-int-int-int-int-) | Добавляет equation object в лист. |
| [addFreeFloatingShape(int type, int top, int left, int height, int width, byte[] imageData, boolean isOriginalSize)](#addFreeFloatingShape-int-int-int-int-int-byte---boolean-) | Добавляет free floating shape в лист. Применяется только к line/image shape. |
| [addFreeform(int topRow, int top, int leftColumn, int left, int height, int width, ShapePath[] paths)](#addFreeform-int-int-int-int-int-int-com.aspose.cells.ShapePath---) | Добавляет freeform shape в лист. |
| [addGroupBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addGroupBox-int-int-int-int-int-int-) | Добавляет GroupBox в лист. |
| [addIcons(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageByteData, byte[] compatibleImageData)](#addIcons-int-int-int-int-int-int-byte---byte---) | Добавляет svg изображение. |
| [addLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, int width, String latex)](#addLaTeXEquation-int-int-int-int-int-int-java.lang.String-) | Добавляет equation object в лист, используя строки формата LaTeX. |
| [addLabel(int topRow, int top, int leftColumn, int left, int height, int width)](#addLabel-int-int-int-int-int-int-) | Добавляет Label в лист. |
| [addLabelInChart(int top, int left, int height, int width)](#addLabelInChart-int-int-int-int-) | Добавляет label в диаграмму. |
| [addLine(int topRow, int top, int leftColumn, int left, int height, int width)](#addLine-int-int-int-int-int-int-) | Добавляет LineShape в лист. |
| [addLinkedPicture(int topRow, int leftColumn, int height, int width, String sourceFullName)](#addLinkedPicture-int-int-int-int-java.lang.String-) | Добавьте linked picture. |
| [addListBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addListBox-int-int-int-int-int-int-) | Добавляет ListBox в лист. |
| [addOleObject(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageData)](#addOleObject-int-int-int-int-int-int-byte---) | Добавляет OleObject. |
| [addOleObjectWithLinkedImage(int topRow, int leftColumn, int height, int width, String sourceFullName)](#addOleObjectWithLinkedImage-int-int-int-int-java.lang.String-) | Добавьте linked picture. |
| [addOval(int topRow, int top, int leftColumn, int left, int height, int width)](#addOval-int-int-int-int-int-int-) | Добавляет Oval в лист. |
| [addPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream)](#addPicture-int-int-int-int-java.io.InputStream-) | Добавляет picture в коллекцию. |
| [addPicture(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale)](#addPicture-int-int-java.io.InputStream-int-int-) | Добавляет picture в коллекцию. |
| [addPictureInChart(int top, int left, InputStream stream, int widthScale, int heightScale)](#addPictureInChart-int-int-java.io.InputStream-int-int-) | Добавляет picture в диаграмму. |
| [addRadioButton(int topRow, int top, int leftColumn, int left, int height, int width)](#addRadioButton-int-int-int-int-int-int-) | Добавляет RadioButton в лист. |
| [addRectangle(int topRow, int top, int leftColumn, int left, int height, int width)](#addRectangle-int-int-int-int-int-int-) | Добавляет RectangleShape в рабочий лист. |
| [addScrollBar(int topRow, int top, int leftColumn, int left, int height, int width)](#addScrollBar-int-int-int-int-int-int-) | Добавляет ScrollBar в рабочий лист. |
| [addShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)](#addShape-int-int-int-int-int-int-int-) | Добавляет Shape в рабочий лист. |
| [addShapeInChart(int type, int placement, int left, int top, int right, int bottom)](#addShapeInChart-int-int-int-int-int-int-) | Добавьте shape в диаграмму. Все единицы — 1/4000 области диаграммы. |
| [addShapeInChart(int type, int placement, int left, int top, int right, int bottom, byte[] imageData)](#addShapeInChart-int-int-int-int-int-int-byte---) | Добавьте shape в диаграмму. Все единицы — 1/4000 области диаграммы. |
| [addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom)](#addShapeInChartByScale-int-int-double-double-double-double-) | Добавьте shape в диаграмму. |
| [addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom, byte[] imageData)](#addShapeInChartByScale-int-int-double-double-double-double-byte---) | Добавьте shape в диаграмму. Все единицы — 1/4000 области диаграммы. |
| [addSignatureLine(int topRow, int leftColumn, SignatureLine signatureLine)](#addSignatureLine-int-int-com.aspose.cells.SignatureLine-) | Добавляет Signature Line в рабочий лист. |
| [addSpinner(int topRow, int top, int leftColumn, int left, int height, int width)](#addSpinner-int-int-int-int-int-int-) | Добавляет Spinner в рабочий лист. |
| [addSvg(int topRow, int top, int leftColumn, int left, int height, int width, byte[] svgData, byte[] compatibleImageData)](#addSvg-int-int-int-int-int-int-byte---byte---) | Добавляет svg изображение. |
| [addTextBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addTextBox-int-int-int-int-int-int-) | Добавляет текстовое поле в рабочий лист. |
| [addTextBoxInChart(int top, int left, int height, int width)](#addTextBoxInChart-int-int-int-int-) | Добавляет текстовое поле в диаграмму. |
| [addTextEffect(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int topRow, int top, int leftColumn, int left, int height, int width)](#addTextEffect-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-int-int-) | Вставляет объект WordArt. |
| [addTextEffectInChart(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int top, int left, int height, int width)](#addTextEffectInChart-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-) | Вставляет объект WordArt в диаграмму. |
| [addWordArt(int style, String text, int topRow, int top, int leftColumn, int left, int height, int width)](#addWordArt-int-java.lang.String-int-int-int-int-int-int-) | Добавляет предустановленный WordArt, начиная с Excel 2007. |
| [clear()](#clear--) | Очистить все фигуры в рабочем листе. |
| [contains(Object o)](#contains-java.lang.Object-) | Возвращает, содержит ли экземпляр этот объект |
| [copyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn)](#copyCommentsInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-) | Скопировать все комментарии в диапазоне. |
| [copyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, boolean isContained)](#copyInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-boolean-) | Скопировать фигуры в диапазоне в целевой диапазон. |
| [deleteInRange(CellArea ca)](#deleteInRange-com.aspose.cells.CellArea-) | Удалить фигуры в диапазоне. Фигуры комментариев не будут удалены. |
| [deleteShape(Shape shape)](#deleteShape-com.aspose.cells.Shape-) | Удалить фигуру. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [find(String what, int previous, FindOptions findOptions)](#find-java.lang.String-int-com.aspose.cells.FindOptions-) | Найти фигуру по тексту. |
| [get(int index)](#get-int-) | Получает объект [Shape](../../com.aspose.cells/shape) по конкретному индексу в списке. |
| [get(String name)](#get-java.lang.String-) | Получает объект [Shape](../../com.aspose.cells/shape) по имени фигуры. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Получает количество элементов, содержащихся в экземпляре CollectionBase. |
| [group(Shape[] groupItems)](#group-com.aspose.cells.Shape---) | Группировать фигуры. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Определяет индекс конкретного элемента в экземпляре CollectionBase. |
| [iterator()](#iterator--) | Возвращает перечислитель, который проходит по экземпляру CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Shape shape)](#remove-com.aspose.cells.Shape-) | Удалить фигуру. |
| [removeAt(int index)](#removeAt-int-) | Удалить фигуру. |
| [toString()](#toString--) |  |
| [ungroup(GroupShape group)](#ungroup-com.aspose.cells.GroupShape-) | Разгруппировать элементы фигур. |
| [updateSelectedValue()](#updateSelectedValue--) | Обновить выбранное значение значением связанной ячейки или диапазона фигуры. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Добавляет элемент в экземпляр CollectionBase.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| o | java.lang.Object | Объект, который нужно добавить в экземпляр CollectionBase. |

**Returns:**
int — позиция, в которую был вставлен новый элемент.
### addActiveXControl(int type, int topRow, int top, int leftColumn, int left, int width, int height) {#addActiveXControl-int-int-int-int-int-int-int-}
```
public Shape addActiveXControl(int type, int topRow, int top, int leftColumn, int left, int width, int height)
```


Создает Activex Control.

**Example**

```
         //add an ActiveX control
         Shape activeXControl = shapes.addActiveXControl(com.aspose.cells.ControlType.CHECK_BOX, 1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [ControlType](../../com.aspose.cells/controltype). Тип управления. |
| topRow | int | Индекс строки в верхнем левом углу. |
| верх | int | Представляет вертикальное смещение Shape от его левой строки, в единицах пикселя. |
| leftColumn | int | Индекс столбца в верхнем левом углу. |
| лево | int | Представляет горизонтальное смещение Shape от его левого столбца, в единицах пикселя. |
| width | int | Представляет ширину Shape, в единицах пикселя. |
| height | int | Представляет высоту Shape, в единицах пикселя. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### addArc(int topRow, int top, int leftColumn, int left, int height, int width) {#addArc-int-int-int-int-int-int-}
```
public ArcShape addArc(int topRow, int top, int leftColumn, int left, int height, int width)
```


Добавляет ArcShape в лист.

**Example**

```
         //add a arc
         ArcShape arcShape = shapes.addArc(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | int | Индекс строки в верхнем левом углу. |
| верх | int | Представляет вертикальное смещение ArcShape от его левой строки, в единицах пикселя. |
| leftColumn | int | Индекс столбца в верхнем левом углу. |
| лево | int | Представляет горизонтальное смещение ArcShape от его левого столбца, в единицах пикселя. |
| height | int | Представляет высоту ArcShape, в единицах пикселя. |
| width | int | Представляет ширину ArcShape, в единицах пикселя. |

**Returns:**
[ArcShape](../../com.aspose.cells/arcshape) - A ArcShape object.
### addAutoShape(int type, int topRow, int top, int leftColumn, int left, int height, int width) {#addAutoShape-int-int-int-int-int-int-int-}
```
public Shape addAutoShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)
```


Добавляет AutoShape в лист.

**Remarks**

Тип не может быть Chart/Comment/Picture/OleObject/Polygon/DialogBox

**Example**

```
         //Adds a AutoShape to the worksheet.
         Shape autoShape = shapes.addAutoShape(AutoShapeType.CUBE, 1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [AutoShapeType](../../com.aspose.cells/autoshapetype). Тип автофигуры. |
| topRow | int | Индекс строки в верхнем левом углу. |
| верх | int | Представляет вертикальное смещение Shape от его левой строки, в единицах пикселя. |
| leftColumn | int | Индекс столбца в верхнем левом углу. |
| лево | int | Представляет горизонтальное смещение Shape от его левого столбца, в единицах пикселя. |
| height | int | Представляет высоту Shape, в единицах пикселя. |
| width | int | Представляет ширину Shape, в единицах пикселя. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - A Shape object.
### addAutoShapeInChart(int type, int top, int left, int height, int width) {#addAutoShapeInChart-int-int-int-int-int-}
```
public Shape addAutoShapeInChart(int type, int top, int left, int height, int width)
```


Добавляет AutoShape в диаграмму.

**Remarks**

Тип не может быть Chart/Comment/Picture/OleObject/Polygon/DialogBox

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [AutoShapeType](../../com.aspose.cells/autoshapetype). Тип автофигуры. |
| верх | int | Представляет вертикальное смещение textbox от верхнего левого угла в единицах 1/4000 области диаграммы. |
| лево | int | Представляет вертикальное смещение textbox от верхнего левого угла в единицах 1/4000 области диаграммы. |
| height | int | Представляет высоту textbox, в единицах 1/4000 области диаграммы. |
| width | int | Представляет ширину textbox, в единицах 1/4000 области диаграммы. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - Returns a shape object.
### addButton(int topRow, int top, int leftColumn, int left, int height, int width) {#addButton-int-int-int-int-int-int-}
```
public Button addButton(int topRow, int top, int leftColumn, int left, int height, int width)
```


Добавляет Button в лист.

**Example**

```
         //add a button
         Button button = shapes.addButton(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | int | Индекс строки в верхнем левом углу. |
| верх | int | Представляет вертикальное смещение Button от его левой строки, в единицах пикселя. |
| leftColumn | int | Индекс столбца в верхнем левом углу. |
| лево | int | Представляет горизонтальное смещение Button от его левого столбца, в единицах пикселя. |
| height | int | Представляет высоту Button, в единицах пикселя. |
| width | int | Представляет ширину Button, в единицах пикселя. |

**Returns:**
[Button](../../com.aspose.cells/button) - A Button object.
### addCheckBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addCheckBox-int-int-int-int-int-int-}
```
public CheckBox addCheckBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Добавляет checkbox в лист.

**Example**

```
         //add a CheckBox
         CheckBox checkBox = shapes.addCheckBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | int | Индекс строки в верхнем левом углу. |
| верх | int | Представляет вертикальное смещение checkbox от его верхней строки, в единицах пикселя. |
| leftColumn | int | Индекс столбца в верхнем левом углу. |
| лево | int | Представляет горизонтальное смещение textbox от его левого столбца, в единицах пикселя. |
| height | int | Высота textbox, в единицах пикселя. |
| width | int | Ширина textbox, в единицах пикселя. |

**Returns:**
[CheckBox](../../com.aspose.cells/checkbox) - The new CheckBox object index.
### addComboBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addComboBox-int-int-int-int-int-int-}
```
public ComboBox addComboBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Добавляет ComboBox в лист.

**Example**

```
         //add a combo box
         ComboBox comboBox = shapes.addComboBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | int | Индекс строки в верхнем левом углу. |
| верх | int | Представляет вертикальное смещение ComboBox от его левой строки, в единицах пикселя. |
| leftColumn | int | Индекс столбца в верхнем левом углу. |
| лево | int | Представляет горизонтальное смещение ComboBox от его левого столбца, в единицах пикселя. |
| height | int | Представляет высоту ComboBox в единицах пикселей. |
| width | int | Представляет ширину ComboBox в единицах пикселей. |

**Returns:**
[ComboBox](../../com.aspose.cells/combobox) - A ComboBox object.
### addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left) {#addCopy-com.aspose.cells.Shape-int-int-int-int-}
```
public Shape addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left)
```


Добавляет и копирует shape в лист.

**Example**

```
         //add a shape
         RectangleShape rectangle = shapes.addRectangle(2, 0, 2, 0, 130, 130);
         //Adds and copies a shape.
         shapes.addCopy(rectangle, 7, 0, 7, 0);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceShape | [Shape](../../com.aspose.cells/shape) | Исходная форма. |
| topRow | int | Индекс верхней строки. |
| верх | int | Представляет вертикальное смещение от её верхней строки в единицах пикселей. |
| leftColumn | int | Индекс левого столбца. |
| лево | int | Представляет горизонтальное смещение от её левого столбца в единицах пикселей. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - The new [Shape](../../com.aspose.cells/shape) object.
### addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left, CopyOptions copyOptions) {#addCopy-com.aspose.cells.Shape-int-int-int-int-com.aspose.cells.CopyOptions-}
```
public Shape addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left, CopyOptions copyOptions)
```


Добавляет и копирует shape в лист.

**Example**

```
         //add a shape
         RectangleShape rectangle = shapes.addRectangle(2, 0, 2, 0, 130, 130);
         //Adds and copies a shape.
         shapes.addCopy(rectangle, 7, 0, 7, 0);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceShape | [Shape](../../com.aspose.cells/shape) | Исходная форма. |
| topRow | int | Индекс верхней строки. |
| верх | int | Представляет вертикальное смещение от её верхней строки в единицах пикселей. |
| leftColumn | int | Индекс левого столбца. |
| лево | int | Представляет горизонтальное смещение от её левого столбца в единицах пикселей. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | Параметры копирования фигур. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - The new [Shape](../../com.aspose.cells/shape) object.
### addEquation(int topRow, int top, int leftColumn, int left, int height, int width) {#addEquation-int-int-int-int-int-int-}
```
public TextBox addEquation(int topRow, int top, int leftColumn, int left, int height, int width)
```


Добавляет equation object в лист.

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | int | Индекс верхней строки. |
| верх | int | Вертикальное смещение её верхней строки в единицах пикселей. |
| leftColumn | int | Индекс левого столбца. |
| лево | int | Горизонтальное смещение от её левого столбца в единицах пикселей. |
| height | int | Высота уравнения в единицах пикселей. |
| width | int | Ширина уравнения в единицах пикселей. |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - 
### addFreeFloatingShape(int type, int top, int left, int height, int width, byte[] imageData, boolean isOriginalSize) {#addFreeFloatingShape-int-int-int-int-int-byte---boolean-}
```
public Shape addFreeFloatingShape(int type, int top, int left, int height, int width, byte[] imageData, boolean isOriginalSize)
```


Добавляет free floating shape в лист. Применяется только к line/image shape.

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Тип фигуры. |
| верх | int | Представляет вертикальное смещение фигуры от верхней строки листа в единицах пикселей. |
| лево | int | Представляет горизонтальное смещение фигуры от левого столбца листа в единицах пикселей. |
| height | int | Представляет высоту LineShape в единицах пикселей. |
| width | int | Представляет ширину LineShape в единицах пикселей. |
| imageData | byte[] | Данные изображения, применимы только к картинке. |
| isOriginalSize | boolean | Использует ли фигура оригинальный размер, если она является изображением. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### addFreeform(int topRow, int top, int leftColumn, int left, int height, int width, ShapePath[] paths) {#addFreeform-int-int-int-int-int-int-com.aspose.cells.ShapePath---}
```
public Shape addFreeform(int topRow, int top, int leftColumn, int left, int height, int width, ShapePath[] paths)
```


Добавляет freeform shape в лист.

**Remarks**

Примечание: Ширина и высота в параметрах могут быть любыми положительными целыми значениями, а не общей шириной и высотой массива ShapePath, указанного в \\u9225\\u6a96aths'. Связь между ними — отношение масштаб‑заполнение, то есть каждый объект ShapePath будет масштабироваться в соответствии с шириной и высотой. Поэтому, когда в 'paths' присутствует несколько объектов, каждый объект ShapePath необходимо проектировать разумно, чтобы соответствовать ожиданиям. Когда присутствует только один объект ShapePath и нет других требований, передача ширины и высоты объекта в качестве значений параметров \\u9225\\u5b27\\u20ac\\u5a94s является хорошим решением.

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | int | Индекс строки в верхнем левом углу. |
| верх | int | Представляет вертикальное смещение свободной формы от её левой строки в единицах пикселей. |
| leftColumn | int | Индекс столбца в верхнем левом углу. |
| лево | int | Представляет горизонтальное смещение свободной формы от её левого столбца в единицах пикселей. |
| height | int | Представляет высоту свободной формы в единицах пикселей. |
| width | int | Представляет ширину свободной формы в единицах пикселей. |
| paths | [ShapePath\[\]](../../com.aspose.cells/shapepath) | Представляет пользовательский путь |

**Returns:**
[Shape](../../com.aspose.cells/shape) - A freeform shape.
### addGroupBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addGroupBox-int-int-int-int-int-int-}
```
public GroupBox addGroupBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Добавляет GroupBox в лист.

**Example**

```
         //add a group box
         GroupBox groupBox = shapes.addGroupBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | int | Индекс строки в верхнем левом углу. |
| верх | int | Представляет вертикальное смещение GroupBox от его левой строки, в пикселях. |
| leftColumn | int | Индекс столбца в верхнем левом углу. |
| лево | int | Представляет горизонтальное смещение GroupBox от его левого столбца, в пикселях. |
| height | int | Представляет высоту GroupBox, в пикселях. |
| width | int | Представляет ширину GroupBox, в пикселях. |

**Returns:**
[GroupBox](../../com.aspose.cells/groupbox) - A GroupBox object.
### addIcons(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageByteData, byte[] compatibleImageData) {#addIcons-int-int-int-int-int-int-byte---byte---}
```
public Picture addIcons(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageByteData, byte[] compatibleImageData)
```


Добавляет svg изображение.

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | int | Индекс строки в верхнем левом углу. |
| верх | int | Представляет вертикальное смещение shape от его левой строки, в пикселях. |
| leftColumn | int | Индекс столбца в верхнем левом углу. |
| лево | int | Горизонтальное смещение shape от его левого столбца, в пикселях. |
| height | int | Высота shape, в пикселях. |
| width | int | Ширина shape, в пикселях. |
| imageByteData | byte[] | Байтовые данные изображения. |
| compatibleImageData | byte[] | Преобразованные данные изображения из svg, чтобы быть совместимыми с Excel 2016 или более ранними версиями. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - 
### addLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, int width, String latex) {#addLaTeXEquation-int-int-int-int-int-int-java.lang.String-}
```
public TextBox addLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, int width, String latex)
```


Добавляет equation object в лист, используя строки формата LaTeX.

**Example**

```
         // LaTeX format string.
         String latex = "\\alpha +  \\frac{\\partial^2}{\\partial x_1\\partial x_2}y - \\left ( a + b \\right )+_{a}^{b}\\beta";
         // Adds an equation object to the worksheet.
         TextBox textBox = shapes.addLaTeXEquation(1, 0, 1, 0, 100, 300, latex);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | int | Индекс верхней строки. |
| верх | int | Вертикальное смещение её верхней строки в единицах пикселей. |
| leftColumn | int | Индекс левого столбца. |
| лево | int | Горизонтальное смещение от её левого столбца в единицах пикселей. |
| height | int | Высота уравнения в единицах пикселей. |
| width | int | Ширина уравнения в единицах пикселей. |
| latex | java.lang.String | Строка формата LaTeX |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - 
### addLabel(int topRow, int top, int leftColumn, int left, int height, int width) {#addLabel-int-int-int-int-int-int-}
```
public Label addLabel(int topRow, int top, int leftColumn, int left, int height, int width)
```


Добавляет Label в лист.

**Example**

```
         //add a label
         Label label = shapes.addLabel(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | int | Индекс строки в верхнем левом углу. |
| верх | int | Представляет вертикальное смещение Label от его левой строки, в пикселях. |
| leftColumn | int | Индекс столбца в верхнем левом углу. |
| лево | int | Представляет горизонтальное смещение Label от его левого столбца, в пикселях. |
| height | int | Представляет высоту Label, в пикселях. |
| width | int | Представляет ширину Label, в пикселях. |

**Returns:**
[Label](../../com.aspose.cells/label) - A Label object.
### addLabelInChart(int top, int left, int height, int width) {#addLabelInChart-int-int-int-int-}
```
public Label addLabelInChart(int top, int left, int height, int width)
```


Добавляет label в диаграмму.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| верх | int | Представляет вертикальное смещение label от верхнего левого угла в единицах 1/4000 области диаграммы. |
| лево | int | Представляет вертикальное смещение label от верхнего левого угла в единицах 1/4000 области диаграммы. |
| height | int | Представляет высоту label, в единицах 1/4000 области диаграммы. |
| width | int | Представляет ширину label, в единицах 1/4000 области диаграммы. |

**Returns:**
[Label](../../com.aspose.cells/label) - A new Label object.
### addLine(int topRow, int top, int leftColumn, int left, int height, int width) {#addLine-int-int-int-int-int-int-}
```
public LineShape addLine(int topRow, int top, int leftColumn, int left, int height, int width)
```


Добавляет LineShape в лист.

**Example**

```
         // add a line object
         LineShape lineShape = shapes.addLine(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | int | Индекс строки в верхнем левом углу. |
| верх | int | Представляет вертикальное смещение LineShape от его левой строки, в пикселях. |
| leftColumn | int | Индекс столбца в верхнем левом углу. |
| лево | int | Представляет горизонтальное смещение LineShape от его левого столбца, в пикселях. |
| height | int | Представляет высоту LineShape в единицах пикселей. |
| width | int | Представляет ширину LineShape в единицах пикселей. |

**Returns:**
[LineShape](../../com.aspose.cells/lineshape) - A LineShape object.
### addLinkedPicture(int topRow, int leftColumn, int height, int width, String sourceFullName) {#addLinkedPicture-int-int-int-int-java.lang.String-}
```
public Picture addLinkedPicture(int topRow, int leftColumn, int height, int width, String sourceFullName)
```


Добавьте linked picture.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | int | Индекс строки в верхнем левом углу. |
| leftColumn | int | Индекс столбца в верхнем левом углу. |
| height | int | Высота формы. В пикселях |
| width | int | Ширина фигуры. В единицах пикселей |
| sourceFullName | java.lang.String | Путь и имя исходного файла для связанного изображения |

**Returns:**
[Picture](../../com.aspose.cells/picture) - [Picture](../../com.aspose.cells/picture) Picture object.
### addListBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addListBox-int-int-int-int-int-int-}
```
public ListBox addListBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Добавляет ListBox в лист.

**Example**

```
         //add a list box
         ListBox listBox = shapes.addListBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | int | Индекс строки в верхнем левом углу. |
| верх | int | Представляет вертикальное смещение ListBox от его левой строки, в единицах пикселей. |
| leftColumn | int | Индекс столбца в верхнем левом углу. |
| лево | int | Представляет горизонтальное смещение ListBox от его левого столбца, в единицах пикселей. |
| height | int | Представляет высоту ListBox, в единицах пикселей. |
| width | int | Представляет ширину ListBox, в единицах пикселей. |

**Returns:**
[ListBox](../../com.aspose.cells/listbox) - A ListBox object.
### addOleObject(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageData) {#addOleObject-int-int-int-int-int-int-byte---}
```
public OleObject addOleObject(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageData)
```


Добавляет OleObject.

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | int |  |
| верх | int |  |
| leftColumn | int |  |
| лево | int |  |
| height | int |  |
| width | int |  |
| imageData | byte[] |  |

**Returns:**
[OleObject](../../com.aspose.cells/oleobject) - 
### addOleObjectWithLinkedImage(int topRow, int leftColumn, int height, int width, String sourceFullName) {#addOleObjectWithLinkedImage-int-int-int-int-java.lang.String-}
```
public OleObject addOleObjectWithLinkedImage(int topRow, int leftColumn, int height, int width, String sourceFullName)
```


Добавьте linked picture.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | int | Индекс строки в верхнем левом углу. |
| leftColumn | int | Индекс столбца в верхнем левом углу. |
| height | int | Высота формы. В пикселях |
| width | int | Ширина фигуры. В единицах пикселей |
| sourceFullName | java.lang.String | Путь и имя исходного файла для связанного изображения |

**Returns:**
[OleObject](../../com.aspose.cells/oleobject) - [Picture](../../com.aspose.cells/picture) Picture object.
### addOval(int topRow, int top, int leftColumn, int left, int height, int width) {#addOval-int-int-int-int-int-int-}
```
public Oval addOval(int topRow, int top, int leftColumn, int left, int height, int width)
```


Добавляет Oval в лист.

**Example**

```
         //add a oval
         Oval oval = shapes.addOval(1, 0, 1, 0, 50, 50);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | int | Индекс строки в верхнем левом углу. |
| верх | int | Представляет вертикальное смещение Oval от его левой строки, в единицах пикселей. |
| leftColumn | int | Индекс столбца в верхнем левом углу. |
| лево | int | Представляет горизонтальное смещение Oval от его левого столбца, в единицах пикселей. |
| height | int | Представляет высоту Oval, в единицах пикселей. |
| width | int | Представляет ширину Oval, в единицах пикселей. |

**Returns:**
[Oval](../../com.aspose.cells/oval) - A Oval object.
### addPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream) {#addPicture-int-int-int-int-java.io.InputStream-}
```
public Picture addPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream)
```


Добавляет picture в коллекцию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | int | Индекс строки в верхнем левом углу. |
| leftColumn | int | Индекс столбца в верхнем левом углу. |
| bottomRow | int | Индекс строки в нижнем правом углу |
| rightColumn | int | Индекс столбца в нижнем правом углу |
| stream | java.io.InputStream | Объект потока, содержащий данные изображения. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - [Picture](../../com.aspose.cells/picture) Picture object.
### addPicture(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale) {#addPicture-int-int-java.io.InputStream-int-int-}
```
public Picture addPicture(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale)
```


Добавляет picture в коллекцию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | int | Индекс строки в верхнем левом углу. |
| leftColumn | int | Индекс столбца в верхнем левом углу. |
| stream | java.io.InputStream | Объект потока, содержащий данные изображения. |
| widthScale | int | Масштаб ширины изображения, в процентах. |
| heightScale | int | Масштаб высоты изображения, в процентах. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - [Picture](../../com.aspose.cells/picture) Picture object.
### addPictureInChart(int top, int left, InputStream stream, int widthScale, int heightScale) {#addPictureInChart-int-int-java.io.InputStream-int-int-}
```
public Picture addPictureInChart(int top, int left, InputStream stream, int widthScale, int heightScale)
```


Добавляет picture в диаграмму.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| верх | int | Представляет вертикальное смещение фигуры от верхнего левого угла в единицах 1/4000 области диаграммы. |
| лево | int | Представляет горизонтальное смещение фигуры от верхнего левого угла в единицах 1/4000 области диаграммы. |
| stream | java.io.InputStream | Объект потока, содержащий данные изображения. |
| widthScale | int | Масштаб ширины изображения, в процентах. |
| heightScale | int | Масштаб высоты изображения, в процентах. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns a Picture object.
### addRadioButton(int topRow, int top, int leftColumn, int left, int height, int width) {#addRadioButton-int-int-int-int-int-int-}
```
public RadioButton addRadioButton(int topRow, int top, int leftColumn, int left, int height, int width)
```


Добавляет RadioButton в лист.

**Example**

```
         //add a radio button
         RadioButton radioButton = shapes.addRadioButton(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | int | Индекс строки в верхнем левом углу. |
| верх | int | Представляет вертикальное смещение RadioButton от его левой строки, в единицах пикселей. |
| leftColumn | int | Индекс столбца в верхнем левом углу. |
| лево | int | Представляет горизонтальное смещение RadioButton от его левого столбца, в единицах пикселей. |
| height | int | Представляет высоту RadioButton, в единицах пикселей. |
| width | int | Представляет ширину RadioButton, в единицах пикселей. |

**Returns:**
[RadioButton](../../com.aspose.cells/radiobutton) - A RadioButton object.
### addRectangle(int topRow, int top, int leftColumn, int left, int height, int width) {#addRectangle-int-int-int-int-int-int-}
```
public RectangleShape addRectangle(int topRow, int top, int leftColumn, int left, int height, int width)
```


Добавляет RectangleShape в рабочий лист.

**Example**

```
         // add a rectangle
         RectangleShape rectangleShape = shapes.addRectangle(2, 0, 2, 0, 130, 130);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | int | Индекс строки в верхнем левом углу. |
| верх | int | Представляет вертикальное смещение RectangleShape от его левой строки, в единицах пикселей. |
| leftColumn | int | Индекс столбца в верхнем левом углу. |
| лево | int | Представляет горизонтальное смещение RectangleShape от его левого столбца, в единицах пикселей. |
| height | int | Представляет высоту RectangleShape в единице пикселя. |
| width | int | Представляет ширину RectangleShape в единице пикселя. |

**Returns:**
[RectangleShape](../../com.aspose.cells/rectangleshape) - A RectangleShape object.
### addScrollBar(int topRow, int top, int leftColumn, int left, int height, int width) {#addScrollBar-int-int-int-int-int-int-}
```
public ScrollBar addScrollBar(int topRow, int top, int leftColumn, int left, int height, int width)
```


Добавляет ScrollBar в рабочий лист.

**Example**

```
         //add a scroll bar
         ScrollBar scrollBar = shapes.addScrollBar(1, 0, 1, 0, 100, 20);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | int | Индекс строки в верхнем левом углу. |
| верх | int | Представляет вертикальное смещение ScrollBar от его левой строки в единице пикселя. |
| leftColumn | int | Индекс столбца в верхнем левом углу. |
| лево | int | Представляет горизонтальное смещение ScrollBar от его левого столбца в единице пикселя. |
| height | int | Представляет высоту ScrollBar в единице пикселя. |
| width | int | Представляет ширину ScrollBar в единице пикселя. |

**Returns:**
[ScrollBar](../../com.aspose.cells/scrollbar) - A ScrollBar object.
### addShape(int type, int topRow, int top, int leftColumn, int left, int height, int width) {#addShape-int-int-int-int-int-int-int-}
```
public Shape addShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)
```


Добавляет Shape в рабочий лист.

**Remarks**

Тип не может быть Chart/Comment/Picture/OleObject/Polygon/DialogBox

**Example**

```
         //Add a shape of the specified type
         Shape shapeByType = shapes.addShape(MsoDrawingType.CELLS_DRAWING, 1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Тип рисунка Mso. |
| topRow | int | Индекс строки в верхнем левом углу. |
| верх | int | Представляет вертикальное смещение Shape от его левой строки, в единицах пикселя. |
| leftColumn | int | Индекс столбца в верхнем левом углу. |
| лево | int | Представляет горизонтальное смещение Shape от его левого столбца, в единицах пикселя. |
| height | int | Представляет высоту Shape, в единицах пикселя. |
| width | int | Представляет ширину Shape, в единицах пикселя. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - A Shape object.
### addShapeInChart(int type, int placement, int left, int top, int right, int bottom) {#addShapeInChart-int-int-int-int-int-int-}
```
public Shape addShapeInChart(int type, int placement, int left, int top, int right, int bottom)
```


Добавьте shape в диаграмму. Все единицы — 1/4000 области диаграммы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Тип рисунка. |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype). тип размещения. |
| лево | int | В единице 1/4000 ширины области диаграммы. |
| верх | int | В единице 1/4000 высоты области диаграммы. |
| право | int | В единице 1/4000 ширины области диаграммы. |
| низ | int | В единице 1/4000 высоты области диаграммы. |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addShapeInChart(int type, int placement, int left, int top, int right, int bottom, byte[] imageData) {#addShapeInChart-int-int-int-int-int-int-byte---}
```
public Shape addShapeInChart(int type, int placement, int left, int top, int right, int bottom, byte[] imageData)
```


Добавьте shape в диаграмму. Все единицы — 1/4000 области диаграммы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Тип рисунка. |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype). тип размещения. |
| лево | int | В единице 1/4000 ширины области диаграммы. |
| верх | int | В единице 1/4000 высоты области диаграммы. |
| право | int | В единице 1/4000 ширины области диаграммы. |
| низ | int | В единице 1/4000 высоты области диаграммы. |
| imageData | byte[] | Если фигура не является изображением или объектом OLE, imageData должно быть null. |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom) {#addShapeInChartByScale-int-int-double-double-double-double-}
```
public Shape addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom)
```


Добавьте фигуру в диаграмму. Все единицы — процентный масштаб области диаграммы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Тип рисунка. |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype). тип размещения. |
| лево | double | Единица — процентный масштаб ширины области диаграммы. |
| верх | double | Единица — процентный масштаб высоты области диаграммы. |
| право | double | Единица — процентный масштаб ширины области диаграммы. |
| низ | double | Единица — процентный масштаб высоты области диаграммы. |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom, byte[] imageData) {#addShapeInChartByScale-int-int-double-double-double-double-byte---}
```
public Shape addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom, byte[] imageData)
```


Добавьте shape в диаграмму. Все единицы — 1/4000 области диаграммы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Тип рисунка. |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype). тип размещения. |
| лево | double | Единица — процентный масштаб ширины области диаграммы. |
| верх | double | Единица — процентный масштаб высоты области диаграммы. |
| право | double | Единица — процентный масштаб ширины области диаграммы. |
| низ | double | Единица — процентный масштаб высоты области диаграммы. |
| imageData | byte[] | Если фигура не является изображением или объектом OLE, imageData должно быть null. |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addSignatureLine(int topRow, int leftColumn, SignatureLine signatureLine) {#addSignatureLine-int-int-com.aspose.cells.SignatureLine-}
```
public Picture addSignatureLine(int topRow, int leftColumn, SignatureLine signatureLine)
```


Добавляет Signature Line в рабочий лист.

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | int | Индекс строки в верхнем левом углу. |
| leftColumn | int | Индекс столбца в верхнем левом углу. |
| signatureLine | [SignatureLine](../../com.aspose.cells/signatureline) | Представляет объект линии подписи. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - 
### addSpinner(int topRow, int top, int leftColumn, int left, int height, int width) {#addSpinner-int-int-int-int-int-int-}
```
public Spinner addSpinner(int topRow, int top, int leftColumn, int left, int height, int width)
```


Добавляет Spinner в рабочий лист.

**Example**

```
         //add a spinner
         Spinner spinner = shapes.addSpinner(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | int | Индекс строки в верхнем левом углу. |
| верх | int | Представляет вертикальное смещение Spinner от его левой строки в единице пикселя. |
| leftColumn | int | Индекс столбца в верхнем левом углу. |
| лево | int | Представляет горизонтальное смещение Spinner от его левого столбца в единице пикселя. |
| height | int | Представляет высоту Spinner в единице пикселя. |
| width | int | Представляет ширину Spinner в единице пикселя. |

**Returns:**
[Spinner](../../com.aspose.cells/spinner) - A Spinner object.
### addSvg(int topRow, int top, int leftColumn, int left, int height, int width, byte[] svgData, byte[] compatibleImageData) {#addSvg-int-int-int-int-int-int-byte---byte---}
```
public Picture addSvg(int topRow, int top, int leftColumn, int left, int height, int width, byte[] svgData, byte[] compatibleImageData)
```


Добавляет svg изображение.

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | int | Индекс строки в верхнем левом углу. |
| верх | int | Представляет вертикальное смещение shape от его левой строки, в пикселях. |
| leftColumn | int | Индекс столбца в верхнем левом углу. |
| лево | int | Горизонтальное смещение shape от его левого столбца, в пикселях. |
| height | int | Высота shape, в пикселях. |
| width | int | Ширина shape, в пикселях. |
| svgData | byte[] | Данные изображения svg. |
| compatibleImageData | byte[] | Преобразованные данные изображения из svg, чтобы быть совместимыми с Excel 2016 или более ранними версиями. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - 
### addTextBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addTextBox-int-int-int-int-int-int-}
```
public TextBox addTextBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Добавляет текстовое поле в рабочий лист.

**Example**

```
         //add a TextBox
         TextBox textBox = shapes.addTextBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | int | Индекс строки в верхнем левом углу. |
| верх | int | Представляет вертикальное смещение textbox от его верхней строки в единице пикселя. |
| leftColumn | int | Индекс столбца в верхнем левом углу. |
| лево | int | Представляет горизонтальное смещение textbox от его левого столбца, в единицах пикселя. |
| height | int | Представляет высоту текстового поля, в единице пикселя. |
| width | int | Представляет ширину текстового поля, в единице пикселя. |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - A [TextBox](../../com.aspose.cells/textbox) object.
### addTextBoxInChart(int top, int left, int height, int width) {#addTextBoxInChart-int-int-int-int-}
```
public TextBox addTextBoxInChart(int top, int left, int height, int width)
```


Добавляет текстовое поле в диаграмму.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| верх | int | Представляет вертикальное смещение textbox от верхнего левого угла в единицах 1/4000 области диаграммы. |
| лево | int | Представляет вертикальное смещение textbox от верхнего левого угла в единицах 1/4000 области диаграммы. |
| height | int | Представляет высоту textbox, в единицах 1/4000 области диаграммы. |
| width | int | Представляет ширину textbox, в единицах 1/4000 области диаграммы. |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - A TextBox object.
### addTextEffect(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int topRow, int top, int leftColumn, int left, int height, int width) {#addTextEffect-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-int-int-}
```
public Shape addTextEffect(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int topRow, int top, int leftColumn, int left, int height, int width)
```


Вставляет объект WordArt.

**Example**

```
         //add a WordArt
         Shape wordArt1 = shapes.addTextEffect(MsoPresetTextEffect.TEXT_EFFECT_10, "WordArt", "arial", 18, false, false, 3, 0, 3, 0, 200, 50);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| effect | int | [MsoPresetTextEffect](../../com.aspose.cells/msopresettexteffect). Тип предустановленного текстового эффекта mso. |
| текст | java.lang.String | Текст WordArt. |
| fontName | java.lang.String | Имя шрифта. |
| size | int | Размер шрифта |
| fontBold | boolean | Указывает, является ли шрифт полужирным. |
| fontItalic | boolean | Указывает, является ли шрифт курсивом. |
| topRow | int | Индекс строки в верхнем левом углу. |
| верх | int | Представляет вертикальное смещение shape от его левой строки, в пикселях. |
| leftColumn | int | Индекс столбца в верхнем левом углу. |
| лево | int | Представляет горизонтальное смещение фигуры от её левого столбца, в единице пикселя. |
| height | int | Представляет высоту фигуры в пикселях. |
| width | int | Представляет ширину фигуры, в единице пикселя. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - Returns a Shape object that represents the new WordArt object.
### addTextEffectInChart(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int top, int left, int height, int width) {#addTextEffectInChart-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-}
```
public Shape addTextEffectInChart(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int top, int left, int height, int width)
```


Вставляет объект WordArt в диаграмму.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| effect | int | [MsoPresetTextEffect](../../com.aspose.cells/msopresettexteffect). Тип предустановленного текстового эффекта mso. |
| текст | java.lang.String | Текст WordArt. |
| fontName | java.lang.String | Имя шрифта. |
| size | int | Размер шрифта |
| fontBold | boolean | Указывает, является ли шрифт полужирным. |
| fontItalic | boolean | Указывает, является ли шрифт курсивом. |
| верх | int | Представляет вертикальное смещение фигуры от верхнего левого угла в единицах 1/4000 области диаграммы. |
| лево | int | Представляет вертикальное смещение фигуры от верхнего левого угла в единицах 1/4000 области диаграммы. |
| height | int | Представляет высоту фигуры, в единицах 1/4000 области диаграммы. |
| width | int | Представляет ширину фигуры, в единицах 1/4000 области диаграммы. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - Returns a Shape object that represents the new WordArt object.
### addWordArt(int style, String text, int topRow, int top, int leftColumn, int left, int height, int width) {#addWordArt-int-java.lang.String-int-int-int-int-int-int-}
```
public Shape addWordArt(int style, String text, int topRow, int top, int leftColumn, int left, int height, int width)
```


Добавляет предустановленный WordArt, начиная с Excel 2007.

**Example**

```
         //add a WordArt
         Shape wordArt2 = shapes.addWordArt(PresetWordArtStyle.WORD_ART_STYLE_1, "WordArt", 3, 0, 3, 0, 50, 200);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). Предустановленный стиль WordArt. |
| текст | java.lang.String | Текст. |
| topRow | int | Индекс строки в верхнем левом углу. |
| верх | int | Представляет вертикальное смещение shape от его левой строки, в пикселях. |
| leftColumn | int | Индекс столбца в верхнем левом углу. |
| лево | int | Представляет горизонтальное смещение фигуры от её левого столбца, в единице пикселя. |
| height | int | Представляет высоту фигуры в пикселях. |
| width | int | Представляет ширину фигуры, в единице пикселя. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### clear() {#clear--}
```
public void clear()
```


Очистить все фигуры в рабочем листе.

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


Возвращает, содержит ли экземпляр этот объект

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| o | java.lang.Object | тестовый объект |

**Returns:**
boolean — содержит ли экземпляр этот объект
### copyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn) {#copyCommentsInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-}
```
public void copyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn)
```


Скопировать все комментарии в диапазоне.

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| shapes | [ShapeCollection](../../com.aspose.cells/shapecollection) | Исходные фигуры. |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Исходный диапазон. |
| destRow | int | Начальная строка целевого диапазона. |
| destColumn | int | Начальный столбец целевого диапазона. |

### copyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, boolean isContained) {#copyInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-boolean-}
```
public void copyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, boolean isContained)
```


Скопировать фигуры в диапазоне в целевой диапазон.

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceShapes | [ShapeCollection](../../com.aspose.cells/shapecollection) | Исходные фигуры. |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Исходный диапазон. |
| destRow | int | Индекс строки целевого диапазона. |
| destColumn | int | Столбец целевого диапазона. |
| isContained | boolean | Определяет, копировать только фигуры, находящиеся в диапазоне. Если true, копирует только фигуры в диапазоне. В противном случае работает как MS Office. |

### deleteInRange(CellArea ca) {#deleteInRange-com.aspose.cells.CellArea-}
```
public void deleteInRange(CellArea ca)
```


Удалить фигуры в диапазоне. Фигуры комментариев не будут удалены.

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Диапазон. Если фигуры находятся в диапазоне, они будут удалены. |

### deleteShape(Shape shape) {#deleteShape-com.aspose.cells.Shape-}
```
public void deleteShape(Shape shape)
```


Удалить фигуру. Если фигура находится в группе или является фигурой‑комментарием, она не будет удалена.

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| shape | [Shape](../../com.aspose.cells/shape) |  |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### find(String what, int previous, FindOptions findOptions) {#find-java.lang.String-int-com.aspose.cells.FindOptions-}
```
public int find(String what, int previous, FindOptions findOptions)
```


Найти фигуру по тексту.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| что | java.lang.String | Текст для поиска. |
| предыдущий | int | Индекс предыдущей фигуры, содержащей тот же текст. -1, если поиск начинается с начала. |
| findOptions | [FindOptions](../../com.aspose.cells/findoptions) | Параметры поиска |

**Returns:**
int — Индекс найденной фигуры, -1 если фигура не найдена.
### get(int index) {#get-int-}
```
public Shape get(int index)
```


Получает объект [Shape](../../com.aspose.cells/shape) по конкретному индексу в списке.

**Example**

```
         //get the first shape
         Shape shape = shapes.get(0);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Индекс. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### get(String name) {#get-java.lang.String-}
```
public Shape get(String name)
```


Получает объект [Shape](../../com.aspose.cells/shape) по имени фигуры.

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| name | java.lang.String | Имя фигуры. |

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


Получает количество элементов, содержащихся в экземпляре CollectionBase.

**Returns:**
int — количество элементов, содержащихся в экземпляре CollectionBase.
### group(Shape[] groupItems) {#group-com.aspose.cells.Shape---}
```
public GroupShape group(Shape[] groupItems)
```


Группировать фигуры.

**Remarks**

Фигура в groupItems не должна быть сгруппирована. Фигура должна находиться в этой коллекции Shapes.

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| groupItems | [Shape\[\]](../../com.aspose.cells/shape) | элементы группы. |

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


Определяет индекс конкретного элемента в экземпляре CollectionBase.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| o | java.lang.Object | Определяет индекс конкретного элемента в экземпляре CollectionBase. |

**Returns:**
int — индекс значения, если оно найдено в списке; иначе -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Возвращает перечислитель, который проходит по экземпляру CollectionBase.

**Returns:**
java.util.Iterator — итератор для экземпляра CollectionBase.
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


Удалить фигуру.

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| shape | [Shape](../../com.aspose.cells/shape) |  |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Удалить фигуру.

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | int | Индекс фигуры. |

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


Разгруппировать элементы фигур.

**Remarks**

Если групповая фигура сгруппирована другой групповой фигурой, ничего не будет сделано.

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| group | [GroupShape](../../com.aspose.cells/groupshape) | Групповая фигура. |

### updateSelectedValue() {#updateSelectedValue--}
```
public void updateSelectedValue()
```


Обновить выбранное значение значением связанной ячейки или диапазона фигуры.

### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

