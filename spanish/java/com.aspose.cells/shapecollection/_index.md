---
title: "ShapeCollection"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa todas las formas en una hoja de cálculo/gráfico."
type: docs
url: /es/java/com.aspose.cells/shapecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ShapeCollection extends CollectionBase
```

Representa todas las formas en una hoja de cálculo/gráfico.

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
## Métodos

| Método | Descripción |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Agrega un elemento a la instancia de CollectionBase. |
| [addActiveXControl(int type, int topRow, int top, int leftColumn, int left, int width, int height)](#addActiveXControl-int-int-int-int-int-int-int-) | Crea un control Activex. |
| [addArc(int topRow, int top, int leftColumn, int left, int height, int width)](#addArc-int-int-int-int-int-int-) | Añade un ArcShape a la hoja de cálculo. |
| [addAutoShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)](#addAutoShape-int-int-int-int-int-int-int-) | Añade un AutoShape a la hoja de cálculo. |
| [addAutoShapeInChart(int type, int top, int left, int height, int width)](#addAutoShapeInChart-int-int-int-int-int-) | Añade un AutoShape al gráfico. |
| [addButton(int topRow, int top, int leftColumn, int left, int height, int width)](#addButton-int-int-int-int-int-int-) | Añade un Button a la hoja de cálculo. |
| [addCheckBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addCheckBox-int-int-int-int-int-int-) | Añade una casilla de verificación a la hoja de cálculo. |
| [addComboBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addComboBox-int-int-int-int-int-int-) | Añade un ComboBox a la hoja de cálculo. |
| [addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left)](#addCopy-com.aspose.cells.Shape-int-int-int-int-) | Añade y copia una forma a la hoja de cálculo. |
| [addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left, CopyOptions copyOptions)](#addCopy-com.aspose.cells.Shape-int-int-int-int-com.aspose.cells.CopyOptions-) | Añade y copia una forma a la hoja de cálculo. |
| [addEquation(int topRow, int top, int leftColumn, int left, int height, int width)](#addEquation-int-int-int-int-int-int-) | Añade un objeto de ecuación a la hoja de cálculo. |
| [addFreeFloatingShape(int type, int top, int left, int height, int width, byte[] imageData, boolean isOriginalSize)](#addFreeFloatingShape-int-int-int-int-int-byte---boolean-) | Añade una forma flotante libre a la hoja de cálculo. Solo se aplica a formas de línea/imagen. |
| [addFreeform(int topRow, int top, int leftColumn, int left, int height, int width, ShapePath[] paths)](#addFreeform-int-int-int-int-int-int-com.aspose.cells.ShapePath---) | Añade una forma libre a la hoja de cálculo. |
| [addGroupBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addGroupBox-int-int-int-int-int-int-) | Añade un GroupBox a la hoja de cálculo. |
| [addIcons(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageByteData, byte[] compatibleImageData)](#addIcons-int-int-int-int-int-int-byte---byte---) | Añade una imagen svg. |
| [addLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, int width, String latex)](#addLaTeXEquation-int-int-int-int-int-int-java.lang.String-) | Añade un objeto de ecuación a la hoja de cálculo usando cadenas con formato LaTeX. |
| [addLabel(int topRow, int top, int leftColumn, int left, int height, int width)](#addLabel-int-int-int-int-int-int-) | Añade una Label a la hoja de cálculo. |
| [addLabelInChart(int top, int left, int height, int width)](#addLabelInChart-int-int-int-int-) | Añade una etiqueta al gráfico. |
| [addLine(int topRow, int top, int leftColumn, int left, int height, int width)](#addLine-int-int-int-int-int-int-) | Añade un LineShape a la hoja de cálculo. |
| [addLinkedPicture(int topRow, int leftColumn, int height, int width, String sourceFullName)](#addLinkedPicture-int-int-int-int-java.lang.String-) | Añade una imagen vinculada. |
| [addListBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addListBox-int-int-int-int-int-int-) | Añade un ListBox a la hoja de cálculo. |
| [addOleObject(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageData)](#addOleObject-int-int-int-int-int-int-byte---) | Añade un OleObject. |
| [addOleObjectWithLinkedImage(int topRow, int leftColumn, int height, int width, String sourceFullName)](#addOleObjectWithLinkedImage-int-int-int-int-java.lang.String-) | Añade una imagen vinculada. |
| [addOval(int topRow, int top, int leftColumn, int left, int height, int width)](#addOval-int-int-int-int-int-int-) | Añade un Oval a la hoja de cálculo. |
| [addPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream)](#addPicture-int-int-int-int-java.io.InputStream-) | Añade una imagen a la colección. |
| [addPicture(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale)](#addPicture-int-int-java.io.InputStream-int-int-) | Añade una imagen a la colección. |
| [addPictureInChart(int top, int left, InputStream stream, int widthScale, int heightScale)](#addPictureInChart-int-int-java.io.InputStream-int-int-) | Añade una imagen al gráfico. |
| [addRadioButton(int topRow, int top, int leftColumn, int left, int height, int width)](#addRadioButton-int-int-int-int-int-int-) | Añade un RadioButton a la hoja de cálculo. |
| [addRectangle(int topRow, int top, int leftColumn, int left, int height, int width)](#addRectangle-int-int-int-int-int-int-) | Agrega un RectangleShape a la hoja de cálculo. |
| [addScrollBar(int topRow, int top, int leftColumn, int left, int height, int width)](#addScrollBar-int-int-int-int-int-int-) | Agrega una ScrollBar a la hoja de cálculo. |
| [addShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)](#addShape-int-int-int-int-int-int-int-) | Agrega una Shape a la hoja de cálculo. |
| [addShapeInChart(int type, int placement, int left, int top, int right, int bottom)](#addShapeInChart-int-int-int-int-int-int-) | Agrega una forma al gráfico. Todas las unidades son 1/4000 del área del gráfico. |
| [addShapeInChart(int type, int placement, int left, int top, int right, int bottom, byte[] imageData)](#addShapeInChart-int-int-int-int-int-int-byte---) | Agrega una forma al gráfico. Todas las unidades son 1/4000 del área del gráfico. |
| [addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom)](#addShapeInChartByScale-int-int-double-double-double-double-) | Agrega una forma al gráfico. |
| [addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom, byte[] imageData)](#addShapeInChartByScale-int-int-double-double-double-double-byte---) | Agrega una forma al gráfico. Todas las unidades son 1/4000 del área del gráfico. |
| [addSignatureLine(int topRow, int leftColumn, SignatureLine signatureLine)](#addSignatureLine-int-int-com.aspose.cells.SignatureLine-) | Agrega una línea de firma a la hoja de cálculo. |
| [addSpinner(int topRow, int top, int leftColumn, int left, int height, int width)](#addSpinner-int-int-int-int-int-int-) | Agrega un Spinner a la hoja de cálculo. |
| [addSvg(int topRow, int top, int leftColumn, int left, int height, int width, byte[] svgData, byte[] compatibleImageData)](#addSvg-int-int-int-int-int-int-byte---byte---) | Añade una imagen svg. |
| [addTextBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addTextBox-int-int-int-int-int-int-) | Agrega un cuadro de texto a la hoja de cálculo. |
| [addTextBoxInChart(int top, int left, int height, int width)](#addTextBoxInChart-int-int-int-int-) | Agrega un cuadro de texto al gráfico. |
| [addTextEffect(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int topRow, int top, int leftColumn, int left, int height, int width)](#addTextEffect-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-int-int-) | Inserta un objeto WordArt. |
| [addTextEffectInChart(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int top, int left, int height, int width)](#addTextEffectInChart-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-) | Inserta un objeto WordArt al gráfico |
| [addWordArt(int style, String text, int topRow, int top, int leftColumn, int left, int height, int width)](#addWordArt-int-java.lang.String-int-int-int-int-int-int-) | Agrega WordArt predefinido desde Excel 2007. |
| [clear()](#clear--) | Elimina todas las formas en la hoja de cálculo. |
| [contains(Object o)](#contains-java.lang.Object-) | Devuelve si la instancia contiene este objeto |
| [copyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn)](#copyCommentsInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-) | Copia todos los comentarios en el rango. |
| [copyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, boolean isContained)](#copyInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-boolean-) | Copia las formas del rango al rango de destino. |
| [deleteInRange(CellArea ca)](#deleteInRange-com.aspose.cells.CellArea-) | Elimina las formas en el rango. Las formas de comentario no se eliminarán. |
| [deleteShape(Shape shape)](#deleteShape-com.aspose.cells.Shape-) | Elimina una forma. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [find(String what, int previous, FindOptions findOptions)](#find-java.lang.String-int-com.aspose.cells.FindOptions-) | Buscar forma por texto |
| [get(int index)](#get-int-) | Obtiene el objeto [Shape](../../com.aspose.cells/shape) en el índice específico de la lista. |
| [get(String name)](#get-java.lang.String-) | Obtiene el objeto [Shape](../../com.aspose.cells/shape) por el nombre de la forma. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtiene el número de elementos contenidos en la instancia de CollectionBase. |
| [group(Shape[] groupItems)](#group-com.aspose.cells.Shape---) | Agrupa las formas. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determina el índice de un elemento específico en la instancia de CollectionBase. |
| [iterator()](#iterator--) | Devuelve un enumerador que recorre la instancia de CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Shape shape)](#remove-com.aspose.cells.Shape-) | Elimina la forma. |
| [removeAt(int index)](#removeAt-int-) | Elimina la forma. |
| [toString()](#toString--) |  |
| [ungroup(GroupShape group)](#ungroup-com.aspose.cells.GroupShape-) | Desagrupa los elementos de forma. |
| [updateSelectedValue()](#updateSelectedValue--) | Actualiza el valor seleccionado con el valor de la celda vinculada o del rango de la forma. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Agrega un elemento a la instancia de CollectionBase.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| o | java.lang.Object | El objeto a agregar a la instancia de CollectionBase. |

**Returns:**
int - La posición en la que se insertó el nuevo elemento.
### addActiveXControl(int type, int topRow, int top, int leftColumn, int left, int width, int height) {#addActiveXControl-int-int-int-int-int-int-int-}
```
public Shape addActiveXControl(int type, int topRow, int top, int leftColumn, int left, int width, int height)
```


Crea un control Activex.

**Example**

```
         //add an ActiveX control
         Shape activeXControl = shapes.addActiveXControl(com.aspose.cells.ControlType.CHECK_BOX, 1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [ControlType](../../com.aspose.cells/controltype). El tipo del control. |
| topRow | int | Índice de fila superior izquierda. |
| superior | int | Representa el desplazamiento vertical de Shape desde su fila izquierda, en unidad de píxel. |
| leftColumn | int | Índice de columna superior izquierda. |
| izquierda | int | Representa el desplazamiento horizontal de Shape desde su columna izquierda, en unidad de píxel. |
| ancho | int | Representa el ancho de Shape, en unidad de píxel. |
| altura | int | Representa la altura de Shape, en unidad de píxel. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### addArc(int topRow, int top, int leftColumn, int left, int height, int width) {#addArc-int-int-int-int-int-int-}
```
public ArcShape addArc(int topRow, int top, int leftColumn, int left, int height, int width)
```


Añade un ArcShape a la hoja de cálculo.

**Example**

```
         //add a arc
         ArcShape arcShape = shapes.addArc(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int | Índice de fila superior izquierda. |
| superior | int | Representa el desplazamiento vertical de ArcShape desde su fila izquierda, en unidad de píxel. |
| leftColumn | int | Índice de columna superior izquierda. |
| izquierda | int | Representa el desplazamiento horizontal de ArcShape desde su columna izquierda, en unidad de píxel. |
| altura | int | Representa la altura de ArcShape, en unidad de píxel. |
| ancho | int | Representa el ancho de ArcShape, en unidad de píxel. |

**Returns:**
[ArcShape](../../com.aspose.cells/arcshape) - A ArcShape object.
### addAutoShape(int type, int topRow, int top, int leftColumn, int left, int height, int width) {#addAutoShape-int-int-int-int-int-int-int-}
```
public Shape addAutoShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)
```


Añade un AutoShape a la hoja de cálculo.

**Remarks**

El tipo no pudo ser Chart/Comment/Picture/OleObject/Polygon/DialogBox

**Example**

```
         //Adds a AutoShape to the worksheet.
         Shape autoShape = shapes.addAutoShape(AutoShapeType.CUBE, 1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [AutoShapeType](../../com.aspose.cells/autoshapetype). Tipo de forma automática. |
| topRow | int | Índice de fila superior izquierda. |
| superior | int | Representa el desplazamiento vertical de Shape desde su fila izquierda, en unidad de píxel. |
| leftColumn | int | Índice de columna superior izquierda. |
| izquierda | int | Representa el desplazamiento horizontal de Shape desde su columna izquierda, en unidad de píxel. |
| altura | int | Representa la altura de Shape, en unidad de píxel. |
| ancho | int | Representa el ancho de Shape, en unidad de píxel. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - A Shape object.
### addAutoShapeInChart(int type, int top, int left, int height, int width) {#addAutoShapeInChart-int-int-int-int-int-}
```
public Shape addAutoShapeInChart(int type, int top, int left, int height, int width)
```


Añade un AutoShape al gráfico.

**Remarks**

El tipo no pudo ser Chart/Comment/Picture/OleObject/Polygon/DialogBox

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [AutoShapeType](../../com.aspose.cells/autoshapetype). Tipo de forma automática. |
| superior | int | Representa el desplazamiento vertical de textbox desde la esquina superior izquierda en unidades de 1/4000 del área del gráfico. |
| izquierda | int | Representa el desplazamiento vertical de textbox desde la esquina superior izquierda en unidades de 1/4000 del área del gráfico. |
| altura | int | Representa la altura de textbox, en unidades de 1/4000 del área del gráfico. |
| ancho | int | Representa el ancho de textbox, en unidades de 1/4000 del área del gráfico. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - Returns a shape object.
### addButton(int topRow, int top, int leftColumn, int left, int height, int width) {#addButton-int-int-int-int-int-int-}
```
public Button addButton(int topRow, int top, int leftColumn, int left, int height, int width)
```


Añade un Button a la hoja de cálculo.

**Example**

```
         //add a button
         Button button = shapes.addButton(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int | Índice de fila superior izquierda. |
| superior | int | Representa el desplazamiento vertical de Button desde su fila izquierda, en unidad de píxel. |
| leftColumn | int | Índice de columna superior izquierda. |
| izquierda | int | Representa el desplazamiento horizontal de Button desde su columna izquierda, en unidad de píxel. |
| altura | int | Representa la altura de Button, en unidad de píxel. |
| ancho | int | Representa el ancho de Button, en unidad de píxel. |

**Returns:**
[Button](../../com.aspose.cells/button) - A Button object.
### addCheckBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addCheckBox-int-int-int-int-int-int-}
```
public CheckBox addCheckBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Añade una casilla de verificación a la hoja de cálculo.

**Example**

```
         //add a CheckBox
         CheckBox checkBox = shapes.addCheckBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int | Índice de fila superior izquierda. |
| superior | int | Representa el desplazamiento vertical de checkbox desde su fila superior, en unidad de píxel. |
| leftColumn | int | Índice de columna superior izquierda. |
| izquierda | int | Representa el desplazamiento horizontal de textbox desde su columna izquierda, en unidad de píxel. |
| altura | int | Altura de textbox, en unidad de píxel. |
| ancho | int | Ancho de textbox, en unidad de píxel. |

**Returns:**
[CheckBox](../../com.aspose.cells/checkbox) - The new CheckBox object index.
### addComboBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addComboBox-int-int-int-int-int-int-}
```
public ComboBox addComboBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Añade un ComboBox a la hoja de cálculo.

**Example**

```
         //add a combo box
         ComboBox comboBox = shapes.addComboBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int | Índice de fila superior izquierda. |
| superior | int | Representa el desplazamiento vertical de ComboBox desde su fila izquierda, en unidad de píxel. |
| leftColumn | int | Índice de columna superior izquierda. |
| izquierda | int | Representa el desplazamiento horizontal de ComboBox desde su columna izquierda, en unidad de píxel. |
| altura | int | Representa la altura del ComboBox, en unidades de píxel. |
| ancho | int | Representa el ancho del ComboBox, en unidades de píxel. |

**Returns:**
[ComboBox](../../com.aspose.cells/combobox) - A ComboBox object.
### addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left) {#addCopy-com.aspose.cells.Shape-int-int-int-int-}
```
public Shape addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left)
```


Añade y copia una forma a la hoja de cálculo.

**Example**

```
         //add a shape
         RectangleShape rectangle = shapes.addRectangle(2, 0, 2, 0, 130, 130);
         //Adds and copies a shape.
         shapes.addCopy(rectangle, 7, 0, 7, 0);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceShape | [Shape](../../com.aspose.cells/shape) | Forma de origen. |
| topRow | int | El índice de la fila superior. |
| superior | int | Representa el desplazamiento vertical desde su fila superior, en unidades de píxel. |
| leftColumn | int | El índice de la columna izquierda. |
| izquierda | int | Representa el desplazamiento horizontal desde su columna izquierda, en unidades de píxel. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - The new [Shape](../../com.aspose.cells/shape) object.
### addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left, CopyOptions copyOptions) {#addCopy-com.aspose.cells.Shape-int-int-int-int-com.aspose.cells.CopyOptions-}
```
public Shape addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left, CopyOptions copyOptions)
```


Añade y copia una forma a la hoja de cálculo.

**Example**

```
         //add a shape
         RectangleShape rectangle = shapes.addRectangle(2, 0, 2, 0, 130, 130);
         //Adds and copies a shape.
         shapes.addCopy(rectangle, 7, 0, 7, 0);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceShape | [Shape](../../com.aspose.cells/shape) | Forma de origen. |
| topRow | int | El índice de la fila superior. |
| superior | int | Representa el desplazamiento vertical desde su fila superior, en unidades de píxel. |
| leftColumn | int | El índice de la columna izquierda. |
| izquierda | int | Representa el desplazamiento horizontal desde su columna izquierda, en unidades de píxel. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | Las opciones de copiar formas. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - The new [Shape](../../com.aspose.cells/shape) object.
### addEquation(int topRow, int top, int leftColumn, int left, int height, int width) {#addEquation-int-int-int-int-int-int-}
```
public TextBox addEquation(int topRow, int top, int leftColumn, int left, int height, int width)
```


Añade un objeto de ecuación a la hoja de cálculo.

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int | El índice de la fila superior. |
| superior | int | El desplazamiento vertical de su fila superior, en unidades de píxel. |
| leftColumn | int | El índice de la columna izquierda. |
| izquierda | int | El desplazamiento horizontal desde su columna izquierda, en unidades de píxel. |
| altura | int | La altura de la ecuación, en unidades de píxel. |
| ancho | int | El ancho de la ecuación, en unidades de píxel. |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - 
### addFreeFloatingShape(int type, int top, int left, int height, int width, byte[] imageData, boolean isOriginalSize) {#addFreeFloatingShape-int-int-int-int-int-byte---boolean-}
```
public Shape addFreeFloatingShape(int type, int top, int left, int height, int width, byte[] imageData, boolean isOriginalSize)
```


Añade una forma flotante libre a la hoja de cálculo. Solo se aplica a formas de línea/imagen.

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). El tipo de forma. |
| superior | int | Representa el desplazamiento vertical de la forma desde la fila superior de la hoja de cálculo, en unidades de píxel. |
| izquierda | int | Representa el desplazamiento horizontal de la forma desde la columna izquierda de la hoja de cálculo, en unidades de píxel. |
| altura | int | Representa la altura de LineShape, en unidades de píxel. |
| ancho | int | Representa el ancho de LineShape, en unidades de píxel. |
| imageData | byte[] | Los datos de la imagen, solo se aplican a la foto. |
| isOriginalSize | boolean | Indica si la forma usa el tamaño original cuando la forma es una imagen. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### addFreeform(int topRow, int top, int leftColumn, int left, int height, int width, ShapePath[] paths) {#addFreeform-int-int-int-int-int-int-com.aspose.cells.ShapePath---}
```
public Shape addFreeform(int topRow, int top, int leftColumn, int left, int height, int width, ShapePath[] paths)
```


Añade una forma libre a la hoja de cálculo.

**Remarks**

Nota: Que el ancho y la altura en los parámetros pueden ser cualquier valor entero positivo, no el ancho y la altura totales del arreglo ShapePath especificado por \\u9225\\u6a96aths'. La relación entre ellos es una relación de escala-relleno, es decir, cada objeto ShapePath se escalará según el ancho y la altura. Por lo tanto, cuando hay varios objetos en 'paths', cada objeto ShapePath debe diseñarse razonablemente para cumplir con las expectativas. Cuando solo hay un objeto ShapePath y no hay otros requisitos, pasar el ancho y la altura del objeto como valores de parámetro \\u9225\\u5b27\\u20ac\\u5a94s es una buena solución.

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int | Índice de fila superior izquierda. |
| superior | int | Representa el desplazamiento vertical de la forma libre desde su fila izquierda, en unidades de píxel. |
| leftColumn | int | Índice de columna superior izquierda. |
| izquierda | int | Representa el desplazamiento horizontal de la forma libre desde su columna izquierda, en unidades de píxel. |
| altura | int | Representa la altura de la forma libre, en unidades de píxel. |
| ancho | int | Representa el ancho de la forma libre, en unidades de píxel. |
| paths | [ShapePath\[\]](../../com.aspose.cells/shapepath) | Representa una ruta definida por el usuario |

**Returns:**
[Shape](../../com.aspose.cells/shape) - A freeform shape.
### addGroupBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addGroupBox-int-int-int-int-int-int-}
```
public GroupBox addGroupBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Añade un GroupBox a la hoja de cálculo.

**Example**

```
         //add a group box
         GroupBox groupBox = shapes.addGroupBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int | Índice de fila superior izquierda. |
| superior | int | Representa el desplazamiento vertical del GroupBox desde su fila izquierda, en unidades de píxel. |
| leftColumn | int | Índice de columna superior izquierda. |
| izquierda | int | Representa el desplazamiento horizontal del GroupBox desde su columna izquierda, en unidades de píxel. |
| altura | int | Representa la altura del GroupBox, en unidades de píxel. |
| ancho | int | Representa el ancho del GroupBox, en unidades de píxel. |

**Returns:**
[GroupBox](../../com.aspose.cells/groupbox) - A GroupBox object.
### addIcons(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageByteData, byte[] compatibleImageData) {#addIcons-int-int-int-int-int-int-byte---byte---}
```
public Picture addIcons(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageByteData, byte[] compatibleImageData)
```


Añade una imagen svg.

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int | Índice de fila superior izquierda. |
| superior | int | Representa el desplazamiento vertical de la forma desde su fila izquierda, en unidades de píxel. |
| leftColumn | int | Índice de columna superior izquierda. |
| izquierda | int | El desplazamiento horizontal de la forma desde su columna izquierda, en unidades de píxel. |
| altura | int | La altura de la forma, en unidades de píxel. |
| ancho | int | El ancho de la forma, en unidades de píxel. |
| imageByteData | byte[] | Los datos de bytes de la imagen. |
| compatibleImageData | byte[] | Datos de imagen convertidos desde SVG para ser compatibles con Excel 2016 o versiones anteriores. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - 
### addLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, int width, String latex) {#addLaTeXEquation-int-int-int-int-int-int-java.lang.String-}
```
public TextBox addLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, int width, String latex)
```


Añade un objeto de ecuación a la hoja de cálculo usando cadenas con formato LaTeX.

**Example**

```
         // LaTeX format string.
         String latex = "\\alpha +  \\frac{\\partial^2}{\\partial x_1\\partial x_2}y - \\left ( a + b \\right )+_{a}^{b}\\beta";
         // Adds an equation object to the worksheet.
         TextBox textBox = shapes.addLaTeXEquation(1, 0, 1, 0, 100, 300, latex);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int | El índice de la fila superior. |
| superior | int | El desplazamiento vertical de su fila superior, en unidades de píxel. |
| leftColumn | int | El índice de la columna izquierda. |
| izquierda | int | El desplazamiento horizontal desde su columna izquierda, en unidades de píxel. |
| altura | int | La altura de la ecuación, en unidades de píxel. |
| ancho | int | El ancho de la ecuación, en unidades de píxel. |
| latex | java.lang.String | Cadena de formato LaTeX |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - 
### addLabel(int topRow, int top, int leftColumn, int left, int height, int width) {#addLabel-int-int-int-int-int-int-}
```
public Label addLabel(int topRow, int top, int leftColumn, int left, int height, int width)
```


Añade una Label a la hoja de cálculo.

**Example**

```
         //add a label
         Label label = shapes.addLabel(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int | Índice de fila superior izquierda. |
| superior | int | Representa el desplazamiento vertical del Label desde su fila izquierda, en unidades de píxel. |
| leftColumn | int | Índice de columna superior izquierda. |
| izquierda | int | Representa el desplazamiento horizontal del Label desde su columna izquierda, en unidades de píxel. |
| altura | int | Representa la altura del Label, en unidades de píxel. |
| ancho | int | Representa el ancho del Label, en unidades de píxel. |

**Returns:**
[Label](../../com.aspose.cells/label) - A Label object.
### addLabelInChart(int top, int left, int height, int width) {#addLabelInChart-int-int-int-int-}
```
public Label addLabelInChart(int top, int left, int height, int width)
```


Añade una etiqueta al gráfico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| superior | int | Representa el desplazamiento vertical de la etiqueta desde la esquina superior izquierda en unidades de 1/4000 del área del gráfico. |
| izquierda | int | Representa el desplazamiento vertical de la etiqueta desde la esquina superior izquierda en unidades de 1/4000 del área del gráfico. |
| altura | int | Representa la altura de la etiqueta, en unidades de 1/4000 del área del gráfico. |
| ancho | int | Representa el ancho de la etiqueta, en unidades de 1/4000 del área del gráfico. |

**Returns:**
[Label](../../com.aspose.cells/label) - A new Label object.
### addLine(int topRow, int top, int leftColumn, int left, int height, int width) {#addLine-int-int-int-int-int-int-}
```
public LineShape addLine(int topRow, int top, int leftColumn, int left, int height, int width)
```


Añade un LineShape a la hoja de cálculo.

**Example**

```
         // add a line object
         LineShape lineShape = shapes.addLine(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int | Índice de fila superior izquierda. |
| superior | int | Representa el desplazamiento vertical del LineShape desde su fila izquierda, en unidades de píxel. |
| leftColumn | int | Índice de columna superior izquierda. |
| izquierda | int | Representa el desplazamiento horizontal del LineShape desde su columna izquierda, en unidades de píxel. |
| altura | int | Representa la altura de LineShape, en unidades de píxel. |
| ancho | int | Representa el ancho de LineShape, en unidades de píxel. |

**Returns:**
[LineShape](../../com.aspose.cells/lineshape) - A LineShape object.
### addLinkedPicture(int topRow, int leftColumn, int height, int width, String sourceFullName) {#addLinkedPicture-int-int-int-int-java.lang.String-}
```
public Picture addLinkedPicture(int topRow, int leftColumn, int height, int width, String sourceFullName)
```


Añade una imagen vinculada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int | Índice de fila superior izquierda. |
| leftColumn | int | Índice de columna superior izquierda. |
| altura | int | La altura de la forma. En unidades de píxeles |
| ancho | int | El ancho de la forma. En unidades de píxeles |
| sourceFullName | java.lang.String | La ruta y el nombre del archivo fuente para la imagen vinculada |

**Returns:**
[Picture](../../com.aspose.cells/picture) - [Picture](../../com.aspose.cells/picture) Picture object.
### addListBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addListBox-int-int-int-int-int-int-}
```
public ListBox addListBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Añade un ListBox a la hoja de cálculo.

**Example**

```
         //add a list box
         ListBox listBox = shapes.addListBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int | Índice de fila superior izquierda. |
| superior | int | Representa el desplazamiento vertical de ListBox desde su fila izquierda, en unidad de píxel. |
| leftColumn | int | Índice de columna superior izquierda. |
| izquierda | int | Representa el desplazamiento horizontal de ListBox desde su columna izquierda, en unidad de píxel. |
| altura | int | Representa la altura de ListBox, en unidad de píxel. |
| ancho | int | Representa el ancho de ListBox, en unidad de píxel. |

**Returns:**
[ListBox](../../com.aspose.cells/listbox) - A ListBox object.
### addOleObject(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageData) {#addOleObject-int-int-int-int-int-int-byte---}
```
public OleObject addOleObject(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageData)
```


Añade un OleObject.

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int |  |
| superior | int |  |
| leftColumn | int |  |
| izquierda | int |  |
| altura | int |  |
| ancho | int |  |
| imageData | byte[] |  |

**Returns:**
[OleObject](../../com.aspose.cells/oleobject) - 
### addOleObjectWithLinkedImage(int topRow, int leftColumn, int height, int width, String sourceFullName) {#addOleObjectWithLinkedImage-int-int-int-int-java.lang.String-}
```
public OleObject addOleObjectWithLinkedImage(int topRow, int leftColumn, int height, int width, String sourceFullName)
```


Añade una imagen vinculada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int | Índice de fila superior izquierda. |
| leftColumn | int | Índice de columna superior izquierda. |
| altura | int | La altura de la forma. En unidades de píxeles |
| ancho | int | El ancho de la forma. En unidades de píxeles |
| sourceFullName | java.lang.String | La ruta y el nombre del archivo fuente para la imagen vinculada |

**Returns:**
[OleObject](../../com.aspose.cells/oleobject) - [Picture](../../com.aspose.cells/picture) Picture object.
### addOval(int topRow, int top, int leftColumn, int left, int height, int width) {#addOval-int-int-int-int-int-int-}
```
public Oval addOval(int topRow, int top, int leftColumn, int left, int height, int width)
```


Añade un Oval a la hoja de cálculo.

**Example**

```
         //add a oval
         Oval oval = shapes.addOval(1, 0, 1, 0, 50, 50);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int | Índice de fila superior izquierda. |
| superior | int | Representa el desplazamiento vertical de Oval desde su fila izquierda, en unidad de píxel. |
| leftColumn | int | Índice de columna superior izquierda. |
| izquierda | int | Representa el desplazamiento horizontal de Oval desde su columna izquierda, en unidad de píxel. |
| altura | int | Representa la altura de Oval, en unidad de píxel. |
| ancho | int | Representa el ancho de Oval, en unidad de píxel. |

**Returns:**
[Oval](../../com.aspose.cells/oval) - A Oval object.
### addPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream) {#addPicture-int-int-int-int-java.io.InputStream-}
```
public Picture addPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream)
```


Añade una imagen a la colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int | Índice de fila superior izquierda. |
| leftColumn | int | Índice de columna superior izquierda. |
| bottomRow | int | Índice de fila inferior derecha |
| rightColumn | int | Índice de columna inferior derecha |
| stream | java.io.InputStream | Objeto de flujo que contiene los datos de la imagen. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - [Picture](../../com.aspose.cells/picture) Picture object.
### addPicture(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale) {#addPicture-int-int-java.io.InputStream-int-int-}
```
public Picture addPicture(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale)
```


Añade una imagen a la colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int | Índice de fila superior izquierda. |
| leftColumn | int | Índice de columna superior izquierda. |
| stream | java.io.InputStream | Objeto de flujo que contiene los datos de la imagen. |
| widthScale | int | Escala del ancho de la imagen, en porcentaje. |
| heightScale | int | Escala de la altura de la imagen, en porcentaje. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - [Picture](../../com.aspose.cells/picture) Picture object.
### addPictureInChart(int top, int left, InputStream stream, int widthScale, int heightScale) {#addPictureInChart-int-int-java.io.InputStream-int-int-}
```
public Picture addPictureInChart(int top, int left, InputStream stream, int widthScale, int heightScale)
```


Añade una imagen al gráfico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| superior | int | Representa el desplazamiento vertical de la forma desde la esquina superior izquierda en unidades de 1/4000 del área del gráfico. |
| izquierda | int | Representa el desplazamiento horizontal de la forma desde la esquina superior izquierda en unidades de 1/4000 del área del gráfico. |
| stream | java.io.InputStream | Objeto de flujo que contiene los datos de la imagen. |
| widthScale | int | Escala del ancho de la imagen, en porcentaje. |
| heightScale | int | Escala de la altura de la imagen, en porcentaje. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns a Picture object.
### addRadioButton(int topRow, int top, int leftColumn, int left, int height, int width) {#addRadioButton-int-int-int-int-int-int-}
```
public RadioButton addRadioButton(int topRow, int top, int leftColumn, int left, int height, int width)
```


Añade un RadioButton a la hoja de cálculo.

**Example**

```
         //add a radio button
         RadioButton radioButton = shapes.addRadioButton(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int | Índice de fila superior izquierda. |
| superior | int | Representa el desplazamiento vertical de RadioButton desde su fila izquierda, en unidad de píxel. |
| leftColumn | int | Índice de columna superior izquierda. |
| izquierda | int | Representa el desplazamiento horizontal de RadioButton desde su columna izquierda, en unidad de píxel. |
| altura | int | Representa la altura de RadioButton, en unidad de píxel. |
| ancho | int | Representa el ancho de RadioButton, en unidad de píxel. |

**Returns:**
[RadioButton](../../com.aspose.cells/radiobutton) - A RadioButton object.
### addRectangle(int topRow, int top, int leftColumn, int left, int height, int width) {#addRectangle-int-int-int-int-int-int-}
```
public RectangleShape addRectangle(int topRow, int top, int leftColumn, int left, int height, int width)
```


Agrega un RectangleShape a la hoja de cálculo.

**Example**

```
         // add a rectangle
         RectangleShape rectangleShape = shapes.addRectangle(2, 0, 2, 0, 130, 130);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int | Índice de fila superior izquierda. |
| superior | int | Representa el desplazamiento vertical de RectangleShape desde su fila izquierda, en unidad de píxel. |
| leftColumn | int | Índice de columna superior izquierda. |
| izquierda | int | Representa el desplazamiento horizontal de RectangleShape desde su columna izquierda, en unidad de píxel. |
| altura | int | Representa la altura de RectangleShape, en unidades de píxel. |
| ancho | int | Representa el ancho de RectangleShape, en unidades de píxel. |

**Returns:**
[RectangleShape](../../com.aspose.cells/rectangleshape) - A RectangleShape object.
### addScrollBar(int topRow, int top, int leftColumn, int left, int height, int width) {#addScrollBar-int-int-int-int-int-int-}
```
public ScrollBar addScrollBar(int topRow, int top, int leftColumn, int left, int height, int width)
```


Agrega una ScrollBar a la hoja de cálculo.

**Example**

```
         //add a scroll bar
         ScrollBar scrollBar = shapes.addScrollBar(1, 0, 1, 0, 100, 20);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int | Índice de fila superior izquierda. |
| superior | int | Representa el desplazamiento vertical de ScrollBar desde su fila izquierda, en unidades de píxel. |
| leftColumn | int | Índice de columna superior izquierda. |
| izquierda | int | Representa el desplazamiento horizontal de ScrollBar desde su columna izquierda, en unidades de píxel. |
| altura | int | Representa la altura de ScrollBar, en unidades de píxel. |
| ancho | int | Representa el ancho de ScrollBar, en unidades de píxel. |

**Returns:**
[ScrollBar](../../com.aspose.cells/scrollbar) - A ScrollBar object.
### addShape(int type, int topRow, int top, int leftColumn, int left, int height, int width) {#addShape-int-int-int-int-int-int-int-}
```
public Shape addShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)
```


Agrega una Shape a la hoja de cálculo.

**Remarks**

El tipo no pudo ser Chart/Comment/Picture/OleObject/Polygon/DialogBox

**Example**

```
         //Add a shape of the specified type
         Shape shapeByType = shapes.addShape(MsoDrawingType.CELLS_DRAWING, 1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Tipo de dibujo Mso. |
| topRow | int | Índice de fila superior izquierda. |
| superior | int | Representa el desplazamiento vertical de Shape desde su fila izquierda, en unidad de píxel. |
| leftColumn | int | Índice de columna superior izquierda. |
| izquierda | int | Representa el desplazamiento horizontal de Shape desde su columna izquierda, en unidad de píxel. |
| altura | int | Representa la altura de Shape, en unidad de píxel. |
| ancho | int | Representa el ancho de Shape, en unidad de píxel. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - A Shape object.
### addShapeInChart(int type, int placement, int left, int top, int right, int bottom) {#addShapeInChart-int-int-int-int-int-int-}
```
public Shape addShapeInChart(int type, int placement, int left, int top, int right, int bottom)
```


Agrega una forma al gráfico. Todas las unidades son 1/4000 del área del gráfico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). El tipo de dibujo. |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype). el tipo de colocación. |
| izquierda | int | En unidades de 1/4000 del ancho del área del gráfico. |
| superior | int | En unidades de 1/4000 de la altura del área del gráfico. |
| derecha | int | En unidades de 1/4000 del ancho del área del gráfico. |
| inferior | int | En unidades de 1/4000 de la altura del área del gráfico. |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addShapeInChart(int type, int placement, int left, int top, int right, int bottom, byte[] imageData) {#addShapeInChart-int-int-int-int-int-int-byte---}
```
public Shape addShapeInChart(int type, int placement, int left, int top, int right, int bottom, byte[] imageData)
```


Agrega una forma al gráfico. Todas las unidades son 1/4000 del área del gráfico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). El tipo de dibujo. |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype). el tipo de colocación. |
| izquierda | int | En unidades de 1/4000 del ancho del área del gráfico. |
| superior | int | En unidades de 1/4000 de la altura del área del gráfico. |
| derecha | int | En unidades de 1/4000 del ancho del área del gráfico. |
| inferior | int | En unidades de 1/4000 de la altura del área del gráfico. |
| imageData | byte[] | Si la forma no es una imagen ni un objeto ole, imageData debe ser nulo. |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom) {#addShapeInChartByScale-int-int-double-double-double-double-}
```
public Shape addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom)
```


Agregar una forma al gráfico. Todas las unidades están en escala porcentual del área del gráfico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). El tipo de dibujo. |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype). el tipo de colocación. |
| izquierda | double | La unidad está en escala porcentual del ancho del área del gráfico. |
| superior | double | La unidad está en escala porcentual de la altura del área del gráfico. |
| derecha | double | La unidad está en escala porcentual del ancho del área del gráfico. |
| inferior | double | La unidad está en escala porcentual de la altura del área del gráfico. |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom, byte[] imageData) {#addShapeInChartByScale-int-int-double-double-double-double-byte---}
```
public Shape addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom, byte[] imageData)
```


Agrega una forma al gráfico. Todas las unidades son 1/4000 del área del gráfico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). El tipo de dibujo. |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype). el tipo de colocación. |
| izquierda | double | La unidad está en escala porcentual del ancho del área del gráfico. |
| superior | double | La unidad está en escala porcentual de la altura del área del gráfico. |
| derecha | double | La unidad está en escala porcentual del ancho del área del gráfico. |
| inferior | double | La unidad está en escala porcentual de la altura del área del gráfico. |
| imageData | byte[] | Si la forma no es una imagen ni un objeto ole, imageData debe ser nulo. |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addSignatureLine(int topRow, int leftColumn, SignatureLine signatureLine) {#addSignatureLine-int-int-com.aspose.cells.SignatureLine-}
```
public Picture addSignatureLine(int topRow, int leftColumn, SignatureLine signatureLine)
```


Agrega una línea de firma a la hoja de cálculo.

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int | Índice de fila superior izquierda. |
| leftColumn | int | Índice de columna superior izquierda. |
| signatureLine | [SignatureLine](../../com.aspose.cells/signatureline) | Representa un objeto de línea de firma. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - 
### addSpinner(int topRow, int top, int leftColumn, int left, int height, int width) {#addSpinner-int-int-int-int-int-int-}
```
public Spinner addSpinner(int topRow, int top, int leftColumn, int left, int height, int width)
```


Agrega un Spinner a la hoja de cálculo.

**Example**

```
         //add a spinner
         Spinner spinner = shapes.addSpinner(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int | Índice de fila superior izquierda. |
| superior | int | Representa el desplazamiento vertical de Spinner desde su fila izquierda, en unidades de píxel. |
| leftColumn | int | Índice de columna superior izquierda. |
| izquierda | int | Representa el desplazamiento horizontal de Spinner desde su columna izquierda, en unidades de píxel. |
| altura | int | Representa la altura de Spinner, en unidades de píxel. |
| ancho | int | Representa el ancho de Spinner, en unidades de píxel. |

**Returns:**
[Spinner](../../com.aspose.cells/spinner) - A Spinner object.
### addSvg(int topRow, int top, int leftColumn, int left, int height, int width, byte[] svgData, byte[] compatibleImageData) {#addSvg-int-int-int-int-int-int-byte---byte---}
```
public Picture addSvg(int topRow, int top, int leftColumn, int left, int height, int width, byte[] svgData, byte[] compatibleImageData)
```


Añade una imagen svg.

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int | Índice de fila superior izquierda. |
| superior | int | Representa el desplazamiento vertical de la forma desde su fila izquierda, en unidades de píxel. |
| leftColumn | int | Índice de columna superior izquierda. |
| izquierda | int | El desplazamiento horizontal de la forma desde su columna izquierda, en unidades de píxel. |
| altura | int | La altura de la forma, en unidades de píxel. |
| ancho | int | El ancho de la forma, en unidades de píxel. |
| svgData | byte[] | Los datos de la imagen svg. |
| compatibleImageData | byte[] | Datos de imagen convertidos desde SVG para ser compatibles con Excel 2016 o versiones anteriores. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - 
### addTextBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addTextBox-int-int-int-int-int-int-}
```
public TextBox addTextBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Agrega un cuadro de texto a la hoja de cálculo.

**Example**

```
         //add a TextBox
         TextBox textBox = shapes.addTextBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | int | Índice de fila superior izquierda. |
| superior | int | Representa el desplazamiento vertical de textbox desde su fila superior, en unidades de píxel. |
| leftColumn | int | Índice de columna superior izquierda. |
| izquierda | int | Representa el desplazamiento horizontal de textbox desde su columna izquierda, en unidad de píxel. |
| altura | int | Representa la altura del cuadro de texto, en unidades de píxel. |
| ancho | int | Representa el ancho del cuadro de texto, en unidades de píxel. |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - A [TextBox](../../com.aspose.cells/textbox) object.
### addTextBoxInChart(int top, int left, int height, int width) {#addTextBoxInChart-int-int-int-int-}
```
public TextBox addTextBoxInChart(int top, int left, int height, int width)
```


Agrega un cuadro de texto al gráfico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| superior | int | Representa el desplazamiento vertical de textbox desde la esquina superior izquierda en unidades de 1/4000 del área del gráfico. |
| izquierda | int | Representa el desplazamiento vertical de textbox desde la esquina superior izquierda en unidades de 1/4000 del área del gráfico. |
| altura | int | Representa la altura de textbox, en unidades de 1/4000 del área del gráfico. |
| ancho | int | Representa el ancho de textbox, en unidades de 1/4000 del área del gráfico. |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - A TextBox object.
### addTextEffect(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int topRow, int top, int leftColumn, int left, int height, int width) {#addTextEffect-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-int-int-}
```
public Shape addTextEffect(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int topRow, int top, int leftColumn, int left, int height, int width)
```


Inserta un objeto WordArt.

**Example**

```
         //add a WordArt
         Shape wordArt1 = shapes.addTextEffect(MsoPresetTextEffect.TEXT_EFFECT_10, "WordArt", "arial", 18, false, false, 3, 0, 3, 0, 200, 50);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| effect | int | [MsoPresetTextEffect](../../com.aspose.cells/msopresettexteffect). El tipo de efecto de texto predefinido mso. |
| texto | java.lang.String | El texto de WordArt. |
| fontName | java.lang.String | El nombre de la fuente. |
| tamaño | int | El tamaño de la fuente |
| fontBold | boolean | Indica si la fuente está en negrita. |
| fontItalic | boolean | Indica si la fuente está en cursiva. |
| topRow | int | Índice de fila superior izquierda. |
| superior | int | Representa el desplazamiento vertical de la forma desde su fila izquierda, en unidades de píxel. |
| leftColumn | int | Índice de columna superior izquierda. |
| izquierda | int | Representa el desplazamiento horizontal de la forma desde su columna izquierda, en unidades de píxel. |
| altura | int | Representa la altura de la forma, en unidades de píxel. |
| ancho | int | Representa el ancho de la forma, en unidades de píxel. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - Returns a Shape object that represents the new WordArt object.
### addTextEffectInChart(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int top, int left, int height, int width) {#addTextEffectInChart-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-}
```
public Shape addTextEffectInChart(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int top, int left, int height, int width)
```


Inserta un objeto WordArt al gráfico

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| effect | int | [MsoPresetTextEffect](../../com.aspose.cells/msopresettexteffect). El tipo de efecto de texto predefinido mso. |
| texto | java.lang.String | El texto de WordArt. |
| fontName | java.lang.String | El nombre de la fuente. |
| tamaño | int | El tamaño de la fuente |
| fontBold | boolean | Indica si la fuente está en negrita. |
| fontItalic | boolean | Indica si la fuente está en cursiva. |
| superior | int | Representa el desplazamiento vertical de la forma desde la esquina superior izquierda en unidades de 1/4000 del área del gráfico. |
| izquierda | int | Representa el desplazamiento vertical de la forma desde la esquina superior izquierda en unidades de 1/4000 del área del gráfico. |
| altura | int | Representa la altura de la forma, en unidades de 1/4000 del área del gráfico. |
| ancho | int | Representa el ancho de la forma, en unidades de 1/4000 del área del gráfico. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - Returns a Shape object that represents the new WordArt object.
### addWordArt(int style, String text, int topRow, int top, int leftColumn, int left, int height, int width) {#addWordArt-int-java.lang.String-int-int-int-int-int-int-}
```
public Shape addWordArt(int style, String text, int topRow, int top, int leftColumn, int left, int height, int width)
```


Agrega WordArt predefinido desde Excel 2007.

**Example**

```
         //add a WordArt
         Shape wordArt2 = shapes.addWordArt(PresetWordArtStyle.WORD_ART_STYLE_1, "WordArt", 3, 0, 3, 0, 50, 200);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). El estilo de WordArt predefinido. |
| texto | java.lang.String | El texto. |
| topRow | int | Índice de fila superior izquierda. |
| superior | int | Representa el desplazamiento vertical de la forma desde su fila izquierda, en unidades de píxel. |
| leftColumn | int | Índice de columna superior izquierda. |
| izquierda | int | Representa el desplazamiento horizontal de la forma desde su columna izquierda, en unidades de píxel. |
| altura | int | Representa la altura de la forma, en unidades de píxel. |
| ancho | int | Representa el ancho de la forma, en unidades de píxel. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### clear() {#clear--}
```
public void clear()
```


Elimina todas las formas en la hoja de cálculo.

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


Devuelve si la instancia contiene este objeto

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| o | java.lang.Object | objeto de prueba |

**Returns:**
boolean - Si la instancia contiene este objeto
### copyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn) {#copyCommentsInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-}
```
public void copyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn)
```


Copia todos los comentarios en el rango.

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| shapes | [ShapeCollection](../../com.aspose.cells/shapecollection) | Las formas de origen. |
| ca | [CellArea](../../com.aspose.cells/cellarea) | El rango de origen. |
| destRow | int | La fila inicial del rango de destino. |
| destColumn | int | La columna inicial del rango de destino. |

### copyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, boolean isContained) {#copyInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-boolean-}
```
public void copyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, boolean isContained)
```


Copia las formas del rango al rango de destino.

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceShapes | [ShapeCollection](../../com.aspose.cells/shapecollection) | Formas de origen. |
| ca | [CellArea](../../com.aspose.cells/cellarea) | El rango de origen. |
| destRow | int | El índice de fila de destino del rango de destino. |
| destColumn | int | La columna de destino del rango de destino. |
| isContained | boolean | Indica si solo se copian las formas que están contenidas en el rango. Si es verdadero, solo copia las formas en el rango. De lo contrario, funciona como MS Office. |

### deleteInRange(CellArea ca) {#deleteInRange-com.aspose.cells.CellArea-}
```
public void deleteInRange(CellArea ca)
```


Elimina las formas en el rango. Las formas de comentario no se eliminarán.

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | El rango. Si las formas están contenidas en el rango, serán eliminadas. |

### deleteShape(Shape shape) {#deleteShape-com.aspose.cells.Shape-}
```
public void deleteShape(Shape shape)
```


Eliminar una forma. Si la forma está en el grupo o es una forma de comentario, no será eliminada.

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| shape | [Shape](../../com.aspose.cells/shape) |  |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### find(String what, int previous, FindOptions findOptions) {#find-java.lang.String-int-com.aspose.cells.FindOptions-}
```
public int find(String what, int previous, FindOptions findOptions)
```


Buscar forma por texto

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| qué | java.lang.String | El texto a buscar. |
| anterior | int | El índice de la forma anterior que contiene el mismo texto. -1 si se busca desde el inicio. |
| findOptions | [FindOptions](../../com.aspose.cells/findoptions) | Opciones de búsqueda |

**Returns:**
int - El índice de la forma encontrada, -1 si no se encuentra ninguna forma.
### get(int index) {#get-int-}
```
public Shape get(int index)
```


Obtiene el objeto [Shape](../../com.aspose.cells/shape) en el índice específico de la lista.

**Example**

```
         //get the first shape
         Shape shape = shapes.get(0);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### get(String name) {#get-java.lang.String-}
```
public Shape get(String name)
```


Obtiene el objeto [Shape](../../com.aspose.cells/shape) por el nombre de la forma.

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre de la forma. |

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


Obtiene el número de elementos contenidos en la instancia de CollectionBase.

**Returns:**
int - El número de elementos contenidos en la instancia de CollectionBase.
### group(Shape[] groupItems) {#group-com.aspose.cells.Shape---}
```
public GroupShape group(Shape[] groupItems)
```


Agrupa las formas.

**Remarks**

La forma en groupItems no debe estar agrupada. La forma debe estar en esta colección Shapes.

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| groupItems | [Shape\[\]](../../com.aspose.cells/shape) | los elementos del grupo. |

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


Determina el índice de un elemento específico en la instancia de CollectionBase.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| o | java.lang.Object | Determina el índice de un elemento específico en la instancia de CollectionBase. |

**Returns:**
int - El índice del valor si se encuentra en la lista; de lo contrario, -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Devuelve un enumerador que recorre la instancia de CollectionBase.

**Returns:**
java.util.Iterator - Un iterador para la instancia de CollectionBase.
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


Elimina la forma.

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| shape | [Shape](../../com.aspose.cells/shape) |  |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Elimina la forma.

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice de la forma. |

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


Desagrupa los elementos de forma.

**Remarks**

Si la forma de grupo está agrupada por otra forma de grupo, no se hará nada.

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| group | [GroupShape](../../com.aspose.cells/groupshape) | La forma de grupo. |

### updateSelectedValue() {#updateSelectedValue--}
```
public void updateSelectedValue()
```


Actualiza el valor seleccionado con el valor de la celda vinculada o del rango de la forma.

### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

