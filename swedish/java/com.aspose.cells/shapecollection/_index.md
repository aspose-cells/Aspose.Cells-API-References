---
title: "ShapeCollection"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar alla former i ett kalkylblad/diagram."
type: docs
url: /sv/java/com.aspose.cells/shapecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ShapeCollection extends CollectionBase
```

Representerar alla former i ett kalkylblad/diagram.

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
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Lägger till ett objekt i CollectionBase-instansen. |
| [addActiveXControl(int type, int topRow, int top, int leftColumn, int left, int width, int height)](#addActiveXControl-int-int-int-int-int-int-int-) | Skapar en Activex-kontroll. |
| [addArc(int topRow, int top, int leftColumn, int left, int height, int width)](#addArc-int-int-int-int-int-int-) | Lägger till en ArcShape i kalkylbladet. |
| [addAutoShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)](#addAutoShape-int-int-int-int-int-int-int-) | Lägger till en AutoShape i kalkylbladet. |
| [addAutoShapeInChart(int type, int top, int left, int height, int width)](#addAutoShapeInChart-int-int-int-int-int-) | Lägger till en AutoShape i diagrammet. |
| [addButton(int topRow, int top, int leftColumn, int left, int height, int width)](#addButton-int-int-int-int-int-int-) | Lägger till en knapp i kalkylbladet. |
| [addCheckBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addCheckBox-int-int-int-int-int-int-) | Lägger till en kryssruta i kalkylbladet. |
| [addComboBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addComboBox-int-int-int-int-int-int-) | Lägger till en ComboBox i kalkylbladet. |
| [addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left)](#addCopy-com.aspose.cells.Shape-int-int-int-int-) | Lägger till och kopierar en form i kalkylbladet. |
| [addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left, CopyOptions copyOptions)](#addCopy-com.aspose.cells.Shape-int-int-int-int-com.aspose.cells.CopyOptions-) | Lägger till och kopierar en form i kalkylbladet. |
| [addEquation(int topRow, int top, int leftColumn, int left, int height, int width)](#addEquation-int-int-int-int-int-int-) | Lägger till ett ekvationsobjekt i kalkylbladet. |
| [addFreeFloatingShape(int type, int top, int left, int height, int width, byte[] imageData, boolean isOriginalSize)](#addFreeFloatingShape-int-int-int-int-int-byte---boolean-) | Lägger till en fritt flytande form i kalkylbladet. Gäller endast för linje-/bildform. |
| [addFreeform(int topRow, int top, int leftColumn, int left, int height, int width, ShapePath[] paths)](#addFreeform-int-int-int-int-int-int-com.aspose.cells.ShapePath---) | Lägger till en frihandsform i kalkylbladet. |
| [addGroupBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addGroupBox-int-int-int-int-int-int-) | Lägger till en GroupBox i kalkylbladet. |
| [addIcons(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageByteData, byte[] compatibleImageData)](#addIcons-int-int-int-int-int-int-byte---byte---) | Lägger till en SVG-bild. |
| [addLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, int width, String latex)](#addLaTeXEquation-int-int-int-int-int-int-java.lang.String-) | Lägger till ett ekvationsobjekt i kalkylbladet med LaTeX-formatsträngar. |
| [addLabel(int topRow, int top, int leftColumn, int left, int height, int width)](#addLabel-int-int-int-int-int-int-) | Lägger till en etikett i kalkylbladet. |
| [addLabelInChart(int top, int left, int height, int width)](#addLabelInChart-int-int-int-int-) | Lägger till en etikett i diagrammet. |
| [addLine(int topRow, int top, int leftColumn, int left, int height, int width)](#addLine-int-int-int-int-int-int-) | Lägger till en LineShape i kalkylbladet. |
| [addLinkedPicture(int topRow, int leftColumn, int height, int width, String sourceFullName)](#addLinkedPicture-int-int-int-int-java.lang.String-) | Lägg till en länkad bild. |
| [addListBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addListBox-int-int-int-int-int-int-) | Lägger till en ListBox i kalkylbladet. |
| [addOleObject(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageData)](#addOleObject-int-int-int-int-int-int-byte---) | Lägger till ett OleObject. |
| [addOleObjectWithLinkedImage(int topRow, int leftColumn, int height, int width, String sourceFullName)](#addOleObjectWithLinkedImage-int-int-int-int-java.lang.String-) | Lägg till en länkad bild. |
| [addOval(int topRow, int top, int leftColumn, int left, int height, int width)](#addOval-int-int-int-int-int-int-) | Lägger till en Oval i kalkylbladet. |
| [addPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream)](#addPicture-int-int-int-int-java.io.InputStream-) | Lägger till en bild i samlingen. |
| [addPicture(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale)](#addPicture-int-int-java.io.InputStream-int-int-) | Lägger till en bild i samlingen. |
| [addPictureInChart(int top, int left, InputStream stream, int widthScale, int heightScale)](#addPictureInChart-int-int-java.io.InputStream-int-int-) | Lägger till en bild i diagrammet. |
| [addRadioButton(int topRow, int top, int leftColumn, int left, int height, int width)](#addRadioButton-int-int-int-int-int-int-) | Lägger till en RadioButton i arbetsbladet. |
| [addRectangle(int topRow, int top, int leftColumn, int left, int height, int width)](#addRectangle-int-int-int-int-int-int-) | Lägger till en RectangleShape i arbetsbladet. |
| [addScrollBar(int topRow, int top, int leftColumn, int left, int height, int width)](#addScrollBar-int-int-int-int-int-int-) | Lägger till en ScrollBar i arbetsbladet. |
| [addShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)](#addShape-int-int-int-int-int-int-int-) | Lägger till en form i arbetsbladet. |
| [addShapeInChart(int type, int placement, int left, int top, int right, int bottom)](#addShapeInChart-int-int-int-int-int-int-) | Lägg till en form i diagrammet. Alla enheter är 1/4000 av diagrammets område. |
| [addShapeInChart(int type, int placement, int left, int top, int right, int bottom, byte[] imageData)](#addShapeInChart-int-int-int-int-int-int-byte---) | Lägg till en form i diagrammet. Alla enheter är 1/4000 av diagrammets område. |
| [addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom)](#addShapeInChartByScale-int-int-double-double-double-double-) | Lägg till en form i diagrammet. |
| [addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom, byte[] imageData)](#addShapeInChartByScale-int-int-double-double-double-double-byte---) | Lägg till en form i diagrammet. Alla enheter är 1/4000 av diagrammets område. |
| [addSignatureLine(int topRow, int leftColumn, SignatureLine signatureLine)](#addSignatureLine-int-int-com.aspose.cells.SignatureLine-) | Lägger till en Signature Line i arbetsbladet. |
| [addSpinner(int topRow, int top, int leftColumn, int left, int height, int width)](#addSpinner-int-int-int-int-int-int-) | Lägger till en Spinner i arbetsbladet. |
| [addSvg(int topRow, int top, int leftColumn, int left, int height, int width, byte[] svgData, byte[] compatibleImageData)](#addSvg-int-int-int-int-int-int-byte---byte---) | Lägger till en SVG-bild. |
| [addTextBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addTextBox-int-int-int-int-int-int-) | Lägger till en textruta i arbetsbladet. |
| [addTextBoxInChart(int top, int left, int height, int width)](#addTextBoxInChart-int-int-int-int-) | Lägger till en textruta i diagrammet. |
| [addTextEffect(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int topRow, int top, int leftColumn, int left, int height, int width)](#addTextEffect-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-int-int-) | Infogar ett WordArt-objekt. |
| [addTextEffectInChart(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int top, int left, int height, int width)](#addTextEffectInChart-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-) | Infogar ett WordArt-objekt i diagrammet |
| [addWordArt(int style, String text, int topRow, int top, int leftColumn, int left, int height, int width)](#addWordArt-int-java.lang.String-int-int-int-int-int-int-) | Lägger till förinställt WordArt sedan Excel 2007.s |
| [clear()](#clear--) | Rensa alla former i arbetsbladet. |
| [contains(Object o)](#contains-java.lang.Object-) | Returnerar om instansen innehåller detta objekt |
| [copyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn)](#copyCommentsInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-) | Kopiera alla kommentarer i området. |
| [copyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, boolean isContained)](#copyInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-boolean-) | Kopiera former i området till målområdet. |
| [deleteInRange(CellArea ca)](#deleteInRange-com.aspose.cells.CellArea-) | Ta bort former i området. Kommentarformer kommer inte att tas bort. |
| [deleteShape(Shape shape)](#deleteShape-com.aspose.cells.Shape-) | Ta bort en form. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [find(String what, int previous, FindOptions findOptions)](#find-java.lang.String-int-com.aspose.cells.FindOptions-) | Hitta form efter text |
| [get(int index)](#get-int-) | Hämtar [Shape](../../com.aspose.cells/shape)-objektet på det specifika indexet i listan. |
| [get(String name)](#get-java.lang.String-) | Hämtar [Shape](../../com.aspose.cells/shape)-objektet efter formens namn. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Hämtar antalet element som finns i CollectionBase-instansen. |
| [group(Shape[] groupItems)](#group-com.aspose.cells.Shape---) | Gruppera formerna. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen. |
| [iterator()](#iterator--) | Returnerar en enumerator som itererar genom CollectionBase-instansen. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Shape shape)](#remove-com.aspose.cells.Shape-) | Ta bort formen. |
| [removeAt(int index)](#removeAt-int-) | Ta bort formen. |
| [toString()](#toString--) |  |
| [ungroup(GroupShape group)](#ungroup-com.aspose.cells.GroupShape-) | Avgruppera formobjekten. |
| [updateSelectedValue()](#updateSelectedValue--) | Uppdatera det valda värdet med värdet från den länkade cellen eller området för formen. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Lägger till ett objekt i CollectionBase-instansen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | Objektet som ska läggas till i CollectionBase-instansen. |

**Returns:**
int - Positionen där det nya elementet infördes.
### addActiveXControl(int type, int topRow, int top, int leftColumn, int left, int width, int height) {#addActiveXControl-int-int-int-int-int-int-int-}
```
public Shape addActiveXControl(int type, int topRow, int top, int leftColumn, int left, int width, int height)
```


Skapar en Activex-kontroll.

**Example**

```
         //add an ActiveX control
         Shape activeXControl = shapes.addActiveXControl(com.aspose.cells.ControlType.CHECK_BOX, 1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | int | [ControlType](../../com.aspose.cells/controltype). Typen av kontrollen. |
| topRow | int | Övre vänstra radindex. |
| överkant | int | Representerar det vertikala avståndet för Shape från dess vänstra rad, i enheten pixel. |
| leftColumn | int | Övre vänstra kolumnindex. |
| vänster | int | Representerar det horisontella avståndet för Shape från dess vänstra kolumn, i enheten pixel. |
| bredd | int | Representerar bredden på Shape, i enheten pixel. |
| höjd | int | Representerar höjden på Shape, i enheten pixel. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### addArc(int topRow, int top, int leftColumn, int left, int height, int width) {#addArc-int-int-int-int-int-int-}
```
public ArcShape addArc(int topRow, int top, int leftColumn, int left, int height, int width)
```


Lägger till en ArcShape i kalkylbladet.

**Example**

```
         //add a arc
         ArcShape arcShape = shapes.addArc(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | int | Övre vänstra radindex. |
| överkant | int | Representerar det vertikala avståndet för ArcShape från dess vänstra rad, i enheten pixel. |
| leftColumn | int | Övre vänstra kolumnindex. |
| vänster | int | Representerar det horisontella avståndet för ArcShape från dess vänstra kolumn, i enheten pixel. |
| höjd | int | Representerar höjden på ArcShape, i enheten pixel. |
| bredd | int | Representerar bredden på ArcShape, i enheten pixel. |

**Returns:**
[ArcShape](../../com.aspose.cells/arcshape) - A ArcShape object.
### addAutoShape(int type, int topRow, int top, int leftColumn, int left, int height, int width) {#addAutoShape-int-int-int-int-int-int-int-}
```
public Shape addAutoShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)
```


Lägger till en AutoShape i kalkylbladet.

**Remarks**

Typen kunde inte vara Diagram/Kommentar/Bild/OleObject/Polygon/DialogBox

**Example**

```
         //Adds a AutoShape to the worksheet.
         Shape autoShape = shapes.addAutoShape(AutoShapeType.CUBE, 1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | int | [AutoShapeType](../../com.aspose.cells/autoshapetype). Automatisk formtyp. |
| topRow | int | Övre vänstra radindex. |
| överkant | int | Representerar det vertikala avståndet för Shape från dess vänstra rad, i enheten pixel. |
| leftColumn | int | Övre vänstra kolumnindex. |
| vänster | int | Representerar det horisontella avståndet för Shape från dess vänstra kolumn, i enheten pixel. |
| höjd | int | Representerar höjden på Shape, i enheten pixel. |
| bredd | int | Representerar bredden på Shape, i enheten pixel. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - A Shape object.
### addAutoShapeInChart(int type, int top, int left, int height, int width) {#addAutoShapeInChart-int-int-int-int-int-}
```
public Shape addAutoShapeInChart(int type, int top, int left, int height, int width)
```


Lägger till en AutoShape i diagrammet.

**Remarks**

Typen kunde inte vara Diagram/Kommentar/Bild/OleObject/Polygon/DialogBox

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | int | [AutoShapeType](../../com.aspose.cells/autoshapetype). Automatisk formtyp. |
| överkant | int | Representerar det vertikala avståndet för textbox från det övre vänstra hörnet i enheter av 1/4000 av diagramområdet. |
| vänster | int | Representerar det vertikala avståndet för textbox från det övre vänstra hörnet i enheter av 1/4000 av diagramområdet. |
| höjd | int | Representerar höjden på textbox, i enheter av 1/4000 av diagramområdet. |
| bredd | int | Representerar bredden på textbox, i enheter av 1/4000 av diagramområdet. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - Returns a shape object.
### addButton(int topRow, int top, int leftColumn, int left, int height, int width) {#addButton-int-int-int-int-int-int-}
```
public Button addButton(int topRow, int top, int leftColumn, int left, int height, int width)
```


Lägger till en knapp i kalkylbladet.

**Example**

```
         //add a button
         Button button = shapes.addButton(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | int | Övre vänstra radindex. |
| överkant | int | Representerar det vertikala avståndet för Button från dess vänstra rad, i enheten pixel. |
| leftColumn | int | Övre vänstra kolumnindex. |
| vänster | int | Representerar det horisontella avståndet för Button från dess vänstra kolumn, i enheten pixel. |
| höjd | int | Representerar höjden på Button, i enheten pixel. |
| bredd | int | Representerar bredden på Button, i enheten pixel. |

**Returns:**
[Button](../../com.aspose.cells/button) - A Button object.
### addCheckBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addCheckBox-int-int-int-int-int-int-}
```
public CheckBox addCheckBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Lägger till en kryssruta i kalkylbladet.

**Example**

```
         //add a CheckBox
         CheckBox checkBox = shapes.addCheckBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | int | Övre vänstra radindex. |
| överkant | int | Representerar det vertikala avståndet för checkbox från dess översta rad, i enheten pixel. |
| leftColumn | int | Övre vänstra kolumnindex. |
| vänster | int | Representerar det horisontella avståndet för textbox från dess vänstra kolumn, i enheten pixel. |
| höjd | int | Höjd på textbox, i enheten pixel. |
| bredd | int | Bredd på textbox, i enheten pixel. |

**Returns:**
[CheckBox](../../com.aspose.cells/checkbox) - The new CheckBox object index.
### addComboBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addComboBox-int-int-int-int-int-int-}
```
public ComboBox addComboBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Lägger till en ComboBox i kalkylbladet.

**Example**

```
         //add a combo box
         ComboBox comboBox = shapes.addComboBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | int | Övre vänstra radindex. |
| överkant | int | Representerar den vertikala förskjutningen av ComboBox från dess vänstra rad, i enhet pixel. |
| leftColumn | int | Övre vänstra kolumnindex. |
| vänster | int | Representerar den horisontella förskjutningen av ComboBox från dess vänstra kolumn, i enhet pixel. |
| höjd | int | Representerar höjden på ComboBox, i enhet pixel. |
| bredd | int | Representerar bredden på ComboBox, i enhet pixel. |

**Returns:**
[ComboBox](../../com.aspose.cells/combobox) - A ComboBox object.
### addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left) {#addCopy-com.aspose.cells.Shape-int-int-int-int-}
```
public Shape addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left)
```


Lägger till och kopierar en form i kalkylbladet.

**Example**

```
         //add a shape
         RectangleShape rectangle = shapes.addRectangle(2, 0, 2, 0, 130, 130);
         //Adds and copies a shape.
         shapes.addCopy(rectangle, 7, 0, 7, 0);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceShape | [Shape](../../com.aspose.cells/shape) | Källform. |
| topRow | int | Det övre radindexet. |
| överkant | int | Representerar den vertikala förskjutningen från dess översta rad, i enhet pixel. |
| leftColumn | int | Det vänstra kolumnindexet. |
| vänster | int | Representerar den horisontella förskjutningen från dess vänstra kolumn, i enhet pixel. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - The new [Shape](../../com.aspose.cells/shape) object.
### addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left, CopyOptions copyOptions) {#addCopy-com.aspose.cells.Shape-int-int-int-int-com.aspose.cells.CopyOptions-}
```
public Shape addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left, CopyOptions copyOptions)
```


Lägger till och kopierar en form i kalkylbladet.

**Example**

```
         //add a shape
         RectangleShape rectangle = shapes.addRectangle(2, 0, 2, 0, 130, 130);
         //Adds and copies a shape.
         shapes.addCopy(rectangle, 7, 0, 7, 0);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceShape | [Shape](../../com.aspose.cells/shape) | Källform. |
| topRow | int | Det övre radindexet. |
| överkant | int | Representerar den vertikala förskjutningen från dess översta rad, i enhet pixel. |
| leftColumn | int | Det vänstra kolumnindexet. |
| vänster | int | Representerar den horisontella förskjutningen från dess vänstra kolumn, i enhet pixel. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | Alternativen för att kopiera former. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - The new [Shape](../../com.aspose.cells/shape) object.
### addEquation(int topRow, int top, int leftColumn, int left, int height, int width) {#addEquation-int-int-int-int-int-int-}
```
public TextBox addEquation(int topRow, int top, int leftColumn, int left, int height, int width)
```


Lägger till ett ekvationsobjekt i kalkylbladet.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | int | Det övre radindexet. |
| överkant | int | Den vertikala förskjutningen från dess översta rad, i enhet pixel. |
| leftColumn | int | Det vänstra kolumnindexet. |
| vänster | int | Den horisontella förskjutningen från dess vänstra kolumn, i enhet pixel. |
| höjd | int | Höjden på ekvationen, i enhet pixel. |
| bredd | int | Bredden på ekvationen, i enhet pixel. |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - 
### addFreeFloatingShape(int type, int top, int left, int height, int width, byte[] imageData, boolean isOriginalSize) {#addFreeFloatingShape-int-int-int-int-int-byte---boolean-}
```
public Shape addFreeFloatingShape(int type, int top, int left, int height, int width, byte[] imageData, boolean isOriginalSize)
```


Lägger till en fritt flytande form i kalkylbladet. Gäller endast för linje-/bildform.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Formtypen. |
| överkant | int | Representerar den vertikala förskjutningen av formen från kalkylbladets översta rad, i enhet pixel. |
| vänster | int | Representerar den horisontella förskjutningen av formen från kalkylbladets vänstra kolumn, i enhet pixel. |
| höjd | int | Representerar höjden på LineShape, i enhet pixel. |
| bredd | int | Representerar bredden på LineShape, i enhet pixel. |
| imageData | byte[] | Bilddata, gäller endast för bilden. |
| isOriginalSize | boolean | Om formen ska använda originalstorlek om formen är en bild. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### addFreeform(int topRow, int top, int leftColumn, int left, int height, int width, ShapePath[] paths) {#addFreeform-int-int-int-int-int-int-com.aspose.cells.ShapePath---}
```
public Shape addFreeform(int topRow, int top, int leftColumn, int left, int height, int width, ShapePath[] paths)
```


Lägger till en frihandsform i kalkylbladet.

**Remarks**

Obs: Att bredden och höjden i parametrarna kan vara vilka positiva heltalsvärden som helst, inte den totala bredden och höjden på ShapePath‑arrayen som specificeras av \\u9225\\u6a96aths'. Förhållandet mellan dem är ett skala‑fyll‑förhållande, det vill säga att varje ShapePath‑objekt kommer att skalas enligt bredden och höjden. Därför, när det finns flera objekt i 'paths', måste varje ShapePath‑objekt utformas på ett rimligt sätt för att möta förväntningarna. När det bara finns ett ShapePath‑objekt och det inte finns några andra krav, är det en bra lösning att skicka objektets bredd och höjd som parametervärden \\u9225\\u5b27\\u20ac\\u5a94s.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | int | Övre vänstra radindex. |
| överkant | int | Representerar den vertikala förskjutningen av frihandsformen från dess vänstra rad, i enhet pixel. |
| leftColumn | int | Övre vänstra kolumnindex. |
| vänster | int | Representerar den horisontella förskjutningen av frihandsformen från dess vänstra kolumn, i enhet pixel. |
| höjd | int | Representerar höjden på frihandsform, i enhet pixel. |
| bredd | int | Representerar bredden på frihandsform, i enhet pixel. |
| paths | [ShapePath\[\]](../../com.aspose.cells/shapepath) | Representerar en användardefinierad sökväg |

**Returns:**
[Shape](../../com.aspose.cells/shape) - A freeform shape.
### addGroupBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addGroupBox-int-int-int-int-int-int-}
```
public GroupBox addGroupBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Lägger till en GroupBox i kalkylbladet.

**Example**

```
         //add a group box
         GroupBox groupBox = shapes.addGroupBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | int | Övre vänstra radindex. |
| överkant | int | Representerar den vertikala förskjutningen av GroupBox från dess vänstra rad, i enhet pixel. |
| leftColumn | int | Övre vänstra kolumnindex. |
| vänster | int | Representerar den horisontella förskjutningen av GroupBox från dess vänstra kolumn, i enhet pixel. |
| höjd | int | Representerar höjden på GroupBox, i enhet pixel. |
| bredd | int | Representerar bredden på GroupBox, i enhet pixel. |

**Returns:**
[GroupBox](../../com.aspose.cells/groupbox) - A GroupBox object.
### addIcons(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageByteData, byte[] compatibleImageData) {#addIcons-int-int-int-int-int-int-byte---byte---}
```
public Picture addIcons(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageByteData, byte[] compatibleImageData)
```


Lägger till en SVG-bild.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | int | Övre vänstra radindex. |
| överkant | int | Representerar den vertikala förskjutningen av formen från dess vänstra rad, i enhet pixel. |
| leftColumn | int | Övre vänstra kolumnindex. |
| vänster | int | Den horisontella förskjutningen av formen från dess vänstra kolumn, i enhet pixel. |
| höjd | int | Höjden på formen, i enhet pixel. |
| bredd | int | Bredden på formen, i enhet pixel. |
| imageByteData | byte[] | Bildens byte-data. |
| compatibleImageData | byte[] | Konverterad bilddata från SVG för att vara kompatibel med Excel 2016 eller lägre versioner. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - 
### addLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, int width, String latex) {#addLaTeXEquation-int-int-int-int-int-int-java.lang.String-}
```
public TextBox addLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, int width, String latex)
```


Lägger till ett ekvationsobjekt i kalkylbladet med LaTeX-formatsträngar.

**Example**

```
         // LaTeX format string.
         String latex = "\\alpha +  \\frac{\\partial^2}{\\partial x_1\\partial x_2}y - \\left ( a + b \\right )+_{a}^{b}\\beta";
         // Adds an equation object to the worksheet.
         TextBox textBox = shapes.addLaTeXEquation(1, 0, 1, 0, 100, 300, latex);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | int | Det övre radindexet. |
| överkant | int | Den vertikala förskjutningen från dess översta rad, i enhet pixel. |
| leftColumn | int | Det vänstra kolumnindexet. |
| vänster | int | Den horisontella förskjutningen från dess vänstra kolumn, i enhet pixel. |
| höjd | int | Höjden på ekvationen, i enhet pixel. |
| bredd | int | Bredden på ekvationen, i enhet pixel. |
| latex | java.lang.String | LaTeX-formatsträng |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - 
### addLabel(int topRow, int top, int leftColumn, int left, int height, int width) {#addLabel-int-int-int-int-int-int-}
```
public Label addLabel(int topRow, int top, int leftColumn, int left, int height, int width)
```


Lägger till en etikett i kalkylbladet.

**Example**

```
         //add a label
         Label label = shapes.addLabel(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | int | Övre vänstra radindex. |
| överkant | int | Representerar den vertikala förskjutningen av Label från dess vänstra rad, i enhet pixel. |
| leftColumn | int | Övre vänstra kolumnindex. |
| vänster | int | Representerar den horisontella förskjutningen av Label från dess vänstra kolumn, i enhet pixel. |
| höjd | int | Representerar höjden på Label, i enhet pixel. |
| bredd | int | Representerar bredden på Label, i enhet pixel. |

**Returns:**
[Label](../../com.aspose.cells/label) - A Label object.
### addLabelInChart(int top, int left, int height, int width) {#addLabelInChart-int-int-int-int-}
```
public Label addLabelInChart(int top, int left, int height, int width)
```


Lägger till en etikett i diagrammet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| överkant | int | Representerar den vertikala förskjutningen av label från det övre vänstra hörnet i enheter av 1/4000 av diagramområdet. |
| vänster | int | Representerar den vertikala förskjutningen av label från det övre vänstra hörnet i enheter av 1/4000 av diagramområdet. |
| höjd | int | Representerar höjden på label, i enheter av 1/4000 av diagramområdet. |
| bredd | int | Representerar bredden på label, i enheter av 1/4000 av diagramområdet. |

**Returns:**
[Label](../../com.aspose.cells/label) - A new Label object.
### addLine(int topRow, int top, int leftColumn, int left, int height, int width) {#addLine-int-int-int-int-int-int-}
```
public LineShape addLine(int topRow, int top, int leftColumn, int left, int height, int width)
```


Lägger till en LineShape i kalkylbladet.

**Example**

```
         // add a line object
         LineShape lineShape = shapes.addLine(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | int | Övre vänstra radindex. |
| överkant | int | Representerar den vertikala förskjutningen av LineShape från dess vänstra rad, i enhet pixel. |
| leftColumn | int | Övre vänstra kolumnindex. |
| vänster | int | Representerar den horisontella förskjutningen av LineShape från dess vänstra kolumn, i enheten pixel. |
| höjd | int | Representerar höjden på LineShape, i enhet pixel. |
| bredd | int | Representerar bredden på LineShape, i enhet pixel. |

**Returns:**
[LineShape](../../com.aspose.cells/lineshape) - A LineShape object.
### addLinkedPicture(int topRow, int leftColumn, int height, int width, String sourceFullName) {#addLinkedPicture-int-int-int-int-java.lang.String-}
```
public Picture addLinkedPicture(int topRow, int leftColumn, int height, int width, String sourceFullName)
```


Lägg till en länkad bild.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | int | Övre vänstra radindex. |
| leftColumn | int | Övre vänstra kolumnindex. |
| höjd | int | Höjden på formen. I enheten pixlar |
| bredd | int | Bredden på formen. I enheten pixlar |
| sourceFullName | java.lang.String | Sökvägen och namnet på källfilen för den länkade bilden |

**Returns:**
[Picture](../../com.aspose.cells/picture) - [Picture](../../com.aspose.cells/picture) Picture object.
### addListBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addListBox-int-int-int-int-int-int-}
```
public ListBox addListBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Lägger till en ListBox i kalkylbladet.

**Example**

```
         //add a list box
         ListBox listBox = shapes.addListBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | int | Övre vänstra radindex. |
| överkant | int | Representerar den vertikala förskjutningen av ListBox från dess vänstra rad, i enheten pixel. |
| leftColumn | int | Övre vänstra kolumnindex. |
| vänster | int | Representerar den horisontella förskjutningen av ListBox från dess vänstra kolumn, i enheten pixel. |
| höjd | int | Representerar höjden på ListBox, i enheten pixel. |
| bredd | int | Representerar bredden på ListBox, i enheten pixel. |

**Returns:**
[ListBox](../../com.aspose.cells/listbox) - A ListBox object.
### addOleObject(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageData) {#addOleObject-int-int-int-int-int-int-byte---}
```
public OleObject addOleObject(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageData)
```


Lägger till ett OleObject.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | int |  |
| överkant | int |  |
| leftColumn | int |  |
| vänster | int |  |
| höjd | int |  |
| bredd | int |  |
| imageData | byte[] |  |

**Returns:**
[OleObject](../../com.aspose.cells/oleobject) - 
### addOleObjectWithLinkedImage(int topRow, int leftColumn, int height, int width, String sourceFullName) {#addOleObjectWithLinkedImage-int-int-int-int-java.lang.String-}
```
public OleObject addOleObjectWithLinkedImage(int topRow, int leftColumn, int height, int width, String sourceFullName)
```


Lägg till en länkad bild.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | int | Övre vänstra radindex. |
| leftColumn | int | Övre vänstra kolumnindex. |
| höjd | int | Höjden på formen. I enheten pixlar |
| bredd | int | Bredden på formen. I enheten pixlar |
| sourceFullName | java.lang.String | Sökvägen och namnet på källfilen för den länkade bilden |

**Returns:**
[OleObject](../../com.aspose.cells/oleobject) - [Picture](../../com.aspose.cells/picture) Picture object.
### addOval(int topRow, int top, int leftColumn, int left, int height, int width) {#addOval-int-int-int-int-int-int-}
```
public Oval addOval(int topRow, int top, int leftColumn, int left, int height, int width)
```


Lägger till en Oval i kalkylbladet.

**Example**

```
         //add a oval
         Oval oval = shapes.addOval(1, 0, 1, 0, 50, 50);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | int | Övre vänstra radindex. |
| överkant | int | Representerar den vertikala förskjutningen av Oval från dess vänstra rad, i enheten pixel. |
| leftColumn | int | Övre vänstra kolumnindex. |
| vänster | int | Representerar den horisontella förskjutningen av Oval från dess vänstra kolumn, i enheten pixel. |
| höjd | int | Representerar höjden på Oval, i enheten pixel. |
| bredd | int | Representerar bredden på Oval, i enheten pixel. |

**Returns:**
[Oval](../../com.aspose.cells/oval) - A Oval object.
### addPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream) {#addPicture-int-int-int-int-java.io.InputStream-}
```
public Picture addPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream)
```


Lägger till en bild i samlingen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | int | Övre vänstra radindex. |
| leftColumn | int | Övre vänstra kolumnindex. |
| bottomRow | int | Nedre högra radindex |
| rightColumn | int | Nedre högra kolumnindex |
| stream | java.io.InputStream | Strömobjekt som innehåller bilddata. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - [Picture](../../com.aspose.cells/picture) Picture object.
### addPicture(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale) {#addPicture-int-int-java.io.InputStream-int-int-}
```
public Picture addPicture(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale)
```


Lägger till en bild i samlingen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | int | Övre vänstra radindex. |
| leftColumn | int | Övre vänstra kolumnindex. |
| stream | java.io.InputStream | Strömobjekt som innehåller bilddata. |
| widthScale | int | Skala för bildens bredd, i procent. |
| heightScale | int | Skala för bildens höjd, i procent. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - [Picture](../../com.aspose.cells/picture) Picture object.
### addPictureInChart(int top, int left, InputStream stream, int widthScale, int heightScale) {#addPictureInChart-int-int-java.io.InputStream-int-int-}
```
public Picture addPictureInChart(int top, int left, InputStream stream, int widthScale, int heightScale)
```


Lägger till en bild i diagrammet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| överkant | int | Representerar den vertikala förskjutningen av formen från det övre vänstra hörnet i enheter av 1/4000 av diagramområdet. |
| vänster | int | Representerar den horisontella förskjutningen av formen från det övre vänstra hörnet i enheter av 1/4000 av diagramområdet. |
| stream | java.io.InputStream | Strömobjekt som innehåller bilddata. |
| widthScale | int | Skala för bildens bredd, i procent. |
| heightScale | int | Skala för bildens höjd, i procent. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns a Picture object.
### addRadioButton(int topRow, int top, int leftColumn, int left, int height, int width) {#addRadioButton-int-int-int-int-int-int-}
```
public RadioButton addRadioButton(int topRow, int top, int leftColumn, int left, int height, int width)
```


Lägger till en RadioButton i arbetsbladet.

**Example**

```
         //add a radio button
         RadioButton radioButton = shapes.addRadioButton(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | int | Övre vänstra radindex. |
| överkant | int | Representerar den vertikala förskjutningen av RadioButton från dess vänstra rad, i enheten pixel. |
| leftColumn | int | Övre vänstra kolumnindex. |
| vänster | int | Representerar den horisontella förskjutningen av RadioButton från dess vänstra kolumn, i enheten pixel. |
| höjd | int | Representerar höjden på RadioButton, i enheten pixel. |
| bredd | int | Representerar bredden på RadioButton, i enheten pixel. |

**Returns:**
[RadioButton](../../com.aspose.cells/radiobutton) - A RadioButton object.
### addRectangle(int topRow, int top, int leftColumn, int left, int height, int width) {#addRectangle-int-int-int-int-int-int-}
```
public RectangleShape addRectangle(int topRow, int top, int leftColumn, int left, int height, int width)
```


Lägger till en RectangleShape i arbetsbladet.

**Example**

```
         // add a rectangle
         RectangleShape rectangleShape = shapes.addRectangle(2, 0, 2, 0, 130, 130);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | int | Övre vänstra radindex. |
| överkant | int | Representerar den vertikala förskjutningen av RectangleShape från dess vänstra rad, i enhet pixel. |
| leftColumn | int | Övre vänstra kolumnindex. |
| vänster | int | Representerar den horisontella förskjutningen av RectangleShape från dess vänstra kolumn, i enhet pixel. |
| höjd | int | Representerar höjden på RectangleShape, i enhet pixel. |
| bredd | int | Representerar bredden på RectangleShape, i enhet pixel. |

**Returns:**
[RectangleShape](../../com.aspose.cells/rectangleshape) - A RectangleShape object.
### addScrollBar(int topRow, int top, int leftColumn, int left, int height, int width) {#addScrollBar-int-int-int-int-int-int-}
```
public ScrollBar addScrollBar(int topRow, int top, int leftColumn, int left, int height, int width)
```


Lägger till en ScrollBar i arbetsbladet.

**Example**

```
         //add a scroll bar
         ScrollBar scrollBar = shapes.addScrollBar(1, 0, 1, 0, 100, 20);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | int | Övre vänstra radindex. |
| överkant | int | Representerar den vertikala förskjutningen av ScrollBar från dess vänstra rad, i enhet pixel. |
| leftColumn | int | Övre vänstra kolumnindex. |
| vänster | int | Representerar den horisontella förskjutningen av ScrollBar från dess vänstra kolumn, i enhet pixel. |
| höjd | int | Representerar höjden på ScrollBar, i enhet pixel. |
| bredd | int | Representerar bredden på ScrollBar, i enhet pixel. |

**Returns:**
[ScrollBar](../../com.aspose.cells/scrollbar) - A ScrollBar object.
### addShape(int type, int topRow, int top, int leftColumn, int left, int height, int width) {#addShape-int-int-int-int-int-int-int-}
```
public Shape addShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)
```


Lägger till en form i arbetsbladet.

**Remarks**

Typen kunde inte vara Diagram/Kommentar/Bild/OleObject/Polygon/DialogBox

**Example**

```
         //Add a shape of the specified type
         Shape shapeByType = shapes.addShape(MsoDrawingType.CELLS_DRAWING, 1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Mso ritningstyp. |
| topRow | int | Övre vänstra radindex. |
| överkant | int | Representerar det vertikala avståndet för Shape från dess vänstra rad, i enheten pixel. |
| leftColumn | int | Övre vänstra kolumnindex. |
| vänster | int | Representerar det horisontella avståndet för Shape från dess vänstra kolumn, i enheten pixel. |
| höjd | int | Representerar höjden på Shape, i enheten pixel. |
| bredd | int | Representerar bredden på Shape, i enheten pixel. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - A Shape object.
### addShapeInChart(int type, int placement, int left, int top, int right, int bottom) {#addShapeInChart-int-int-int-int-int-int-}
```
public Shape addShapeInChart(int type, int placement, int left, int top, int right, int bottom)
```


Lägg till en form i diagrammet. Alla enheter är 1/4000 av diagrammets område.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Ritningstypen. |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype). placerings typen. |
| vänster | int | I enhet 1/4000 av diagramområdets bredd. |
| överkant | int | I enhet 1/4000 av diagramområdets höjd. |
| höger | int | I enhet 1/4000 av diagramområdets bredd. |
| nedre | int | I enhet 1/4000 av diagramområdets höjd. |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addShapeInChart(int type, int placement, int left, int top, int right, int bottom, byte[] imageData) {#addShapeInChart-int-int-int-int-int-int-byte---}
```
public Shape addShapeInChart(int type, int placement, int left, int top, int right, int bottom, byte[] imageData)
```


Lägg till en form i diagrammet. Alla enheter är 1/4000 av diagrammets område.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Ritningstypen. |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype). placerings typen. |
| vänster | int | I enhet 1/4000 av diagramområdets bredd. |
| överkant | int | I enhet 1/4000 av diagramområdets höjd. |
| höger | int | I enhet 1/4000 av diagramområdets bredd. |
| nedre | int | I enhet 1/4000 av diagramområdets höjd. |
| imageData | byte[] | Om formen inte är en bild eller ole-objekt,imageData bör vara null. |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom) {#addShapeInChartByScale-int-int-double-double-double-double-}
```
public Shape addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom)
```


Lägg till en form i diagrammet. Alla enheter är procentuell skala av diagramområdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Ritningstypen. |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype). placerings typen. |
| vänster | double | Enheten är procentuell skala av diagramområdets bredd. |
| överkant | double | Enheten är procentuell skala av diagramområdets höjd. |
| höger | double | Enheten är procentuell skala av diagramområdets bredd. |
| nedre | double | Enheten är procentuell skala av diagramområdets höjd. |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom, byte[] imageData) {#addShapeInChartByScale-int-int-double-double-double-double-byte---}
```
public Shape addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom, byte[] imageData)
```


Lägg till en form i diagrammet. Alla enheter är 1/4000 av diagrammets område.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Ritningstypen. |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype). placerings typen. |
| vänster | double | Enheten är procentuell skala av diagramområdets bredd. |
| överkant | double | Enheten är procentuell skala av diagramområdets höjd. |
| höger | double | Enheten är procentuell skala av diagramområdets bredd. |
| nedre | double | Enheten är procentuell skala av diagramområdets höjd. |
| imageData | byte[] | Om formen inte är en bild eller ole-objekt,imageData bör vara null. |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addSignatureLine(int topRow, int leftColumn, SignatureLine signatureLine) {#addSignatureLine-int-int-com.aspose.cells.SignatureLine-}
```
public Picture addSignatureLine(int topRow, int leftColumn, SignatureLine signatureLine)
```


Lägger till en Signature Line i arbetsbladet.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | int | Övre vänstra radindex. |
| leftColumn | int | Övre vänstra kolumnindex. |
| signatureLine | [SignatureLine](../../com.aspose.cells/signatureline) | Representerar ett signaturlinjeobjekt. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - 
### addSpinner(int topRow, int top, int leftColumn, int left, int height, int width) {#addSpinner-int-int-int-int-int-int-}
```
public Spinner addSpinner(int topRow, int top, int leftColumn, int left, int height, int width)
```


Lägger till en Spinner i arbetsbladet.

**Example**

```
         //add a spinner
         Spinner spinner = shapes.addSpinner(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | int | Övre vänstra radindex. |
| överkant | int | Representerar den vertikala förskjutningen av Spinner från dess vänstra rad, i enhet pixel. |
| leftColumn | int | Övre vänstra kolumnindex. |
| vänster | int | Representerar den horisontella förskjutningen av Spinner från dess vänstra kolumn, i enhet pixel. |
| höjd | int | Representerar höjden på Spinner, i enhet pixel. |
| bredd | int | Representerar bredden på Spinner, i enhet pixel. |

**Returns:**
[Spinner](../../com.aspose.cells/spinner) - A Spinner object.
### addSvg(int topRow, int top, int leftColumn, int left, int height, int width, byte[] svgData, byte[] compatibleImageData) {#addSvg-int-int-int-int-int-int-byte---byte---}
```
public Picture addSvg(int topRow, int top, int leftColumn, int left, int height, int width, byte[] svgData, byte[] compatibleImageData)
```


Lägger till en SVG-bild.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | int | Övre vänstra radindex. |
| överkant | int | Representerar den vertikala förskjutningen av formen från dess vänstra rad, i enhet pixel. |
| leftColumn | int | Övre vänstra kolumnindex. |
| vänster | int | Den horisontella förskjutningen av formen från dess vänstra kolumn, i enhet pixel. |
| höjd | int | Höjden på formen, i enhet pixel. |
| bredd | int | Bredden på formen, i enhet pixel. |
| svgData | byte[] | Svg-bilddata. |
| compatibleImageData | byte[] | Konverterad bilddata från SVG för att vara kompatibel med Excel 2016 eller lägre versioner. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - 
### addTextBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addTextBox-int-int-int-int-int-int-}
```
public TextBox addTextBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Lägger till en textruta i arbetsbladet.

**Example**

```
         //add a TextBox
         TextBox textBox = shapes.addTextBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | int | Övre vänstra radindex. |
| överkant | int | Representerar den vertikala förskjutningen av textrutan från dess översta rad, i enhet pixel. |
| leftColumn | int | Övre vänstra kolumnindex. |
| vänster | int | Representerar det horisontella avståndet för textbox från dess vänstra kolumn, i enheten pixel. |
| höjd | int | Representerar textrutans höjd, i enhet pixel. |
| bredd | int | Representerar textrutans bredd, i enhet pixel. |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - A [TextBox](../../com.aspose.cells/textbox) object.
### addTextBoxInChart(int top, int left, int height, int width) {#addTextBoxInChart-int-int-int-int-}
```
public TextBox addTextBoxInChart(int top, int left, int height, int width)
```


Lägger till en textruta i diagrammet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| överkant | int | Representerar det vertikala avståndet för textbox från det övre vänstra hörnet i enheter av 1/4000 av diagramområdet. |
| vänster | int | Representerar det vertikala avståndet för textbox från det övre vänstra hörnet i enheter av 1/4000 av diagramområdet. |
| höjd | int | Representerar höjden på textbox, i enheter av 1/4000 av diagramområdet. |
| bredd | int | Representerar bredden på textbox, i enheter av 1/4000 av diagramområdet. |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - A TextBox object.
### addTextEffect(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int topRow, int top, int leftColumn, int left, int height, int width) {#addTextEffect-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-int-int-}
```
public Shape addTextEffect(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int topRow, int top, int leftColumn, int left, int height, int width)
```


Infogar ett WordArt-objekt.

**Example**

```
         //add a WordArt
         Shape wordArt1 = shapes.addTextEffect(MsoPresetTextEffect.TEXT_EFFECT_10, "WordArt", "arial", 18, false, false, 3, 0, 3, 0, 200, 50);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| effect | int | [MsoPresetTextEffect](../../com.aspose.cells/msopresettexteffect). Den mso-förinställda texteffekttypen. |
| text | java.lang.String | WordArt-texten. |
| fontName | java.lang.String | Typsnittets namn. |
| storlek | int | Typsnittsstorleken |
| fontBold | boolean | Indikerar om typsnittet är fetstil. |
| fontItalic | boolean | Indikerar om typsnittet är kursivt. |
| topRow | int | Övre vänstra radindex. |
| överkant | int | Representerar den vertikala förskjutningen av formen från dess vänstra rad, i enhet pixel. |
| leftColumn | int | Övre vänstra kolumnindex. |
| vänster | int | Representerar den horisontella förskjutningen av formen från dess vänstra kolumn, i enhet pixel. |
| höjd | int | Representerar höjden på formen, i enhet pixlar. |
| bredd | int | Representerar formens bredd, i enhet pixel. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - Returns a Shape object that represents the new WordArt object.
### addTextEffectInChart(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int top, int left, int height, int width) {#addTextEffectInChart-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-}
```
public Shape addTextEffectInChart(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int top, int left, int height, int width)
```


Infogar ett WordArt-objekt i diagrammet

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| effect | int | [MsoPresetTextEffect](../../com.aspose.cells/msopresettexteffect). Den mso-förinställda texteffekttypen. |
| text | java.lang.String | WordArt-texten. |
| fontName | java.lang.String | Typsnittets namn. |
| storlek | int | Typsnittsstorleken |
| fontBold | boolean | Indikerar om typsnittet är fetstil. |
| fontItalic | boolean | Indikerar om typsnittet är kursivt. |
| överkant | int | Representerar den vertikala förskjutningen av formen från det övre vänstra hörnet i enheter av 1/4000 av diagramområdet. |
| vänster | int | Representerar den vertikala förskjutningen av formen från det övre vänstra hörnet i enheter av 1/4000 av diagramområdet. |
| höjd | int | Representerar formens höjd, i enheter av 1/4000 av diagramområdet. |
| bredd | int | Representerar formens bredd, i enheter av 1/4000 av diagramområdet. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - Returns a Shape object that represents the new WordArt object.
### addWordArt(int style, String text, int topRow, int top, int leftColumn, int left, int height, int width) {#addWordArt-int-java.lang.String-int-int-int-int-int-int-}
```
public Shape addWordArt(int style, String text, int topRow, int top, int leftColumn, int left, int height, int width)
```


Lägger till förinställt WordArt sedan Excel 2007.s

**Example**

```
         //add a WordArt
         Shape wordArt2 = shapes.addWordArt(PresetWordArtStyle.WORD_ART_STYLE_1, "WordArt", 3, 0, 3, 0, 50, 200);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). Den förinställda WordArt-stilen. |
| text | java.lang.String | Texten. |
| topRow | int | Övre vänstra radindex. |
| överkant | int | Representerar den vertikala förskjutningen av formen från dess vänstra rad, i enhet pixel. |
| leftColumn | int | Övre vänstra kolumnindex. |
| vänster | int | Representerar den horisontella förskjutningen av formen från dess vänstra kolumn, i enhet pixel. |
| höjd | int | Representerar höjden på formen, i enhet pixlar. |
| bredd | int | Representerar formens bredd, i enhet pixel. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### clear() {#clear--}
```
public void clear()
```


Rensa alla former i arbetsbladet.

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


Returnerar om instansen innehåller detta objekt

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | testobjekt |

**Returns:**
boolean - Om instansen innehåller detta objekt
### copyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn) {#copyCommentsInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-}
```
public void copyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn)
```


Kopiera alla kommentarer i området.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| shapes | [ShapeCollection](../../com.aspose.cells/shapecollection) | Källformerna. |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Källintervallet. |
| destRow | int | Målintervallens startrad. |
| destColumn | int | Målintervallens startkolumn. |

### copyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, boolean isContained) {#copyInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-boolean-}
```
public void copyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, boolean isContained)
```


Kopiera former i området till målområdet.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceShapes | [ShapeCollection](../../com.aspose.cells/shapecollection) | Källformer. |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Källintervallet. |
| destRow | int | Dest radindex för dest-området. |
| destColumn | int | Dest kolumn för dest-området. |
| isContained | boolean | Om endast formerna som finns inom området ska kopieras. Om true, kopieras endast formerna i området. Annars fungerar det som MS Office. |

### deleteInRange(CellArea ca) {#deleteInRange-com.aspose.cells.CellArea-}
```
public void deleteInRange(CellArea ca)
```


Ta bort former i området. Kommentarformer kommer inte att tas bort.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Området. Om formerna finns inom området kommer de att tas bort. |

### deleteShape(Shape shape) {#deleteShape-com.aspose.cells.Shape-}
```
public void deleteShape(Shape shape)
```


Ta bort en form. Om formen är i gruppen eller är en kommentarsform, kommer den inte att tas bort.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| shape | [Shape](../../com.aspose.cells/shape) |  |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### find(String what, int previous, FindOptions findOptions) {#find-java.lang.String-int-com.aspose.cells.FindOptions-}
```
public int find(String what, int previous, FindOptions findOptions)
```


Hitta form efter text

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| vad | java.lang.String | Texten att söka efter. |
| föregående | int | Indexet för föregående form som innehåller samma text. -1 om sökningen startas från början. |
| findOptions | [FindOptions](../../com.aspose.cells/findoptions) | Sökalternativ |

**Returns:**
int – Indexet för hittad form, -1 om ingen form hittas.
### get(int index) {#get-int-}
```
public Shape get(int index)
```


Hämtar [Shape](../../com.aspose.cells/shape)-objektet på det specifika indexet i listan.

**Example**

```
         //get the first shape
         Shape shape = shapes.get(0);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Indexet. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### get(String name) {#get-java.lang.String-}
```
public Shape get(String name)
```


Hämtar [Shape](../../com.aspose.cells/shape)-objektet efter formens namn.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Formens namn. |

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


Hämtar antalet element som finns i CollectionBase-instansen.

**Returns:**
int - Antalet element som finns i CollectionBase-instansen.
### group(Shape[] groupItems) {#group-com.aspose.cells.Shape---}
```
public GroupShape group(Shape[] groupItems)
```


Gruppera formerna.

**Remarks**

Formen i groupItems bör inte vara grupperad. Formen måste finnas i denna Shapes-samling.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| groupItems | [Shape\[\]](../../com.aspose.cells/shape) | gruppobjekten. |

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


Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen. |

**Returns:**
int - Indexet för värdet om det hittas i listan; annars -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Returnerar en enumerator som itererar genom CollectionBase-instansen.

**Returns:**
java.util.Iterator - En iterator för CollectionBase-instansen.
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


Ta bort formen.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| shape | [Shape](../../com.aspose.cells/shape) |  |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Ta bort formen.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Formens index. |

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


Avgruppera formobjekten.

**Remarks**

Om gruppformen är grupperad av en annan gruppform, görs inget.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| group | [GroupShape](../../com.aspose.cells/groupshape) | Gruppformen. |

### updateSelectedValue() {#updateSelectedValue--}
```
public void updateSelectedValue()
```


Uppdatera det valda värdet med värdet från den länkade cellen eller området för formen.

### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

