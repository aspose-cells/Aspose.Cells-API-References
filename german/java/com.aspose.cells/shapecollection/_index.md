---
title: "ShapeCollection"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt alle Formen in einem Arbeitsblatt/Diagramm dar."
type: docs
url: /de/java/com.aspose.cells/shapecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ShapeCollection extends CollectionBase
```

Stellt alle Formen in einem Arbeitsblatt/Diagramm dar.

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
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Fügt ein Element zur CollectionBase-Instanz hinzu. |
| [addActiveXControl(int type, int topRow, int top, int leftColumn, int left, int width, int height)](#addActiveXControl-int-int-int-int-int-int-int-) | Erstellt ein Activex-Steuerelement. |
| [addArc(int topRow, int top, int leftColumn, int left, int height, int width)](#addArc-int-int-int-int-int-int-) | Fügt dem Arbeitsblatt ein ArcShape hinzu. |
| [addAutoShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)](#addAutoShape-int-int-int-int-int-int-int-) | Fügt dem Arbeitsblatt ein AutoShape hinzu. |
| [addAutoShapeInChart(int type, int top, int left, int height, int width)](#addAutoShapeInChart-int-int-int-int-int-) | Fügt dem Diagramm ein AutoShape hinzu. |
| [addButton(int topRow, int top, int leftColumn, int left, int height, int width)](#addButton-int-int-int-int-int-int-) | Fügt dem Arbeitsblatt einen Button hinzu. |
| [addCheckBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addCheckBox-int-int-int-int-int-int-) | Fügt dem Arbeitsblatt ein Kontrollkästchen hinzu. |
| [addComboBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addComboBox-int-int-int-int-int-int-) | Fügt dem Arbeitsblatt eine ComboBox hinzu. |
| [addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left)](#addCopy-com.aspose.cells.Shape-int-int-int-int-) | Fügt eine Form dem Arbeitsblatt hinzu und kopiert sie. |
| [addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left, CopyOptions copyOptions)](#addCopy-com.aspose.cells.Shape-int-int-int-int-com.aspose.cells.CopyOptions-) | Fügt eine Form dem Arbeitsblatt hinzu und kopiert sie. |
| [addEquation(int topRow, int top, int leftColumn, int left, int height, int width)](#addEquation-int-int-int-int-int-int-) | Fügt dem Arbeitsblatt ein Gleichungsobjekt hinzu. |
| [addFreeFloatingShape(int type, int top, int left, int height, int width, byte[] imageData, boolean isOriginalSize)](#addFreeFloatingShape-int-int-int-int-int-byte---boolean-) | Fügt dem Arbeitsblatt eine frei schwebende Form hinzu. Gilt nur für Linien-/Bildformen. |
| [addFreeform(int topRow, int top, int leftColumn, int left, int height, int width, ShapePath[] paths)](#addFreeform-int-int-int-int-int-int-com.aspose.cells.ShapePath---) | Fügt dem Arbeitsblatt eine Freiformform hinzu. |
| [addGroupBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addGroupBox-int-int-int-int-int-int-) | Fügt dem Arbeitsblatt eine GroupBox hinzu. |
| [addIcons(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageByteData, byte[] compatibleImageData)](#addIcons-int-int-int-int-int-int-byte---byte---) | Fügt ein SVG-Bild hinzu. |
| [addLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, int width, String latex)](#addLaTeXEquation-int-int-int-int-int-int-java.lang.String-) | Fügt dem Arbeitsblatt ein Gleichungsobjekt hinzu, das LaTeX-Formatzeichenketten verwendet. |
| [addLabel(int topRow, int top, int leftColumn, int left, int height, int width)](#addLabel-int-int-int-int-int-int-) | Fügt dem Arbeitsblatt ein Label hinzu. |
| [addLabelInChart(int top, int left, int height, int width)](#addLabelInChart-int-int-int-int-) | Fügt dem Diagramm ein Label hinzu. |
| [addLine(int topRow, int top, int leftColumn, int left, int height, int width)](#addLine-int-int-int-int-int-int-) | Fügt dem Arbeitsblatt ein LineShape hinzu. |
| [addLinkedPicture(int topRow, int leftColumn, int height, int width, String sourceFullName)](#addLinkedPicture-int-int-int-int-java.lang.String-) | Füge ein verknüpftes Bild hinzu. |
| [addListBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addListBox-int-int-int-int-int-int-) | Fügt dem Arbeitsblatt eine ListBox hinzu. |
| [addOleObject(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageData)](#addOleObject-int-int-int-int-int-int-byte---) | Fügt ein OleObject hinzu. |
| [addOleObjectWithLinkedImage(int topRow, int leftColumn, int height, int width, String sourceFullName)](#addOleObjectWithLinkedImage-int-int-int-int-java.lang.String-) | Füge ein verknüpftes Bild hinzu. |
| [addOval(int topRow, int top, int leftColumn, int left, int height, int width)](#addOval-int-int-int-int-int-int-) | Fügt dem Arbeitsblatt ein Oval hinzu. |
| [addPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream)](#addPicture-int-int-int-int-java.io.InputStream-) | Fügt ein Bild zur Sammlung hinzu. |
| [addPicture(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale)](#addPicture-int-int-java.io.InputStream-int-int-) | Fügt ein Bild zur Sammlung hinzu. |
| [addPictureInChart(int top, int left, InputStream stream, int widthScale, int heightScale)](#addPictureInChart-int-int-java.io.InputStream-int-int-) | Fügt ein Bild zum Diagramm hinzu. |
| [addRadioButton(int topRow, int top, int leftColumn, int left, int height, int width)](#addRadioButton-int-int-int-int-int-int-) | Fügt einen RadioButton zum Arbeitsblatt hinzu. |
| [addRectangle(int topRow, int top, int leftColumn, int left, int height, int width)](#addRectangle-int-int-int-int-int-int-) | Fügt eine RectangleShape zum Arbeitsblatt hinzu. |
| [addScrollBar(int topRow, int top, int leftColumn, int left, int height, int width)](#addScrollBar-int-int-int-int-int-int-) | Fügt eine ScrollBar zum Arbeitsblatt hinzu. |
| [addShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)](#addShape-int-int-int-int-int-int-int-) | Fügt eine Shape zum Arbeitsblatt hinzu. |
| [addShapeInChart(int type, int placement, int left, int top, int right, int bottom)](#addShapeInChart-int-int-int-int-int-int-) | Füge eine Form zum Diagramm hinzu. Alle Einheiten sind 1/4000 des Diagrammbereichs. |
| [addShapeInChart(int type, int placement, int left, int top, int right, int bottom, byte[] imageData)](#addShapeInChart-int-int-int-int-int-int-byte---) | Füge eine Form zum Diagramm hinzu. Alle Einheiten sind 1/4000 des Diagrammbereichs. |
| [addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom)](#addShapeInChartByScale-int-int-double-double-double-double-) | Füge eine Form zum Diagramm hinzu. |
| [addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom, byte[] imageData)](#addShapeInChartByScale-int-int-double-double-double-double-byte---) | Füge eine Form zum Diagramm hinzu. Alle Einheiten sind 1/4000 des Diagrammbereichs. |
| [addSignatureLine(int topRow, int leftColumn, SignatureLine signatureLine)](#addSignatureLine-int-int-com.aspose.cells.SignatureLine-) | Fügt eine Signaturzeile zum Arbeitsblatt hinzu. |
| [addSpinner(int topRow, int top, int leftColumn, int left, int height, int width)](#addSpinner-int-int-int-int-int-int-) | Fügt einen Spinner zum Arbeitsblatt hinzu. |
| [addSvg(int topRow, int top, int leftColumn, int left, int height, int width, byte[] svgData, byte[] compatibleImageData)](#addSvg-int-int-int-int-int-int-byte---byte---) | Fügt ein SVG-Bild hinzu. |
| [addTextBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addTextBox-int-int-int-int-int-int-) | Fügt ein Textfeld zum Arbeitsblatt hinzu. |
| [addTextBoxInChart(int top, int left, int height, int width)](#addTextBoxInChart-int-int-int-int-) | Fügt ein Textfeld zum Diagramm hinzu. |
| [addTextEffect(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int topRow, int top, int leftColumn, int left, int height, int width)](#addTextEffect-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-int-int-) | Fügt ein WordArt-Objekt ein. |
| [addTextEffectInChart(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int top, int left, int height, int width)](#addTextEffectInChart-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-) | Fügt ein WordArt-Objekt zum Diagramm ein. |
| [addWordArt(int style, String text, int topRow, int top, int leftColumn, int left, int height, int width)](#addWordArt-int-java.lang.String-int-int-int-int-int-int-) | Fügt vordefiniertes WordArt seit Excel 2007 hinzu. |
| [clear()](#clear--) | Löscht alle Formen im Arbeitsblatt. |
| [contains(Object o)](#contains-java.lang.Object-) | Gibt zurück, ob die Instanz dieses Objekt enthält |
| [copyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn)](#copyCommentsInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-) | Kopiert alle Kommentare im Bereich. |
| [copyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, boolean isContained)](#copyInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-boolean-) | Kopiert Formen im Bereich zum Zielbereich. |
| [deleteInRange(CellArea ca)](#deleteInRange-com.aspose.cells.CellArea-) | Löscht Formen im Bereich. Kommentarformen werden nicht gelöscht. |
| [deleteShape(Shape shape)](#deleteShape-com.aspose.cells.Shape-) | Löscht eine Form. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [find(String what, int previous, FindOptions findOptions)](#find-java.lang.String-int-com.aspose.cells.FindOptions-) | Finde Form nach Text |
| [get(int index)](#get-int-) | Ruft das [Shape](../../com.aspose.cells/shape)-Objekt am bestimmten Index in der Liste ab. |
| [get(String name)](#get-java.lang.String-) | Ruft das [Shape](../../com.aspose.cells/shape)-Objekt anhand des Namens der Form ab. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ermittelt die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente. |
| [group(Shape[] groupItems)](#group-com.aspose.cells.Shape---) | Gruppiere die Formen. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz. |
| [iterator()](#iterator--) | Gibt einen Enumerator zurück, der die CollectionBase-Instanz durchläuft. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Shape shape)](#remove-com.aspose.cells.Shape-) | Entferne die Form. |
| [removeAt(int index)](#removeAt-int-) | Entferne die Form. |
| [toString()](#toString--) |  |
| [ungroup(GroupShape group)](#ungroup-com.aspose.cells.GroupShape-) | Entgruppiert die Formelemente. |
| [updateSelectedValue()](#updateSelectedValue--) | Aktualisiert den ausgewählten Wert anhand des Werts der verknüpften Zelle oder des Bereichs der Form. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Fügt ein Element zur CollectionBase-Instanz hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | Das Objekt, das zur CollectionBase-Instanz hinzugefügt werden soll. |

**Returns:**
int - Die Position, an der das neue Element eingefügt wurde.
### addActiveXControl(int type, int topRow, int top, int leftColumn, int left, int width, int height) {#addActiveXControl-int-int-int-int-int-int-int-}
```
public Shape addActiveXControl(int type, int topRow, int top, int leftColumn, int left, int width, int height)
```


Erstellt ein Activex-Steuerelement.

**Example**

```
         //add an ActiveX control
         Shape activeXControl = shapes.addActiveXControl(com.aspose.cells.ControlType.CHECK_BOX, 1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [ControlType](../../com.aspose.cells/controltype). Der Typ des Steuerelements. |
| topRow | int | Index der oberen linken Zeile. |
| oben | int | Stellt den vertikalen Versatz von Shape von seiner linken Zeile dar, in Pixeln. |
| leftColumn | int | Index der oberen linken Spalte. |
| links | int | Stellt den horizontalen Versatz von Shape von seiner linken Spalte dar, in Pixeln. |
| Breite | int | Stellt die Breite von Shape dar, in Pixeln. |
| Höhe | int | Stellt die Höhe von Shape dar, in Pixeln. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### addArc(int topRow, int top, int leftColumn, int left, int height, int width) {#addArc-int-int-int-int-int-int-}
```
public ArcShape addArc(int topRow, int top, int leftColumn, int left, int height, int width)
```


Fügt dem Arbeitsblatt ein ArcShape hinzu.

**Example**

```
         //add a arc
         ArcShape arcShape = shapes.addArc(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | int | Index der oberen linken Zeile. |
| oben | int | Stellt den vertikalen Versatz von ArcShape von seiner linken Zeile dar, in Pixeln. |
| leftColumn | int | Index der oberen linken Spalte. |
| links | int | Stellt den horizontalen Versatz von ArcShape von seiner linken Spalte dar, in Pixeln. |
| Höhe | int | Stellt die Höhe von ArcShape dar, in Pixeln. |
| Breite | int | Stellt die Breite von ArcShape dar, in Pixeln. |

**Returns:**
[ArcShape](../../com.aspose.cells/arcshape) - A ArcShape object.
### addAutoShape(int type, int topRow, int top, int leftColumn, int left, int height, int width) {#addAutoShape-int-int-int-int-int-int-int-}
```
public Shape addAutoShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)
```


Fügt dem Arbeitsblatt ein AutoShape hinzu.

**Remarks**

Der Typ konnte nicht Chart/Comment/Picture/OleObject/Polygon/DialogBox sein.

**Example**

```
         //Adds a AutoShape to the worksheet.
         Shape autoShape = shapes.addAutoShape(AutoShapeType.CUBE, 1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [AutoShapeType](../../com.aspose.cells/autoshapetype). Auto-Formtyp. |
| topRow | int | Index der oberen linken Zeile. |
| oben | int | Stellt den vertikalen Versatz von Shape von seiner linken Zeile dar, in Pixeln. |
| leftColumn | int | Index der oberen linken Spalte. |
| links | int | Stellt den horizontalen Versatz von Shape von seiner linken Spalte dar, in Pixeln. |
| Höhe | int | Stellt die Höhe von Shape dar, in Pixeln. |
| Breite | int | Stellt die Breite von Shape dar, in Pixeln. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - A Shape object.
### addAutoShapeInChart(int type, int top, int left, int height, int width) {#addAutoShapeInChart-int-int-int-int-int-}
```
public Shape addAutoShapeInChart(int type, int top, int left, int height, int width)
```


Fügt dem Diagramm ein AutoShape hinzu.

**Remarks**

Der Typ konnte nicht Chart/Comment/Picture/OleObject/Polygon/DialogBox sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [AutoShapeType](../../com.aspose.cells/autoshapetype). Auto-Formtyp. |
| oben | int | Stellt den vertikalen Versatz von textbox vom oberen linken Eckpunkt in Einheiten von 1/4000 des Diagrammbereichs dar. |
| links | int | Stellt den vertikalen Versatz von textbox vom oberen linken Eckpunkt in Einheiten von 1/4000 des Diagrammbereichs dar. |
| Höhe | int | Stellt die Höhe von textbox dar, in Einheiten von 1/4000 des Diagrammbereichs. |
| Breite | int | Stellt die Breite von textbox dar, in Einheiten von 1/4000 des Diagrammbereichs. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - Returns a shape object.
### addButton(int topRow, int top, int leftColumn, int left, int height, int width) {#addButton-int-int-int-int-int-int-}
```
public Button addButton(int topRow, int top, int leftColumn, int left, int height, int width)
```


Fügt dem Arbeitsblatt einen Button hinzu.

**Example**

```
         //add a button
         Button button = shapes.addButton(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | int | Index der oberen linken Zeile. |
| oben | int | Stellt den vertikalen Versatz von Button von seiner linken Zeile dar, in Pixeln. |
| leftColumn | int | Index der oberen linken Spalte. |
| links | int | Stellt den horizontalen Versatz von Button von seiner linken Spalte dar, in Pixeln. |
| Höhe | int | Stellt die Höhe von Button dar, in Pixeln. |
| Breite | int | Stellt die Breite von Button dar, in Pixeln. |

**Returns:**
[Button](../../com.aspose.cells/button) - A Button object.
### addCheckBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addCheckBox-int-int-int-int-int-int-}
```
public CheckBox addCheckBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Fügt dem Arbeitsblatt ein Kontrollkästchen hinzu.

**Example**

```
         //add a CheckBox
         CheckBox checkBox = shapes.addCheckBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | int | Index der oberen linken Zeile. |
| oben | int | Stellt den vertikalen Versatz von checkbox von seiner oberen Zeile dar, in Pixeln. |
| leftColumn | int | Index der oberen linken Spalte. |
| links | int | Stellt den horizontalen Versatz von textbox von seiner linken Spalte dar, in Pixeln. |
| Höhe | int | Höhe von textbox, in Pixeln. |
| Breite | int | Breite des Textfelds, in Pixel. |

**Returns:**
[CheckBox](../../com.aspose.cells/checkbox) - The new CheckBox object index.
### addComboBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addComboBox-int-int-int-int-int-int-}
```
public ComboBox addComboBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Fügt dem Arbeitsblatt eine ComboBox hinzu.

**Example**

```
         //add a combo box
         ComboBox comboBox = shapes.addComboBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | int | Index der oberen linken Zeile. |
| oben | int | Stellt den vertikalen Versatz der ComboBox von ihrer linken Zeile dar, in Pixel. |
| leftColumn | int | Index der oberen linken Spalte. |
| links | int | Stellt den horizontalen Versatz der ComboBox von ihrer linken Spalte dar, in Pixel. |
| Höhe | int | Stellt die Höhe der ComboBox dar, in Pixel. |
| Breite | int | Stellt die Breite der ComboBox dar, in Pixel. |

**Returns:**
[ComboBox](../../com.aspose.cells/combobox) - A ComboBox object.
### addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left) {#addCopy-com.aspose.cells.Shape-int-int-int-int-}
```
public Shape addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left)
```


Fügt eine Form dem Arbeitsblatt hinzu und kopiert sie.

**Example**

```
         //add a shape
         RectangleShape rectangle = shapes.addRectangle(2, 0, 2, 0, 130, 130);
         //Adds and copies a shape.
         shapes.addCopy(rectangle, 7, 0, 7, 0);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceShape | [Shape](../../com.aspose.cells/shape) | Quellform. |
| topRow | int | Der Index der oberen Zeile. |
| oben | int | Stellt den vertikalen Versatz von ihrer oberen Zeile dar, in Pixel. |
| leftColumn | int | Der Index der linken Spalte. |
| links | int | Stellt den horizontalen Versatz von ihrer linken Spalte dar, in Pixel. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - The new [Shape](../../com.aspose.cells/shape) object.
### addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left, CopyOptions copyOptions) {#addCopy-com.aspose.cells.Shape-int-int-int-int-com.aspose.cells.CopyOptions-}
```
public Shape addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left, CopyOptions copyOptions)
```


Fügt eine Form dem Arbeitsblatt hinzu und kopiert sie.

**Example**

```
         //add a shape
         RectangleShape rectangle = shapes.addRectangle(2, 0, 2, 0, 130, 130);
         //Adds and copies a shape.
         shapes.addCopy(rectangle, 7, 0, 7, 0);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceShape | [Shape](../../com.aspose.cells/shape) | Quellform. |
| topRow | int | Der Index der oberen Zeile. |
| oben | int | Stellt den vertikalen Versatz von ihrer oberen Zeile dar, in Pixel. |
| leftColumn | int | Der Index der linken Spalte. |
| links | int | Stellt den horizontalen Versatz von ihrer linken Spalte dar, in Pixel. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | Die Optionen zum Kopieren von Formen. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - The new [Shape](../../com.aspose.cells/shape) object.
### addEquation(int topRow, int top, int leftColumn, int left, int height, int width) {#addEquation-int-int-int-int-int-int-}
```
public TextBox addEquation(int topRow, int top, int leftColumn, int left, int height, int width)
```


Fügt dem Arbeitsblatt ein Gleichungsobjekt hinzu.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | int | Der Index der oberen Zeile. |
| oben | int | Der vertikale Versatz ihrer oberen Zeile, in Pixel. |
| leftColumn | int | Der Index der linken Spalte. |
| links | int | Der horizontale Versatz von ihrer linken Spalte, in Pixel. |
| Höhe | int | Die Höhe der Gleichung, in Pixel. |
| Breite | int | Die Breite der Gleichung, in Pixel. |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - 
### addFreeFloatingShape(int type, int top, int left, int height, int width, byte[] imageData, boolean isOriginalSize) {#addFreeFloatingShape-int-int-int-int-int-byte---boolean-}
```
public Shape addFreeFloatingShape(int type, int top, int left, int height, int width, byte[] imageData, boolean isOriginalSize)
```


Fügt dem Arbeitsblatt eine frei schwebende Form hinzu. Gilt nur für Linien-/Bildformen.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Der Formtyp. |
| oben | int | Stellt den vertikalen Versatz der Form von der oberen Zeile des Arbeitsblatts dar, in Pixel. |
| links | int | Stellt den horizontalen Versatz der Form von der linken Spalte des Arbeitsblatts dar, in Pixel. |
| Höhe | int | Stellt die Höhe von LineShape dar, in Pixel. |
| Breite | int | Stellt die Breite von LineShape dar, in Pixel. |
| imageData | byte[] | Die Bilddaten, gelten nur für das Bild. |
| isOriginalSize | boolean | Ob die Form die Originalgröße verwendet, wenn die Form ein Bild ist. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### addFreeform(int topRow, int top, int leftColumn, int left, int height, int width, ShapePath[] paths) {#addFreeform-int-int-int-int-int-int-com.aspose.cells.ShapePath---}
```
public Shape addFreeform(int topRow, int top, int leftColumn, int left, int height, int width, ShapePath[] paths)
```


Fügt dem Arbeitsblatt eine Freiformform hinzu.

**Remarks**

Hinweis: Die Breite und Höhe in den Parametern können beliebige positive Ganzzahlen sein, nicht die gesamte Breite und Höhe des ShapePath-Arrays, das durch \\u9225\\u6a96aths' angegeben ist. Die Beziehung zwischen ihnen ist eine Skalierungs‑Füll‑Beziehung, das heißt, jedes ShapePath-Objekt wird entsprechend der Breite und Höhe skaliert. Daher muss, wenn mehrere Objekte in den 'paths' vorhanden sind, jedes ShapePath-Objekt vernünftig gestaltet werden, um den Erwartungen zu entsprechen. Wenn nur ein ShapePath-Objekt vorhanden ist und keine weiteren Anforderungen bestehen, ist das Übergeben der Breite und Höhe des Objekts als Parameterwerte \\u9225\\u5b27\\u20ac\\u5a94s eine gute Lösung.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | int | Index der oberen linken Zeile. |
| oben | int | Stellt den vertikalen Versatz der Freiformform von ihrer linken Zeile dar, in Pixel. |
| leftColumn | int | Index der oberen linken Spalte. |
| links | int | Stellt den horizontalen Versatz der Freiformform von ihrer linken Spalte dar, in Pixel. |
| Höhe | int | Stellt die Höhe der Freiformform dar, in Pixel. |
| Breite | int | Stellt die Breite der Freiformform dar, in Pixel. |
| paths | [ShapePath\[\]](../../com.aspose.cells/shapepath) | Stellt einen benutzerdefinierten Pfad dar |

**Returns:**
[Shape](../../com.aspose.cells/shape) - A freeform shape.
### addGroupBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addGroupBox-int-int-int-int-int-int-}
```
public GroupBox addGroupBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Fügt dem Arbeitsblatt eine GroupBox hinzu.

**Example**

```
         //add a group box
         GroupBox groupBox = shapes.addGroupBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | int | Index der oberen linken Zeile. |
| oben | int | Stellt den vertikalen Versatz der GroupBox von ihrer linken Zeile dar, in Pixel. |
| leftColumn | int | Index der oberen linken Spalte. |
| links | int | Stellt den horizontalen Versatz der GroupBox von ihrer linken Spalte dar, in Pixel. |
| Höhe | int | Stellt die Höhe der GroupBox dar, in Pixel. |
| Breite | int | Stellt die Breite der GroupBox dar, in Pixel. |

**Returns:**
[GroupBox](../../com.aspose.cells/groupbox) - A GroupBox object.
### addIcons(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageByteData, byte[] compatibleImageData) {#addIcons-int-int-int-int-int-int-byte---byte---}
```
public Picture addIcons(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageByteData, byte[] compatibleImageData)
```


Fügt ein SVG-Bild hinzu.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | int | Index der oberen linken Zeile. |
| oben | int | Stellt den vertikalen Versatz der Form von ihrer linken Zeile dar, in Pixel. |
| leftColumn | int | Index der oberen linken Spalte. |
| links | int | Der horizontale Versatz der Form von ihrer linken Spalte, in Pixel. |
| Höhe | int | Die Höhe der Form, in Pixel. |
| Breite | int | Die Breite der Form, in Pixel. |
| imageByteData | byte[] | Die Bild-Byte-Daten. |
| compatibleImageData | byte[] | Konvertierte Bilddaten von SVG, um mit Excel 2016 oder älteren Versionen kompatibel zu sein. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - 
### addLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, int width, String latex) {#addLaTeXEquation-int-int-int-int-int-int-java.lang.String-}
```
public TextBox addLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, int width, String latex)
```


Fügt dem Arbeitsblatt ein Gleichungsobjekt hinzu, das LaTeX-Formatzeichenketten verwendet.

**Example**

```
         // LaTeX format string.
         String latex = "\\alpha +  \\frac{\\partial^2}{\\partial x_1\\partial x_2}y - \\left ( a + b \\right )+_{a}^{b}\\beta";
         // Adds an equation object to the worksheet.
         TextBox textBox = shapes.addLaTeXEquation(1, 0, 1, 0, 100, 300, latex);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | int | Der Index der oberen Zeile. |
| oben | int | Der vertikale Versatz ihrer oberen Zeile, in Pixel. |
| leftColumn | int | Der Index der linken Spalte. |
| links | int | Der horizontale Versatz von ihrer linken Spalte, in Pixel. |
| Höhe | int | Die Höhe der Gleichung, in Pixel. |
| Breite | int | Die Breite der Gleichung, in Pixel. |
| latex | java.lang.String | LaTeX-Formatzeichenfolge |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - 
### addLabel(int topRow, int top, int leftColumn, int left, int height, int width) {#addLabel-int-int-int-int-int-int-}
```
public Label addLabel(int topRow, int top, int leftColumn, int left, int height, int width)
```


Fügt dem Arbeitsblatt ein Label hinzu.

**Example**

```
         //add a label
         Label label = shapes.addLabel(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | int | Index der oberen linken Zeile. |
| oben | int | Stellt den vertikalen Versatz des Labels von seiner linken Zeile dar, in Pixel. |
| leftColumn | int | Index der oberen linken Spalte. |
| links | int | Stellt den horizontalen Versatz des Labels von seiner linken Spalte dar, in Pixel. |
| Höhe | int | Stellt die Höhe des Labels dar, in Pixel. |
| Breite | int | Stellt die Breite des Labels dar, in Pixel. |

**Returns:**
[Label](../../com.aspose.cells/label) - A Label object.
### addLabelInChart(int top, int left, int height, int width) {#addLabelInChart-int-int-int-int-}
```
public Label addLabelInChart(int top, int left, int height, int width)
```


Fügt dem Diagramm ein Label hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| oben | int | Stellt den vertikalen Versatz des Labels von der oberen linken Ecke in Einheiten von 1/4000 des Diagrammbereichs dar. |
| links | int | Stellt den vertikalen Versatz des Labels von der oberen linken Ecke in Einheiten von 1/4000 des Diagrammbereichs dar. |
| Höhe | int | Stellt die Höhe des Labels in Einheiten von 1/4000 des Diagrammbereichs dar. |
| Breite | int | Stellt die Breite des Labels in Einheiten von 1/4000 des Diagrammbereichs dar. |

**Returns:**
[Label](../../com.aspose.cells/label) - A new Label object.
### addLine(int topRow, int top, int leftColumn, int left, int height, int width) {#addLine-int-int-int-int-int-int-}
```
public LineShape addLine(int topRow, int top, int leftColumn, int left, int height, int width)
```


Fügt dem Arbeitsblatt ein LineShape hinzu.

**Example**

```
         // add a line object
         LineShape lineShape = shapes.addLine(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | int | Index der oberen linken Zeile. |
| oben | int | Stellt den vertikalen Versatz von LineShape von seiner linken Zeile dar, in Einheit Pixel. |
| leftColumn | int | Index der oberen linken Spalte. |
| links | int | Stellt den horizontalen Versatz von LineShape von seiner linken Spalte dar, in Einheit Pixel. |
| Höhe | int | Stellt die Höhe von LineShape dar, in Pixel. |
| Breite | int | Stellt die Breite von LineShape dar, in Pixel. |

**Returns:**
[LineShape](../../com.aspose.cells/lineshape) - A LineShape object.
### addLinkedPicture(int topRow, int leftColumn, int height, int width, String sourceFullName) {#addLinkedPicture-int-int-int-int-java.lang.String-}
```
public Picture addLinkedPicture(int topRow, int leftColumn, int height, int width, String sourceFullName)
```


Füge ein verknüpftes Bild hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | int | Index der oberen linken Zeile. |
| leftColumn | int | Index der oberen linken Spalte. |
| Höhe | int | Die Höhe der Form. In Einheit Pixel. |
| Breite | int | Die Breite der Form. In Einheit Pixel. |
| sourceFullName | java.lang.String | Der Pfad und Name der Quelldatei für das verknüpfte Bild. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - [Picture](../../com.aspose.cells/picture) Picture object.
### addListBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addListBox-int-int-int-int-int-int-}
```
public ListBox addListBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Fügt dem Arbeitsblatt eine ListBox hinzu.

**Example**

```
         //add a list box
         ListBox listBox = shapes.addListBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | int | Index der oberen linken Zeile. |
| oben | int | Stellt den vertikalen Versatz von ListBox von seiner linken Zeile dar, in Einheit Pixel. |
| leftColumn | int | Index der oberen linken Spalte. |
| links | int | Stellt den horizontalen Versatz von ListBox von seiner linken Spalte dar, in Einheit Pixel. |
| Höhe | int | Stellt die Höhe von ListBox dar, in Einheit Pixel. |
| Breite | int | Stellt die Breite von ListBox dar, in Einheit Pixel. |

**Returns:**
[ListBox](../../com.aspose.cells/listbox) - A ListBox object.
### addOleObject(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageData) {#addOleObject-int-int-int-int-int-int-byte---}
```
public OleObject addOleObject(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageData)
```


Fügt ein OleObject hinzu.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | int |  |
| oben | int |  |
| leftColumn | int |  |
| links | int |  |
| Höhe | int |  |
| Breite | int |  |
| imageData | byte[] |  |

**Returns:**
[OleObject](../../com.aspose.cells/oleobject) - 
### addOleObjectWithLinkedImage(int topRow, int leftColumn, int height, int width, String sourceFullName) {#addOleObjectWithLinkedImage-int-int-int-int-java.lang.String-}
```
public OleObject addOleObjectWithLinkedImage(int topRow, int leftColumn, int height, int width, String sourceFullName)
```


Füge ein verknüpftes Bild hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | int | Index der oberen linken Zeile. |
| leftColumn | int | Index der oberen linken Spalte. |
| Höhe | int | Die Höhe der Form. In Einheit Pixel. |
| Breite | int | Die Breite der Form. In Einheit Pixel. |
| sourceFullName | java.lang.String | Der Pfad und Name der Quelldatei für das verknüpfte Bild. |

**Returns:**
[OleObject](../../com.aspose.cells/oleobject) - [Picture](../../com.aspose.cells/picture) Picture object.
### addOval(int topRow, int top, int leftColumn, int left, int height, int width) {#addOval-int-int-int-int-int-int-}
```
public Oval addOval(int topRow, int top, int leftColumn, int left, int height, int width)
```


Fügt dem Arbeitsblatt ein Oval hinzu.

**Example**

```
         //add a oval
         Oval oval = shapes.addOval(1, 0, 1, 0, 50, 50);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | int | Index der oberen linken Zeile. |
| oben | int | Stellt den vertikalen Versatz von Oval von seiner linken Zeile dar, in Einheit Pixel. |
| leftColumn | int | Index der oberen linken Spalte. |
| links | int | Stellt den horizontalen Versatz von Oval von seiner linken Spalte dar, in Einheit Pixel. |
| Höhe | int | Stellt die Höhe von Oval dar, in Einheit Pixel. |
| Breite | int | Stellt die Breite von Oval dar, in Einheit Pixel. |

**Returns:**
[Oval](../../com.aspose.cells/oval) - A Oval object.
### addPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream) {#addPicture-int-int-int-int-java.io.InputStream-}
```
public Picture addPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream)
```


Fügt ein Bild zur Sammlung hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | int | Index der oberen linken Zeile. |
| leftColumn | int | Index der oberen linken Spalte. |
| bottomRow | int | Index der unteren rechten Zeile |
| rightColumn | int | Index der unteren rechten Spalte |
| stream | java.io.InputStream | Stream-Objekt, das die Bilddaten enthält. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - [Picture](../../com.aspose.cells/picture) Picture object.
### addPicture(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale) {#addPicture-int-int-java.io.InputStream-int-int-}
```
public Picture addPicture(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale)
```


Fügt ein Bild zur Sammlung hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | int | Index der oberen linken Zeile. |
| leftColumn | int | Index der oberen linken Spalte. |
| stream | java.io.InputStream | Stream-Objekt, das die Bilddaten enthält. |
| widthScale | int | Skalierung der Bildbreite, ein Prozentsatz. |
| heightScale | int | Skalierung der Bildhöhe, ein Prozentsatz. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - [Picture](../../com.aspose.cells/picture) Picture object.
### addPictureInChart(int top, int left, InputStream stream, int widthScale, int heightScale) {#addPictureInChart-int-int-java.io.InputStream-int-int-}
```
public Picture addPictureInChart(int top, int left, InputStream stream, int widthScale, int heightScale)
```


Fügt ein Bild zum Diagramm hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| oben | int | Stellt den vertikalen Versatz der Form vom oberen linken Eckpunkt in Einheiten von 1/4000 des Diagrammbereichs dar. |
| links | int | Stellt den horizontalen Versatz der Form vom oberen linken Eckpunkt in Einheiten von 1/4000 des Diagrammbereichs dar. |
| stream | java.io.InputStream | Stream-Objekt, das die Bilddaten enthält. |
| widthScale | int | Skalierung der Bildbreite, ein Prozentsatz. |
| heightScale | int | Skalierung der Bildhöhe, ein Prozentsatz. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns a Picture object.
### addRadioButton(int topRow, int top, int leftColumn, int left, int height, int width) {#addRadioButton-int-int-int-int-int-int-}
```
public RadioButton addRadioButton(int topRow, int top, int leftColumn, int left, int height, int width)
```


Fügt einen RadioButton zum Arbeitsblatt hinzu.

**Example**

```
         //add a radio button
         RadioButton radioButton = shapes.addRadioButton(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | int | Index der oberen linken Zeile. |
| oben | int | Stellt den vertikalen Versatz von RadioButton von seiner linken Zeile dar, in Einheit Pixel. |
| leftColumn | int | Index der oberen linken Spalte. |
| links | int | Stellt den horizontalen Versatz von RadioButton von seiner linken Spalte dar, in Einheit Pixel. |
| Höhe | int | Stellt die Höhe von RadioButton dar, in Einheit Pixel. |
| Breite | int | Stellt die Breite des RadioButton dar, in Einheit Pixel. |

**Returns:**
[RadioButton](../../com.aspose.cells/radiobutton) - A RadioButton object.
### addRectangle(int topRow, int top, int leftColumn, int left, int height, int width) {#addRectangle-int-int-int-int-int-int-}
```
public RectangleShape addRectangle(int topRow, int top, int leftColumn, int left, int height, int width)
```


Fügt eine RectangleShape zum Arbeitsblatt hinzu.

**Example**

```
         // add a rectangle
         RectangleShape rectangleShape = shapes.addRectangle(2, 0, 2, 0, 130, 130);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | int | Index der oberen linken Zeile. |
| oben | int | Stellt den vertikalen Versatz von RectangleShape von seiner linken Zeile dar, in Einheit Pixel. |
| leftColumn | int | Index der oberen linken Spalte. |
| links | int | Stellt den horizontalen Versatz von RectangleShape von seiner linken Spalte dar, in Einheit Pixel. |
| Höhe | int | Stellt die Höhe von RectangleShape dar, in Einheit Pixel. |
| Breite | int | Stellt die Breite von RectangleShape dar, in Einheit Pixel. |

**Returns:**
[RectangleShape](../../com.aspose.cells/rectangleshape) - A RectangleShape object.
### addScrollBar(int topRow, int top, int leftColumn, int left, int height, int width) {#addScrollBar-int-int-int-int-int-int-}
```
public ScrollBar addScrollBar(int topRow, int top, int leftColumn, int left, int height, int width)
```


Fügt eine ScrollBar zum Arbeitsblatt hinzu.

**Example**

```
         //add a scroll bar
         ScrollBar scrollBar = shapes.addScrollBar(1, 0, 1, 0, 100, 20);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | int | Index der oberen linken Zeile. |
| oben | int | Stellt den vertikalen Versatz von ScrollBar von seiner linken Zeile dar, in Einheit Pixel. |
| leftColumn | int | Index der oberen linken Spalte. |
| links | int | Stellt den horizontalen Versatz von ScrollBar von seiner linken Spalte dar, in Einheit Pixel. |
| Höhe | int | Stellt die Höhe von ScrollBar dar, in Einheit Pixel. |
| Breite | int | Stellt die Breite von ScrollBar dar, in Einheit Pixel. |

**Returns:**
[ScrollBar](../../com.aspose.cells/scrollbar) - A ScrollBar object.
### addShape(int type, int topRow, int top, int leftColumn, int left, int height, int width) {#addShape-int-int-int-int-int-int-int-}
```
public Shape addShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)
```


Fügt eine Shape zum Arbeitsblatt hinzu.

**Remarks**

Der Typ konnte nicht Chart/Comment/Picture/OleObject/Polygon/DialogBox sein.

**Example**

```
         //Add a shape of the specified type
         Shape shapeByType = shapes.addShape(MsoDrawingType.CELLS_DRAWING, 1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Mso-Zeichnungstyp. |
| topRow | int | Index der oberen linken Zeile. |
| oben | int | Stellt den vertikalen Versatz von Shape von seiner linken Zeile dar, in Pixeln. |
| leftColumn | int | Index der oberen linken Spalte. |
| links | int | Stellt den horizontalen Versatz von Shape von seiner linken Spalte dar, in Pixeln. |
| Höhe | int | Stellt die Höhe von Shape dar, in Pixeln. |
| Breite | int | Stellt die Breite von Shape dar, in Pixeln. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - A Shape object.
### addShapeInChart(int type, int placement, int left, int top, int right, int bottom) {#addShapeInChart-int-int-int-int-int-int-}
```
public Shape addShapeInChart(int type, int placement, int left, int top, int right, int bottom)
```


Füge eine Form zum Diagramm hinzu. Alle Einheiten sind 1/4000 des Diagrammbereichs.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Der Zeichnungstyp. |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype). der Platzierungstyp. |
| links | int | In Einheit von 1/4000 der Diagrammbereichsbreite. |
| oben | int | In Einheit von 1/4000 der Diagrammbereichshöhe. |
| rechts | int | In Einheit von 1/4000 der Diagrammbereichsbreite. |
| unten | int | In Einheit von 1/4000 der Diagrammbereichshöhe. |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addShapeInChart(int type, int placement, int left, int top, int right, int bottom, byte[] imageData) {#addShapeInChart-int-int-int-int-int-int-byte---}
```
public Shape addShapeInChart(int type, int placement, int left, int top, int right, int bottom, byte[] imageData)
```


Füge eine Form zum Diagramm hinzu. Alle Einheiten sind 1/4000 des Diagrammbereichs.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Der Zeichnungstyp. |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype). der Platzierungstyp. |
| links | int | In Einheit von 1/4000 der Diagrammbereichsbreite. |
| oben | int | In Einheit von 1/4000 der Diagrammbereichshöhe. |
| rechts | int | In Einheit von 1/4000 der Diagrammbereichsbreite. |
| unten | int | In Einheit von 1/4000 der Diagrammbereichshöhe. |
| imageData | byte[] | Wenn die Form kein Bild oder OLE-Objekt ist, sollte imageData null sein. |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom) {#addShapeInChartByScale-int-int-double-double-double-double-}
```
public Shape addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom)
```


Füge eine Form zum Diagramm hinzu. Alle Einheiten sind prozentuale Skalierung des Diagrammbereichs.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Der Zeichnungstyp. |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype). der Platzierungstyp. |
| links | double | Einheit ist prozentuale Skalierung der Diagrammbereichsbreite. |
| oben | double | Einheit ist prozentuale Skalierung der Diagrammbereichshöhe. |
| rechts | double | Einheit ist prozentuale Skalierung der Diagrammbereichsbreite. |
| unten | double | Einheit ist prozentuale Skalierung der Diagrammbereichshöhe. |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom, byte[] imageData) {#addShapeInChartByScale-int-int-double-double-double-double-byte---}
```
public Shape addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom, byte[] imageData)
```


Füge eine Form zum Diagramm hinzu. Alle Einheiten sind 1/4000 des Diagrammbereichs.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Der Zeichnungstyp. |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype). der Platzierungstyp. |
| links | double | Einheit ist prozentuale Skalierung der Diagrammbereichsbreite. |
| oben | double | Einheit ist prozentuale Skalierung der Diagrammbereichshöhe. |
| rechts | double | Einheit ist prozentuale Skalierung der Diagrammbereichsbreite. |
| unten | double | Einheit ist prozentuale Skalierung der Diagrammbereichshöhe. |
| imageData | byte[] | Wenn die Form kein Bild oder OLE-Objekt ist, sollte imageData null sein. |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addSignatureLine(int topRow, int leftColumn, SignatureLine signatureLine) {#addSignatureLine-int-int-com.aspose.cells.SignatureLine-}
```
public Picture addSignatureLine(int topRow, int leftColumn, SignatureLine signatureLine)
```


Fügt eine Signaturzeile zum Arbeitsblatt hinzu.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | int | Index der oberen linken Zeile. |
| leftColumn | int | Index der oberen linken Spalte. |
| signatureLine | [SignatureLine](../../com.aspose.cells/signatureline) | Stellt ein Signaturlinienobjekt dar. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - 
### addSpinner(int topRow, int top, int leftColumn, int left, int height, int width) {#addSpinner-int-int-int-int-int-int-}
```
public Spinner addSpinner(int topRow, int top, int leftColumn, int left, int height, int width)
```


Fügt einen Spinner zum Arbeitsblatt hinzu.

**Example**

```
         //add a spinner
         Spinner spinner = shapes.addSpinner(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | int | Index der oberen linken Zeile. |
| oben | int | Stellt den vertikalen Versatz von Spinner von seiner linken Zeile dar, in Einheit Pixel. |
| leftColumn | int | Index der oberen linken Spalte. |
| links | int | Stellt den horizontalen Versatz von Spinner von seiner linken Spalte dar, in Einheit Pixel. |
| Höhe | int | Stellt die Höhe von Spinner dar, in Einheit Pixel. |
| Breite | int | Stellt die Breite von Spinner dar, in Einheit Pixel. |

**Returns:**
[Spinner](../../com.aspose.cells/spinner) - A Spinner object.
### addSvg(int topRow, int top, int leftColumn, int left, int height, int width, byte[] svgData, byte[] compatibleImageData) {#addSvg-int-int-int-int-int-int-byte---byte---}
```
public Picture addSvg(int topRow, int top, int leftColumn, int left, int height, int width, byte[] svgData, byte[] compatibleImageData)
```


Fügt ein SVG-Bild hinzu.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | int | Index der oberen linken Zeile. |
| oben | int | Stellt den vertikalen Versatz der Form von ihrer linken Zeile dar, in Pixel. |
| leftColumn | int | Index der oberen linken Spalte. |
| links | int | Der horizontale Versatz der Form von ihrer linken Spalte, in Pixel. |
| Höhe | int | Die Höhe der Form, in Pixel. |
| Breite | int | Die Breite der Form, in Pixel. |
| svgData | byte[] | Die SVG-Bilddaten. |
| compatibleImageData | byte[] | Konvertierte Bilddaten von SVG, um mit Excel 2016 oder älteren Versionen kompatibel zu sein. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - 
### addTextBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addTextBox-int-int-int-int-int-int-}
```
public TextBox addTextBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Fügt ein Textfeld zum Arbeitsblatt hinzu.

**Example**

```
         //add a TextBox
         TextBox textBox = shapes.addTextBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | int | Index der oberen linken Zeile. |
| oben | int | Stellt den vertikalen Versatz des Textfelds von seiner oberen Zeile dar, in Pixel. |
| leftColumn | int | Index der oberen linken Spalte. |
| links | int | Stellt den horizontalen Versatz von textbox von seiner linken Spalte dar, in Pixeln. |
| Höhe | int | Stellt die Höhe des Textfelds dar, in Pixel. |
| Breite | int | Stellt die Breite des Textfelds dar, in Pixel. |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - A [TextBox](../../com.aspose.cells/textbox) object.
### addTextBoxInChart(int top, int left, int height, int width) {#addTextBoxInChart-int-int-int-int-}
```
public TextBox addTextBoxInChart(int top, int left, int height, int width)
```


Fügt ein Textfeld zum Diagramm hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| oben | int | Stellt den vertikalen Versatz von textbox vom oberen linken Eckpunkt in Einheiten von 1/4000 des Diagrammbereichs dar. |
| links | int | Stellt den vertikalen Versatz von textbox vom oberen linken Eckpunkt in Einheiten von 1/4000 des Diagrammbereichs dar. |
| Höhe | int | Stellt die Höhe von textbox dar, in Einheiten von 1/4000 des Diagrammbereichs. |
| Breite | int | Stellt die Breite von textbox dar, in Einheiten von 1/4000 des Diagrammbereichs. |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - A TextBox object.
### addTextEffect(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int topRow, int top, int leftColumn, int left, int height, int width) {#addTextEffect-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-int-int-}
```
public Shape addTextEffect(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int topRow, int top, int leftColumn, int left, int height, int width)
```


Fügt ein WordArt-Objekt ein.

**Example**

```
         //add a WordArt
         Shape wordArt1 = shapes.addTextEffect(MsoPresetTextEffect.TEXT_EFFECT_10, "WordArt", "arial", 18, false, false, 3, 0, 3, 0, 200, 50);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| effect | int | [MsoPresetTextEffect](../../com.aspose.cells/msopresettexteffect). Der mso preset text effect type. |
| Text | java.lang.String | Der WordArt-Text. |
| fontName | java.lang.String | Der Schriftname. |
| Größe | int | Die Schriftgröße |
| fontBold | boolean | Gibt an, ob die Schrift fett ist. |
| fontItalic | boolean | Gibt an, ob die Schrift kursiv ist. |
| topRow | int | Index der oberen linken Zeile. |
| oben | int | Stellt den vertikalen Versatz der Form von ihrer linken Zeile dar, in Pixel. |
| leftColumn | int | Index der oberen linken Spalte. |
| links | int | Stellt den horizontalen Versatz der Form von ihrer linken Spalte dar, in Pixel. |
| Höhe | int | Stellt die Höhe der Form in Pixeln dar. |
| Breite | int | Stellt die Breite der Form dar, in Pixel. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - Returns a Shape object that represents the new WordArt object.
### addTextEffectInChart(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int top, int left, int height, int width) {#addTextEffectInChart-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-}
```
public Shape addTextEffectInChart(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int top, int left, int height, int width)
```


Fügt ein WordArt-Objekt zum Diagramm ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| effect | int | [MsoPresetTextEffect](../../com.aspose.cells/msopresettexteffect). Der mso preset text effect type. |
| Text | java.lang.String | Der WordArt-Text. |
| fontName | java.lang.String | Der Schriftname. |
| Größe | int | Die Schriftgröße |
| fontBold | boolean | Gibt an, ob die Schrift fett ist. |
| fontItalic | boolean | Gibt an, ob die Schrift kursiv ist. |
| oben | int | Stellt den vertikalen Versatz der Form vom oberen linken Eckpunkt in Einheiten von 1/4000 des Diagrammbereichs dar. |
| links | int | Stellt den vertikalen Versatz der Form vom oberen linken Eckpunkt in Einheiten von 1/4000 des Diagrammbereichs dar. |
| Höhe | int | Stellt die Höhe der Form dar, in Einheiten von 1/4000 des Diagrammbereichs. |
| Breite | int | Stellt die Breite der Form dar, in Einheiten von 1/4000 des Diagrammbereichs. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - Returns a Shape object that represents the new WordArt object.
### addWordArt(int style, String text, int topRow, int top, int leftColumn, int left, int height, int width) {#addWordArt-int-java.lang.String-int-int-int-int-int-int-}
```
public Shape addWordArt(int style, String text, int topRow, int top, int leftColumn, int left, int height, int width)
```


Fügt vordefiniertes WordArt seit Excel 2007 hinzu.

**Example**

```
         //add a WordArt
         Shape wordArt2 = shapes.addWordArt(PresetWordArtStyle.WORD_ART_STYLE_1, "WordArt", 3, 0, 3, 0, 50, 200);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). Der preset WordArt Style. |
| Text | java.lang.String | Der Text. |
| topRow | int | Index der oberen linken Zeile. |
| oben | int | Stellt den vertikalen Versatz der Form von ihrer linken Zeile dar, in Pixel. |
| leftColumn | int | Index der oberen linken Spalte. |
| links | int | Stellt den horizontalen Versatz der Form von ihrer linken Spalte dar, in Pixel. |
| Höhe | int | Stellt die Höhe der Form in Pixeln dar. |
| Breite | int | Stellt die Breite der Form dar, in Pixel. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### clear() {#clear--}
```
public void clear()
```


Löscht alle Formen im Arbeitsblatt.

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


Gibt zurück, ob die Instanz dieses Objekt enthält

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | Testobjekt |

**Returns:**
boolean - Ob die Instanz dieses Objekt enthält
### copyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn) {#copyCommentsInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-}
```
public void copyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn)
```


Kopiert alle Kommentare im Bereich.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| shapes | [ShapeCollection](../../com.aspose.cells/shapecollection) | Die Quellformen. |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Der Quellbereich. |
| destRow | int | Die Zielbereich-Startzeile. |
| destColumn | int | Die Zielbereich-Startspalte. |

### copyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, boolean isContained) {#copyInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-boolean-}
```
public void copyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, boolean isContained)
```


Kopiert Formen im Bereich zum Zielbereich.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceShapes | [ShapeCollection](../../com.aspose.cells/shapecollection) | Quellformen. |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Der Quellbereich. |
| destRow | int | Der Zielzeilenindex des Zielbereichs. |
| destColumn | int | Die Zielspalte des Zielbereichs. |
| isContained | boolean | Ob nur die Formen kopiert werden, die im Bereich enthalten sind. Wenn true, werden nur die Formen im Bereich kopiert. Andernfalls funktioniert es wie MS Office. |

### deleteInRange(CellArea ca) {#deleteInRange-com.aspose.cells.CellArea-}
```
public void deleteInRange(CellArea ca)
```


Löscht Formen im Bereich. Kommentarformen werden nicht gelöscht.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | Der Bereich. Wenn die Formen im Bereich enthalten sind, werden sie entfernt. |

### deleteShape(Shape shape) {#deleteShape-com.aspose.cells.Shape-}
```
public void deleteShape(Shape shape)
```


Eine Form löschen. Wenn die Form in der Gruppe ist oder eine Kommentarform ist, wird sie nicht gelöscht.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| shape | [Shape](../../com.aspose.cells/shape) |  |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### find(String what, int previous, FindOptions findOptions) {#find-java.lang.String-int-com.aspose.cells.FindOptions-}
```
public int find(String what, int previous, FindOptions findOptions)
```


Finde Form nach Text

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| was | java.lang.String | Der zu suchende Text. |
| vorherige | int | Der Index der vorherigen Form, die denselben Text enthält. -1, wenn von Anfang an gesucht wird. |
| findOptions | [FindOptions](../../com.aspose.cells/findoptions) | Suchoptionen |

**Returns:**
int - Der Index der gefundenen Form, -1 wenn keine Form gefunden wird.
### get(int index) {#get-int-}
```
public Shape get(int index)
```


Ruft das [Shape](../../com.aspose.cells/shape)-Objekt am bestimmten Index in der Liste ab.

**Example**

```
         //get the first shape
         Shape shape = shapes.get(0);
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der Index. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### get(String name) {#get-java.lang.String-}
```
public Shape get(String name)
```


Ruft das [Shape](../../com.aspose.cells/shape)-Objekt anhand des Namens der Form ab.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | Der Name der Form. |

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


Ermittelt die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente.

**Returns:**
int - Die Anzahl der in der CollectionBase-Instanz enthaltenen Elemente.
### group(Shape[] groupItems) {#group-com.aspose.cells.Shape---}
```
public GroupShape group(Shape[] groupItems)
```


Gruppiere die Formen.

**Remarks**

Die Form in den groupItems sollte nicht gruppiert sein. Die Form muss in dieser Shapes-Sammlung sein.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| groupItems | [Shape\[\]](../../com.aspose.cells/shape) | die Gruppenobjekte. |

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


Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | Bestimmt den Index eines bestimmten Elements in der CollectionBase-Instanz. |

**Returns:**
int - Der Index des Wertes, falls in der Liste gefunden; sonst -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Gibt einen Enumerator zurück, der die CollectionBase-Instanz durchläuft.

**Returns:**
java.util.Iterator - Ein Iterator für die CollectionBase-Instanz.
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


Entferne die Form.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| shape | [Shape](../../com.aspose.cells/shape) |  |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Entferne die Form.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der Index der Form. |

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


Entgruppiert die Formelemente.

**Remarks**

Wenn die Gruppenform von einer anderen Gruppenform gruppiert wird, wird nichts unternommen.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| group | [GroupShape](../../com.aspose.cells/groupshape) | Die Gruppenform. |

### updateSelectedValue() {#updateSelectedValue--}
```
public void updateSelectedValue()
```


Aktualisiert den ausgewählten Wert anhand des Werts der verknüpften Zelle oder des Bereichs der Form.

### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

