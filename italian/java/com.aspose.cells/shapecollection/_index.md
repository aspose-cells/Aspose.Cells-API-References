---
title: "ShapeCollection"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta tutte le forme in un foglio di lavoro/grafico."
type: docs
url: /it/java/com.aspose.cells/shapecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ShapeCollection extends CollectionBase
```

Rappresenta tutte le forme in un foglio di lavoro/grafico.

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
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Aggiunge un elemento all'istanza di CollectionBase. |
| [addActiveXControl(int type, int topRow, int top, int leftColumn, int left, int width, int height)](#addActiveXControl-int-int-int-int-int-int-int-) | Crea un Activex Control. |
| [addArc(int topRow, int top, int leftColumn, int left, int height, int width)](#addArc-int-int-int-int-int-int-) | Aggiunge un ArcShape al foglio di lavoro. |
| [addAutoShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)](#addAutoShape-int-int-int-int-int-int-int-) | Aggiunge un AutoShape al foglio di lavoro. |
| [addAutoShapeInChart(int type, int top, int left, int height, int width)](#addAutoShapeInChart-int-int-int-int-int-) | Aggiunge un AutoShape al grafico. |
| [addButton(int topRow, int top, int leftColumn, int left, int height, int width)](#addButton-int-int-int-int-int-int-) | Aggiunge un Button al foglio di lavoro. |
| [addCheckBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addCheckBox-int-int-int-int-int-int-) | Aggiunge una checkbox al foglio di lavoro. |
| [addComboBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addComboBox-int-int-int-int-int-int-) | Aggiunge un ComboBox al foglio di lavoro. |
| [addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left)](#addCopy-com.aspose.cells.Shape-int-int-int-int-) | Aggiunge e copia una forma al foglio di lavoro. |
| [addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left, CopyOptions copyOptions)](#addCopy-com.aspose.cells.Shape-int-int-int-int-com.aspose.cells.CopyOptions-) | Aggiunge e copia una forma al foglio di lavoro. |
| [addEquation(int topRow, int top, int leftColumn, int left, int height, int width)](#addEquation-int-int-int-int-int-int-) | Aggiunge un oggetto di equazione al foglio di lavoro. |
| [addFreeFloatingShape(int type, int top, int left, int height, int width, byte[] imageData, boolean isOriginalSize)](#addFreeFloatingShape-int-int-int-int-int-byte---boolean-) | Aggiunge una forma fluttuante al foglio di lavoro. Si applica solo per forme linea/immagine. |
| [addFreeform(int topRow, int top, int leftColumn, int left, int height, int width, ShapePath[] paths)](#addFreeform-int-int-int-int-int-int-com.aspose.cells.ShapePath---) | Aggiunge una forma libera al foglio di lavoro. |
| [addGroupBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addGroupBox-int-int-int-int-int-int-) | Aggiunge un GroupBox al foglio di lavoro. |
| [addIcons(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageByteData, byte[] compatibleImageData)](#addIcons-int-int-int-int-int-int-byte---byte---) | Aggiunge un'immagine svg. |
| [addLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, int width, String latex)](#addLaTeXEquation-int-int-int-int-int-int-java.lang.String-) | Aggiunge un oggetto di equazione al foglio di lavoro usando stringhe di formato LaTeX. |
| [addLabel(int topRow, int top, int leftColumn, int left, int height, int width)](#addLabel-int-int-int-int-int-int-) | Aggiunge un Label al foglio di lavoro. |
| [addLabelInChart(int top, int left, int height, int width)](#addLabelInChart-int-int-int-int-) | Aggiunge un label al grafico. |
| [addLine(int topRow, int top, int leftColumn, int left, int height, int width)](#addLine-int-int-int-int-int-int-) | Aggiunge un LineShape al foglio di lavoro. |
| [addLinkedPicture(int topRow, int leftColumn, int height, int width, String sourceFullName)](#addLinkedPicture-int-int-int-int-java.lang.String-) | Aggiungi un'immagine collegata. |
| [addListBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addListBox-int-int-int-int-int-int-) | Aggiunge un ListBox al foglio di lavoro. |
| [addOleObject(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageData)](#addOleObject-int-int-int-int-int-int-byte---) | Aggiunge un OleObject. |
| [addOleObjectWithLinkedImage(int topRow, int leftColumn, int height, int width, String sourceFullName)](#addOleObjectWithLinkedImage-int-int-int-int-java.lang.String-) | Aggiungi un'immagine collegata. |
| [addOval(int topRow, int top, int leftColumn, int left, int height, int width)](#addOval-int-int-int-int-int-int-) | Aggiunge un Oval al foglio di lavoro. |
| [addPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream)](#addPicture-int-int-int-int-java.io.InputStream-) | Aggiunge un'immagine alla collezione. |
| [addPicture(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale)](#addPicture-int-int-java.io.InputStream-int-int-) | Aggiunge un'immagine alla collezione. |
| [addPictureInChart(int top, int left, InputStream stream, int widthScale, int heightScale)](#addPictureInChart-int-int-java.io.InputStream-int-int-) | Aggiunge un'immagine al grafico. |
| [addRadioButton(int topRow, int top, int leftColumn, int left, int height, int width)](#addRadioButton-int-int-int-int-int-int-) | Aggiunge un RadioButton al foglio di lavoro. |
| [addRectangle(int topRow, int top, int leftColumn, int left, int height, int width)](#addRectangle-int-int-int-int-int-int-) | Aggiunge un RectangleShape al foglio di lavoro. |
| [addScrollBar(int topRow, int top, int leftColumn, int left, int height, int width)](#addScrollBar-int-int-int-int-int-int-) | Aggiunge una ScrollBar al foglio di lavoro. |
| [addShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)](#addShape-int-int-int-int-int-int-int-) | Aggiunge una Shape al foglio di lavoro. |
| [addShapeInChart(int type, int placement, int left, int top, int right, int bottom)](#addShapeInChart-int-int-int-int-int-int-) | Aggiungi una forma al grafico. Tutte le unità sono 1/4000 dell'area del grafico. |
| [addShapeInChart(int type, int placement, int left, int top, int right, int bottom, byte[] imageData)](#addShapeInChart-int-int-int-int-int-int-byte---) | Aggiungi una forma al grafico. Tutte le unità sono 1/4000 dell'area del grafico. |
| [addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom)](#addShapeInChartByScale-int-int-double-double-double-double-) | Aggiungi una forma al grafico. |
| [addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom, byte[] imageData)](#addShapeInChartByScale-int-int-double-double-double-double-byte---) | Aggiungi una forma al grafico. Tutte le unità sono 1/4000 dell'area del grafico. |
| [addSignatureLine(int topRow, int leftColumn, SignatureLine signatureLine)](#addSignatureLine-int-int-com.aspose.cells.SignatureLine-) | Aggiunge una Signature Line al foglio di lavoro. |
| [addSpinner(int topRow, int top, int leftColumn, int left, int height, int width)](#addSpinner-int-int-int-int-int-int-) | Aggiunge uno Spinner al foglio di lavoro. |
| [addSvg(int topRow, int top, int leftColumn, int left, int height, int width, byte[] svgData, byte[] compatibleImageData)](#addSvg-int-int-int-int-int-int-byte---byte---) | Aggiunge un'immagine svg. |
| [addTextBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addTextBox-int-int-int-int-int-int-) | Aggiunge una casella di testo al foglio di lavoro. |
| [addTextBoxInChart(int top, int left, int height, int width)](#addTextBoxInChart-int-int-int-int-) | Aggiunge una casella di testo al grafico. |
| [addTextEffect(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int topRow, int top, int leftColumn, int left, int height, int width)](#addTextEffect-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-int-int-) | Inserisce un oggetto WordArt. |
| [addTextEffectInChart(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int top, int left, int height, int width)](#addTextEffectInChart-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-) | Inserisce un oggetto WordArt nel grafico. |
| [addWordArt(int style, String text, int topRow, int top, int leftColumn, int left, int height, int width)](#addWordArt-int-java.lang.String-int-int-int-int-int-int-) | Aggiunge WordArt predefinito da Excel 2007. |
| [clear()](#clear--) | Cancella tutte le forme nel foglio di lavoro. |
| [contains(Object o)](#contains-java.lang.Object-) | Restituisce se l'istanza contiene questo oggetto |
| [copyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn)](#copyCommentsInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-) | Copia tutti i commenti nell'intervallo. |
| [copyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, boolean isContained)](#copyInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-boolean-) | Copia le forme nell'intervallo nell'intervallo di destinazione. |
| [deleteInRange(CellArea ca)](#deleteInRange-com.aspose.cells.CellArea-) | Elimina le forme nell'intervallo. Le forme dei commenti non saranno eliminate. |
| [deleteShape(Shape shape)](#deleteShape-com.aspose.cells.Shape-) | Elimina una forma. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [find(String what, int previous, FindOptions findOptions)](#find-java.lang.String-int-com.aspose.cells.FindOptions-) | Trova la forma per testo. |
| [get(int index)](#get-int-) | Ottiene l'oggetto [Shape](../../com.aspose.cells/shape) all'indice specifico nella lista. |
| [get(String name)](#get-java.lang.String-) | Ottiene l'oggetto [Shape](../../com.aspose.cells/shape) per nome della forma. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ottiene il numero di elementi contenuti nell'istanza di CollectionBase. |
| [group(Shape[] groupItems)](#group-com.aspose.cells.Shape---) | Raggruppa le forme. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determina l'indice di un elemento specifico nell'istanza di CollectionBase. |
| [iterator()](#iterator--) | Restituisce un enumeratore che itera attraverso l'istanza di CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Shape shape)](#remove-com.aspose.cells.Shape-) | Rimuovi la forma. |
| [removeAt(int index)](#removeAt-int-) | Rimuovi la forma. |
| [toString()](#toString--) |  |
| [ungroup(GroupShape group)](#ungroup-com.aspose.cells.GroupShape-) | Separa gli elementi della forma. |
| [updateSelectedValue()](#updateSelectedValue--) | Aggiorna il valore selezionato con il valore della cella collegata o dell'intervallo della forma. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Aggiunge un elemento all'istanza di CollectionBase.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | java.lang.Object | L'Object da aggiungere all'istanza di CollectionBase. |

**Returns:**
int - La posizione in cui è stato inserito il nuovo elemento.
### addActiveXControl(int type, int topRow, int top, int leftColumn, int left, int width, int height) {#addActiveXControl-int-int-int-int-int-int-int-}
```
public Shape addActiveXControl(int type, int topRow, int top, int leftColumn, int left, int width, int height)
```


Crea un Activex Control.

**Example**

```
         //add an ActiveX control
         Shape activeXControl = shapes.addActiveXControl(com.aspose.cells.ControlType.CHECK_BOX, 1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | int | [ControlType](../../com.aspose.cells/controltype). Il tipo del controllo. |
| topRow | int | Indice della riga in alto a sinistra. |
| superiore | int | Rappresenta lo spostamento verticale della Shape dalla sua riga sinistra, in unità di pixel. |
| leftColumn | int | Indice della colonna in alto a sinistra. |
| sinistra | int | Rappresenta lo spostamento orizzontale della Shape dalla sua colonna sinistra, in unità di pixel. |
| larghezza | int | Rappresenta la larghezza della Shape, in unità di pixel. |
| altezza | int | Rappresenta l'altezza della Shape, in unità di pixel. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### addArc(int topRow, int top, int leftColumn, int left, int height, int width) {#addArc-int-int-int-int-int-int-}
```
public ArcShape addArc(int topRow, int top, int leftColumn, int left, int height, int width)
```


Aggiunge un ArcShape al foglio di lavoro.

**Example**

```
         //add a arc
         ArcShape arcShape = shapes.addArc(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | int | Indice della riga in alto a sinistra. |
| superiore | int | Rappresenta lo spostamento verticale dell'ArcShape dalla sua riga sinistra, in unità di pixel. |
| leftColumn | int | Indice della colonna in alto a sinistra. |
| sinistra | int | Rappresenta lo spostamento orizzontale dell'ArcShape dalla sua colonna sinistra, in unità di pixel. |
| altezza | int | Rappresenta l'altezza dell'ArcShape, in unità di pixel. |
| larghezza | int | Rappresenta la larghezza dell'ArcShape, in unità di pixel. |

**Returns:**
[ArcShape](../../com.aspose.cells/arcshape) - A ArcShape object.
### addAutoShape(int type, int topRow, int top, int leftColumn, int left, int height, int width) {#addAutoShape-int-int-int-int-int-int-int-}
```
public Shape addAutoShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)
```


Aggiunge un AutoShape al foglio di lavoro.

**Remarks**

Il tipo non può essere Chart/Comment/Picture/OleObject/Polygon/DialogBox

**Example**

```
         //Adds a AutoShape to the worksheet.
         Shape autoShape = shapes.addAutoShape(AutoShapeType.CUBE, 1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | int | [AutoShapeType](../../com.aspose.cells/autoshapetype). Tipo di forma automatica. |
| topRow | int | Indice della riga in alto a sinistra. |
| superiore | int | Rappresenta lo spostamento verticale della Shape dalla sua riga sinistra, in unità di pixel. |
| leftColumn | int | Indice della colonna in alto a sinistra. |
| sinistra | int | Rappresenta lo spostamento orizzontale della Shape dalla sua colonna sinistra, in unità di pixel. |
| altezza | int | Rappresenta l'altezza della Shape, in unità di pixel. |
| larghezza | int | Rappresenta la larghezza della Shape, in unità di pixel. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - A Shape object.
### addAutoShapeInChart(int type, int top, int left, int height, int width) {#addAutoShapeInChart-int-int-int-int-int-}
```
public Shape addAutoShapeInChart(int type, int top, int left, int height, int width)
```


Aggiunge un AutoShape al grafico.

**Remarks**

Il tipo non può essere Chart/Comment/Picture/OleObject/Polygon/DialogBox

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | int | [AutoShapeType](../../com.aspose.cells/autoshapetype). Tipo di forma automatica. |
| superiore | int | Rappresenta lo spostamento verticale della textbox dall'angolo superiore sinistro in unità di 1/4000 dell'area del grafico. |
| sinistra | int | Rappresenta lo spostamento verticale della textbox dall'angolo superiore sinistro in unità di 1/4000 dell'area del grafico. |
| altezza | int | Rappresenta l'altezza della textbox, in unità di 1/4000 dell'area del grafico. |
| larghezza | int | Rappresenta la larghezza della textbox, in unità di 1/4000 dell'area del grafico. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - Returns a shape object.
### addButton(int topRow, int top, int leftColumn, int left, int height, int width) {#addButton-int-int-int-int-int-int-}
```
public Button addButton(int topRow, int top, int leftColumn, int left, int height, int width)
```


Aggiunge un Button al foglio di lavoro.

**Example**

```
         //add a button
         Button button = shapes.addButton(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | int | Indice della riga in alto a sinistra. |
| superiore | int | Rappresenta lo spostamento verticale del Button dalla sua riga sinistra, in unità di pixel. |
| leftColumn | int | Indice della colonna in alto a sinistra. |
| sinistra | int | Rappresenta lo spostamento orizzontale del Button dalla sua colonna sinistra, in unità di pixel. |
| altezza | int | Rappresenta l'altezza del Button, in unità di pixel. |
| larghezza | int | Rappresenta la larghezza del Button, in unità di pixel. |

**Returns:**
[Button](../../com.aspose.cells/button) - A Button object.
### addCheckBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addCheckBox-int-int-int-int-int-int-}
```
public CheckBox addCheckBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Aggiunge una checkbox al foglio di lavoro.

**Example**

```
         //add a CheckBox
         CheckBox checkBox = shapes.addCheckBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | int | Indice della riga in alto a sinistra. |
| superiore | int | Rappresenta lo spostamento verticale del checkbox dalla sua riga superiore, in unità di pixel. |
| leftColumn | int | Indice della colonna in alto a sinistra. |
| sinistra | int | Rappresenta lo spostamento orizzontale della textbox dalla sua colonna sinistra, in unità di pixel. |
| altezza | int | Altezza della textbox, in unità di pixel. |
| larghezza | int | Larghezza della textbox, in unità di pixel. |

**Returns:**
[CheckBox](../../com.aspose.cells/checkbox) - The new CheckBox object index.
### addComboBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addComboBox-int-int-int-int-int-int-}
```
public ComboBox addComboBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Aggiunge un ComboBox al foglio di lavoro.

**Example**

```
         //add a combo box
         ComboBox comboBox = shapes.addComboBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | int | Indice della riga in alto a sinistra. |
| superiore | int | Rappresenta lo spostamento verticale del ComboBox dalla sua riga sinistra, in unità di pixel. |
| leftColumn | int | Indice della colonna in alto a sinistra. |
| sinistra | int | Rappresenta lo spostamento orizzontale del ComboBox dalla sua colonna sinistra, in unità di pixel. |
| altezza | int | Rappresenta l'altezza del ComboBox, in unità di pixel. |
| larghezza | int | Rappresenta la larghezza del ComboBox, in unità di pixel. |

**Returns:**
[ComboBox](../../com.aspose.cells/combobox) - A ComboBox object.
### addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left) {#addCopy-com.aspose.cells.Shape-int-int-int-int-}
```
public Shape addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left)
```


Aggiunge e copia una forma al foglio di lavoro.

**Example**

```
         //add a shape
         RectangleShape rectangle = shapes.addRectangle(2, 0, 2, 0, 130, 130);
         //Adds and copies a shape.
         shapes.addCopy(rectangle, 7, 0, 7, 0);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceShape | [Shape](../../com.aspose.cells/shape) | Forma di origine. |
| topRow | int | L'indice della riga superiore. |
| superiore | int | Rappresenta lo spostamento verticale dalla sua riga superiore, in unità di pixel. |
| leftColumn | int | L'indice della colonna sinistra. |
| sinistra | int | Rappresenta lo spostamento orizzontale dalla sua colonna sinistra, in unità di pixel. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - The new [Shape](../../com.aspose.cells/shape) object.
### addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left, CopyOptions copyOptions) {#addCopy-com.aspose.cells.Shape-int-int-int-int-com.aspose.cells.CopyOptions-}
```
public Shape addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left, CopyOptions copyOptions)
```


Aggiunge e copia una forma al foglio di lavoro.

**Example**

```
         //add a shape
         RectangleShape rectangle = shapes.addRectangle(2, 0, 2, 0, 130, 130);
         //Adds and copies a shape.
         shapes.addCopy(rectangle, 7, 0, 7, 0);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceShape | [Shape](../../com.aspose.cells/shape) | Forma di origine. |
| topRow | int | L'indice della riga superiore. |
| superiore | int | Rappresenta lo spostamento verticale dalla sua riga superiore, in unità di pixel. |
| leftColumn | int | L'indice della colonna sinistra. |
| sinistra | int | Rappresenta lo spostamento orizzontale dalla sua colonna sinistra, in unità di pixel. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | Le opzioni di copia delle forme. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - The new [Shape](../../com.aspose.cells/shape) object.
### addEquation(int topRow, int top, int leftColumn, int left, int height, int width) {#addEquation-int-int-int-int-int-int-}
```
public TextBox addEquation(int topRow, int top, int leftColumn, int left, int height, int width)
```


Aggiunge un oggetto di equazione al foglio di lavoro.

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | int | L'indice della riga superiore. |
| superiore | int | Lo spostamento verticale della sua riga superiore, in unità di pixel. |
| leftColumn | int | L'indice della colonna sinistra. |
| sinistra | int | Lo spostamento orizzontale dalla sua colonna sinistra, in unità di pixel. |
| altezza | int | L'altezza dell'equazione, in unità di pixel. |
| larghezza | int | La larghezza dell'equazione, in unità di pixel. |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - 
### addFreeFloatingShape(int type, int top, int left, int height, int width, byte[] imageData, boolean isOriginalSize) {#addFreeFloatingShape-int-int-int-int-int-byte---boolean-}
```
public Shape addFreeFloatingShape(int type, int top, int left, int height, int width, byte[] imageData, boolean isOriginalSize)
```


Aggiunge una forma fluttuante al foglio di lavoro. Si applica solo per forme linea/immagine.

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Il tipo di forma. |
| superiore | int | Rappresenta lo spostamento verticale della forma dalla riga superiore del foglio di lavoro, in unità di pixel. |
| sinistra | int | Rappresenta lo spostamento orizzontale della forma dalla colonna sinistra del foglio di lavoro, in unità di pixel. |
| altezza | int | Rappresenta l'altezza di LineShape, in unità di pixel. |
| larghezza | int | Rappresenta la larghezza di LineShape, in unità di pixel. |
| imageData | byte[] | I dati dell'immagine, si applicano solo all'immagine. |
| isOriginalSize | boolean | Indica se la forma utilizza le dimensioni originali se la forma è un'immagine. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### addFreeform(int topRow, int top, int leftColumn, int left, int height, int width, ShapePath[] paths) {#addFreeform-int-int-int-int-int-int-com.aspose.cells.ShapePath---}
```
public Shape addFreeform(int topRow, int top, int leftColumn, int left, int height, int width, ShapePath[] paths)
```


Aggiunge una forma libera al foglio di lavoro.

**Remarks**

Nota: la larghezza e l'altezza nei parametri possono essere qualsiasi valore intero positivo, non la larghezza e l'altezza totali dell'array ShapePath specificato da \u9225\u6a96aths'. La relazione tra di essi è una relazione di scala-riempimento, cioè ogni oggetto ShapePath verrà scalato in base alla larghezza e all'altezza. Pertanto, quando ci sono più oggetti nei 'paths', ogni oggetto ShapePath deve essere progettato in modo ragionevole per soddisfare le aspettative. Quando c'è un solo oggetto ShapePath e non ci sono altri requisiti, passare la larghezza e l'altezza dell'oggetto come valori dei parametri \u9225\u5b27\u20ac\u5a94s è una buona soluzione.

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | int | Indice della riga in alto a sinistra. |
| superiore | int | Rappresenta lo spostamento verticale della forma libera dalla sua riga sinistra, in unità di pixel. |
| leftColumn | int | Indice della colonna in alto a sinistra. |
| sinistra | int | Rappresenta lo spostamento orizzontale della forma libera dalla sua colonna sinistra, in unità di pixel. |
| altezza | int | Rappresenta l'altezza della forma libera, in unità di pixel. |
| larghezza | int | Rappresenta la larghezza della forma libera, in unità di pixel. |
| paths | [ShapePath\[\]](../../com.aspose.cells/shapepath) | Rappresenta un percorso definito dall'utente |

**Returns:**
[Shape](../../com.aspose.cells/shape) - A freeform shape.
### addGroupBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addGroupBox-int-int-int-int-int-int-}
```
public GroupBox addGroupBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Aggiunge un GroupBox al foglio di lavoro.

**Example**

```
         //add a group box
         GroupBox groupBox = shapes.addGroupBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | int | Indice della riga in alto a sinistra. |
| superiore | int | Rappresenta lo spostamento verticale del GroupBox dalla sua riga sinistra, in unità di pixel. |
| leftColumn | int | Indice della colonna in alto a sinistra. |
| sinistra | int | Rappresenta lo spostamento orizzontale del GroupBox dalla sua colonna sinistra, in unità di pixel. |
| altezza | int | Rappresenta l'altezza del GroupBox, in unità di pixel. |
| larghezza | int | Rappresenta la larghezza del GroupBox, in unità di pixel. |

**Returns:**
[GroupBox](../../com.aspose.cells/groupbox) - A GroupBox object.
### addIcons(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageByteData, byte[] compatibleImageData) {#addIcons-int-int-int-int-int-int-byte---byte---}
```
public Picture addIcons(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageByteData, byte[] compatibleImageData)
```


Aggiunge un'immagine svg.

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | int | Indice della riga in alto a sinistra. |
| superiore | int | Rappresenta lo spostamento verticale della forma dalla sua riga sinistra, in unità di pixel. |
| leftColumn | int | Indice della colonna in alto a sinistra. |
| sinistra | int | Lo spostamento orizzontale della forma dalla sua colonna sinistra, in unità di pixel. |
| altezza | int | L'altezza della forma, in unità di pixel. |
| larghezza | int | La larghezza della forma, in unità di pixel. |
| imageByteData | byte[] | I dati byte dell'immagine. |
| compatibleImageData | byte[] | Dati immagine convertiti da SVG per essere compatibili con Excel 2016 o versioni precedenti. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - 
### addLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, int width, String latex) {#addLaTeXEquation-int-int-int-int-int-int-java.lang.String-}
```
public TextBox addLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, int width, String latex)
```


Aggiunge un oggetto di equazione al foglio di lavoro usando stringhe di formato LaTeX.

**Example**

```
         // LaTeX format string.
         String latex = "\\alpha +  \\frac{\\partial^2}{\\partial x_1\\partial x_2}y - \\left ( a + b \\right )+_{a}^{b}\\beta";
         // Adds an equation object to the worksheet.
         TextBox textBox = shapes.addLaTeXEquation(1, 0, 1, 0, 100, 300, latex);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | int | L'indice della riga superiore. |
| superiore | int | Lo spostamento verticale della sua riga superiore, in unità di pixel. |
| leftColumn | int | L'indice della colonna sinistra. |
| sinistra | int | Lo spostamento orizzontale dalla sua colonna sinistra, in unità di pixel. |
| altezza | int | L'altezza dell'equazione, in unità di pixel. |
| larghezza | int | La larghezza dell'equazione, in unità di pixel. |
| latex | java.lang.String | Stringa di formato LaTeX |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - 
### addLabel(int topRow, int top, int leftColumn, int left, int height, int width) {#addLabel-int-int-int-int-int-int-}
```
public Label addLabel(int topRow, int top, int leftColumn, int left, int height, int width)
```


Aggiunge un Label al foglio di lavoro.

**Example**

```
         //add a label
         Label label = shapes.addLabel(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | int | Indice della riga in alto a sinistra. |
| superiore | int | Rappresenta lo spostamento verticale del Label dalla sua riga sinistra, in unità di pixel. |
| leftColumn | int | Indice della colonna in alto a sinistra. |
| sinistra | int | Rappresenta lo spostamento orizzontale del Label dalla sua colonna sinistra, in unità di pixel. |
| altezza | int | Rappresenta l'altezza del Label, in unità di pixel. |
| larghezza | int | Rappresenta la larghezza del Label, in unità di pixel. |

**Returns:**
[Label](../../com.aspose.cells/label) - A Label object.
### addLabelInChart(int top, int left, int height, int width) {#addLabelInChart-int-int-int-int-}
```
public Label addLabelInChart(int top, int left, int height, int width)
```


Aggiunge un label al grafico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| superiore | int | Rappresenta lo spostamento verticale dell'etichetta dall'angolo in alto a sinistra in unità di 1/4000 dell'area del grafico. |
| sinistra | int | Rappresenta lo spostamento verticale dell'etichetta dall'angolo in alto a sinistra in unità di 1/4000 dell'area del grafico. |
| altezza | int | Rappresenta l'altezza dell'etichetta, in unità di 1/4000 dell'area del grafico. |
| larghezza | int | Rappresenta la larghezza dell'etichetta, in unità di 1/4000 dell'area del grafico. |

**Returns:**
[Label](../../com.aspose.cells/label) - A new Label object.
### addLine(int topRow, int top, int leftColumn, int left, int height, int width) {#addLine-int-int-int-int-int-int-}
```
public LineShape addLine(int topRow, int top, int leftColumn, int left, int height, int width)
```


Aggiunge un LineShape al foglio di lavoro.

**Example**

```
         // add a line object
         LineShape lineShape = shapes.addLine(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | int | Indice della riga in alto a sinistra. |
| superiore | int | Rappresenta lo spostamento verticale del LineShape dalla sua riga sinistra, in unità di pixel. |
| leftColumn | int | Indice della colonna in alto a sinistra. |
| sinistra | int | Rappresenta lo spostamento orizzontale del LineShape dalla sua colonna sinistra, in unità di pixel. |
| altezza | int | Rappresenta l'altezza di LineShape, in unità di pixel. |
| larghezza | int | Rappresenta la larghezza di LineShape, in unità di pixel. |

**Returns:**
[LineShape](../../com.aspose.cells/lineshape) - A LineShape object.
### addLinkedPicture(int topRow, int leftColumn, int height, int width, String sourceFullName) {#addLinkedPicture-int-int-int-int-java.lang.String-}
```
public Picture addLinkedPicture(int topRow, int leftColumn, int height, int width, String sourceFullName)
```


Aggiungi un'immagine collegata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | int | Indice della riga in alto a sinistra. |
| leftColumn | int | Indice della colonna in alto a sinistra. |
| altezza | int | L'altezza della forma. In unità di pixel. |
| larghezza | int | La larghezza della forma. In unità di pixel |
| sourceFullName | java.lang.String | Il percorso e il nome del file sorgente per l'immagine collegata |

**Returns:**
[Picture](../../com.aspose.cells/picture) - [Picture](../../com.aspose.cells/picture) Picture object.
### addListBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addListBox-int-int-int-int-int-int-}
```
public ListBox addListBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Aggiunge un ListBox al foglio di lavoro.

**Example**

```
         //add a list box
         ListBox listBox = shapes.addListBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | int | Indice della riga in alto a sinistra. |
| superiore | int | Rappresenta lo spostamento verticale di ListBox dalla sua riga sinistra, in unità di pixel. |
| leftColumn | int | Indice della colonna in alto a sinistra. |
| sinistra | int | Rappresenta lo spostamento orizzontale di ListBox dalla sua colonna sinistra, in unità di pixel. |
| altezza | int | Rappresenta l'altezza di ListBox, in unità di pixel. |
| larghezza | int | Rappresenta la larghezza di ListBox, in unità di pixel. |

**Returns:**
[ListBox](../../com.aspose.cells/listbox) - A ListBox object.
### addOleObject(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageData) {#addOleObject-int-int-int-int-int-int-byte---}
```
public OleObject addOleObject(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageData)
```


Aggiunge un OleObject.

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | int |  |
| superiore | int |  |
| leftColumn | int |  |
| sinistra | int |  |
| altezza | int |  |
| larghezza | int |  |
| imageData | byte[] |  |

**Returns:**
[OleObject](../../com.aspose.cells/oleobject) - 
### addOleObjectWithLinkedImage(int topRow, int leftColumn, int height, int width, String sourceFullName) {#addOleObjectWithLinkedImage-int-int-int-int-java.lang.String-}
```
public OleObject addOleObjectWithLinkedImage(int topRow, int leftColumn, int height, int width, String sourceFullName)
```


Aggiungi un'immagine collegata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | int | Indice della riga in alto a sinistra. |
| leftColumn | int | Indice della colonna in alto a sinistra. |
| altezza | int | L'altezza della forma. In unità di pixel. |
| larghezza | int | La larghezza della forma. In unità di pixel |
| sourceFullName | java.lang.String | Il percorso e il nome del file sorgente per l'immagine collegata |

**Returns:**
[OleObject](../../com.aspose.cells/oleobject) - [Picture](../../com.aspose.cells/picture) Picture object.
### addOval(int topRow, int top, int leftColumn, int left, int height, int width) {#addOval-int-int-int-int-int-int-}
```
public Oval addOval(int topRow, int top, int leftColumn, int left, int height, int width)
```


Aggiunge un Oval al foglio di lavoro.

**Example**

```
         //add a oval
         Oval oval = shapes.addOval(1, 0, 1, 0, 50, 50);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | int | Indice della riga in alto a sinistra. |
| superiore | int | Rappresenta lo spostamento verticale di Oval dalla sua riga sinistra, in unità di pixel. |
| leftColumn | int | Indice della colonna in alto a sinistra. |
| sinistra | int | Rappresenta lo spostamento orizzontale di Oval dalla sua colonna sinistra, in unità di pixel. |
| altezza | int | Rappresenta l'altezza di Oval, in unità di pixel. |
| larghezza | int | Rappresenta la larghezza di Oval, in unità di pixel. |

**Returns:**
[Oval](../../com.aspose.cells/oval) - A Oval object.
### addPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream) {#addPicture-int-int-int-int-java.io.InputStream-}
```
public Picture addPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream)
```


Aggiunge un'immagine alla collezione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | int | Indice della riga in alto a sinistra. |
| leftColumn | int | Indice della colonna in alto a sinistra. |
| bottomRow | int | Indice della riga in basso a destra |
| rightColumn | int | Indice della colonna in basso a destra |
| stream | java.io.InputStream | Oggetto stream che contiene i dati dell'immagine. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - [Picture](../../com.aspose.cells/picture) Picture object.
### addPicture(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale) {#addPicture-int-int-java.io.InputStream-int-int-}
```
public Picture addPicture(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale)
```


Aggiunge un'immagine alla collezione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | int | Indice della riga in alto a sinistra. |
| leftColumn | int | Indice della colonna in alto a sinistra. |
| stream | java.io.InputStream | Oggetto stream che contiene i dati dell'immagine. |
| widthScale | int | Scala della larghezza dell'immagine, in percentuale. |
| heightScale | int | Scala dell'altezza dell'immagine, in percentuale. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - [Picture](../../com.aspose.cells/picture) Picture object.
### addPictureInChart(int top, int left, InputStream stream, int widthScale, int heightScale) {#addPictureInChart-int-int-java.io.InputStream-int-int-}
```
public Picture addPictureInChart(int top, int left, InputStream stream, int widthScale, int heightScale)
```


Aggiunge un'immagine al grafico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| superiore | int | Rappresenta lo spostamento verticale della forma dall'angolo in alto a sinistra in unità di 1/4000 dell'area del grafico. |
| sinistra | int | Rappresenta lo spostamento orizzontale della forma dall'angolo in alto a sinistra in unità di 1/4000 dell'area del grafico. |
| stream | java.io.InputStream | Oggetto stream che contiene i dati dell'immagine. |
| widthScale | int | Scala della larghezza dell'immagine, in percentuale. |
| heightScale | int | Scala dell'altezza dell'immagine, in percentuale. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns a Picture object.
### addRadioButton(int topRow, int top, int leftColumn, int left, int height, int width) {#addRadioButton-int-int-int-int-int-int-}
```
public RadioButton addRadioButton(int topRow, int top, int leftColumn, int left, int height, int width)
```


Aggiunge un RadioButton al foglio di lavoro.

**Example**

```
         //add a radio button
         RadioButton radioButton = shapes.addRadioButton(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | int | Indice della riga in alto a sinistra. |
| superiore | int | Rappresenta lo spostamento verticale di RadioButton dalla sua riga sinistra, in unità di pixel. |
| leftColumn | int | Indice della colonna in alto a sinistra. |
| sinistra | int | Rappresenta lo spostamento orizzontale di RadioButton dalla sua colonna sinistra, in unità di pixel. |
| altezza | int | Rappresenta l'altezza di RadioButton, in unità di pixel. |
| larghezza | int | Rappresenta la larghezza di RadioButton, in unità di pixel. |

**Returns:**
[RadioButton](../../com.aspose.cells/radiobutton) - A RadioButton object.
### addRectangle(int topRow, int top, int leftColumn, int left, int height, int width) {#addRectangle-int-int-int-int-int-int-}
```
public RectangleShape addRectangle(int topRow, int top, int leftColumn, int left, int height, int width)
```


Aggiunge un RectangleShape al foglio di lavoro.

**Example**

```
         // add a rectangle
         RectangleShape rectangleShape = shapes.addRectangle(2, 0, 2, 0, 130, 130);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | int | Indice della riga in alto a sinistra. |
| superiore | int | Rappresenta lo spostamento verticale di RectangleShape dalla sua riga sinistra, in unità di pixel. |
| leftColumn | int | Indice della colonna in alto a sinistra. |
| sinistra | int | Rappresenta lo spostamento orizzontale di RectangleShape dalla sua colonna sinistra, in unità di pixel. |
| altezza | int | Rappresenta l'altezza di RectangleShape, in unità di pixel. |
| larghezza | int | Rappresenta la larghezza di RectangleShape, in unità di pixel. |

**Returns:**
[RectangleShape](../../com.aspose.cells/rectangleshape) - A RectangleShape object.
### addScrollBar(int topRow, int top, int leftColumn, int left, int height, int width) {#addScrollBar-int-int-int-int-int-int-}
```
public ScrollBar addScrollBar(int topRow, int top, int leftColumn, int left, int height, int width)
```


Aggiunge una ScrollBar al foglio di lavoro.

**Example**

```
         //add a scroll bar
         ScrollBar scrollBar = shapes.addScrollBar(1, 0, 1, 0, 100, 20);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | int | Indice della riga in alto a sinistra. |
| superiore | int | Rappresenta lo spostamento verticale della ScrollBar dalla sua riga sinistra, in unità di pixel. |
| leftColumn | int | Indice della colonna in alto a sinistra. |
| sinistra | int | Rappresenta lo spostamento orizzontale della ScrollBar dalla sua colonna sinistra, in unità di pixel. |
| altezza | int | Rappresenta l'altezza della ScrollBar, in unità di pixel. |
| larghezza | int | Rappresenta la larghezza della ScrollBar, in unità di pixel. |

**Returns:**
[ScrollBar](../../com.aspose.cells/scrollbar) - A ScrollBar object.
### addShape(int type, int topRow, int top, int leftColumn, int left, int height, int width) {#addShape-int-int-int-int-int-int-int-}
```
public Shape addShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)
```


Aggiunge una Shape al foglio di lavoro.

**Remarks**

Il tipo non può essere Chart/Comment/Picture/OleObject/Polygon/DialogBox

**Example**

```
         //Add a shape of the specified type
         Shape shapeByType = shapes.addShape(MsoDrawingType.CELLS_DRAWING, 1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Tipo di disegno Mso. |
| topRow | int | Indice della riga in alto a sinistra. |
| superiore | int | Rappresenta lo spostamento verticale della Shape dalla sua riga sinistra, in unità di pixel. |
| leftColumn | int | Indice della colonna in alto a sinistra. |
| sinistra | int | Rappresenta lo spostamento orizzontale della Shape dalla sua colonna sinistra, in unità di pixel. |
| altezza | int | Rappresenta l'altezza della Shape, in unità di pixel. |
| larghezza | int | Rappresenta la larghezza della Shape, in unità di pixel. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - A Shape object.
### addShapeInChart(int type, int placement, int left, int top, int right, int bottom) {#addShapeInChart-int-int-int-int-int-int-}
```
public Shape addShapeInChart(int type, int placement, int left, int top, int right, int bottom)
```


Aggiungi una forma al grafico. Tutte le unità sono 1/4000 dell'area del grafico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Il tipo di disegno. |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype). il tipo di posizionamento. |
| sinistra | int | In unità di 1/4000 della larghezza dell'area del grafico. |
| superiore | int | In unità di 1/4000 dell'altezza dell'area del grafico. |
| destra | int | In unità di 1/4000 della larghezza dell'area del grafico. |
| in basso | int | In unità di 1/4000 dell'altezza dell'area del grafico. |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addShapeInChart(int type, int placement, int left, int top, int right, int bottom, byte[] imageData) {#addShapeInChart-int-int-int-int-int-int-byte---}
```
public Shape addShapeInChart(int type, int placement, int left, int top, int right, int bottom, byte[] imageData)
```


Aggiungi una forma al grafico. Tutte le unità sono 1/4000 dell'area del grafico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Il tipo di disegno. |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype). il tipo di posizionamento. |
| sinistra | int | In unità di 1/4000 della larghezza dell'area del grafico. |
| superiore | int | In unità di 1/4000 dell'altezza dell'area del grafico. |
| destra | int | In unità di 1/4000 della larghezza dell'area del grafico. |
| in basso | int | In unità di 1/4000 dell'altezza dell'area del grafico. |
| imageData | byte[] | Se la forma non è un'immagine o un oggetto ole, imageData dovrebbe essere null. |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom) {#addShapeInChartByScale-int-int-double-double-double-double-}
```
public Shape addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom)
```


Aggiungi una forma al grafico. Tutte le unità sono in scala percentuale dell'area del grafico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Il tipo di disegno. |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype). il tipo di posizionamento. |
| sinistra | double | L'unità è in scala percentuale della larghezza dell'area del grafico. |
| superiore | double | L'unità è in scala percentuale dell'altezza dell'area del grafico. |
| destra | double | L'unità è in scala percentuale della larghezza dell'area del grafico. |
| in basso | double | L'unità è in scala percentuale dell'altezza dell'area del grafico. |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom, byte[] imageData) {#addShapeInChartByScale-int-int-double-double-double-double-byte---}
```
public Shape addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom, byte[] imageData)
```


Aggiungi una forma al grafico. Tutte le unità sono 1/4000 dell'area del grafico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Il tipo di disegno. |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype). il tipo di posizionamento. |
| sinistra | double | L'unità è in scala percentuale della larghezza dell'area del grafico. |
| superiore | double | L'unità è in scala percentuale dell'altezza dell'area del grafico. |
| destra | double | L'unità è in scala percentuale della larghezza dell'area del grafico. |
| in basso | double | L'unità è in scala percentuale dell'altezza dell'area del grafico. |
| imageData | byte[] | Se la forma non è un'immagine o un oggetto ole, imageData dovrebbe essere null. |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addSignatureLine(int topRow, int leftColumn, SignatureLine signatureLine) {#addSignatureLine-int-int-com.aspose.cells.SignatureLine-}
```
public Picture addSignatureLine(int topRow, int leftColumn, SignatureLine signatureLine)
```


Aggiunge una Signature Line al foglio di lavoro.

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | int | Indice della riga in alto a sinistra. |
| leftColumn | int | Indice della colonna in alto a sinistra. |
| signatureLine | [SignatureLine](../../com.aspose.cells/signatureline) | Rappresenta un oggetto linea di firma. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - 
### addSpinner(int topRow, int top, int leftColumn, int left, int height, int width) {#addSpinner-int-int-int-int-int-int-}
```
public Spinner addSpinner(int topRow, int top, int leftColumn, int left, int height, int width)
```


Aggiunge uno Spinner al foglio di lavoro.

**Example**

```
         //add a spinner
         Spinner spinner = shapes.addSpinner(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | int | Indice della riga in alto a sinistra. |
| superiore | int | Rappresenta lo spostamento verticale dello Spinner dalla sua riga sinistra, in unità di pixel. |
| leftColumn | int | Indice della colonna in alto a sinistra. |
| sinistra | int | Rappresenta lo spostamento orizzontale dello Spinner dalla sua colonna sinistra, in unità di pixel. |
| altezza | int | Rappresenta l'altezza dello Spinner, in unità di pixel. |
| larghezza | int | Rappresenta la larghezza dello Spinner, in unità di pixel. |

**Returns:**
[Spinner](../../com.aspose.cells/spinner) - A Spinner object.
### addSvg(int topRow, int top, int leftColumn, int left, int height, int width, byte[] svgData, byte[] compatibleImageData) {#addSvg-int-int-int-int-int-int-byte---byte---}
```
public Picture addSvg(int topRow, int top, int leftColumn, int left, int height, int width, byte[] svgData, byte[] compatibleImageData)
```


Aggiunge un'immagine svg.

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | int | Indice della riga in alto a sinistra. |
| superiore | int | Rappresenta lo spostamento verticale della forma dalla sua riga sinistra, in unità di pixel. |
| leftColumn | int | Indice della colonna in alto a sinistra. |
| sinistra | int | Lo spostamento orizzontale della forma dalla sua colonna sinistra, in unità di pixel. |
| altezza | int | L'altezza della forma, in unità di pixel. |
| larghezza | int | La larghezza della forma, in unità di pixel. |
| svgData | byte[] | I dati dell'immagine svg. |
| compatibleImageData | byte[] | Dati immagine convertiti da SVG per essere compatibili con Excel 2016 o versioni precedenti. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - 
### addTextBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addTextBox-int-int-int-int-int-int-}
```
public TextBox addTextBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Aggiunge una casella di testo al foglio di lavoro.

**Example**

```
         //add a TextBox
         TextBox textBox = shapes.addTextBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | int | Indice della riga in alto a sinistra. |
| superiore | int | Rappresenta lo spostamento verticale della textbox dalla sua riga superiore, in unità di pixel. |
| leftColumn | int | Indice della colonna in alto a sinistra. |
| sinistra | int | Rappresenta lo spostamento orizzontale della textbox dalla sua colonna sinistra, in unità di pixel. |
| altezza | int | Rappresenta l'altezza della casella di testo, in unità di pixel. |
| larghezza | int | Rappresenta la larghezza della casella di testo, in unità di pixel. |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - A [TextBox](../../com.aspose.cells/textbox) object.
### addTextBoxInChart(int top, int left, int height, int width) {#addTextBoxInChart-int-int-int-int-}
```
public TextBox addTextBoxInChart(int top, int left, int height, int width)
```


Aggiunge una casella di testo al grafico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| superiore | int | Rappresenta lo spostamento verticale della textbox dall'angolo superiore sinistro in unità di 1/4000 dell'area del grafico. |
| sinistra | int | Rappresenta lo spostamento verticale della textbox dall'angolo superiore sinistro in unità di 1/4000 dell'area del grafico. |
| altezza | int | Rappresenta l'altezza della textbox, in unità di 1/4000 dell'area del grafico. |
| larghezza | int | Rappresenta la larghezza della textbox, in unità di 1/4000 dell'area del grafico. |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - A TextBox object.
### addTextEffect(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int topRow, int top, int leftColumn, int left, int height, int width) {#addTextEffect-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-int-int-}
```
public Shape addTextEffect(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int topRow, int top, int leftColumn, int left, int height, int width)
```


Inserisce un oggetto WordArt.

**Example**

```
         //add a WordArt
         Shape wordArt1 = shapes.addTextEffect(MsoPresetTextEffect.TEXT_EFFECT_10, "WordArt", "arial", 18, false, false, 3, 0, 3, 0, 200, 50);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| effect | int | [MsoPresetTextEffect](../../com.aspose.cells/msopresettexteffect). Il tipo di effetto di testo predefinito mso. |
| testo | java.lang.String | Il testo WordArt. |
| fontName | java.lang.String | Il nome del carattere. |
| size | int | La dimensione del carattere |
| fontBold | boolean | Indica se il carattere è in grassetto. |
| fontItalic | boolean | Indica se il carattere è in corsivo. |
| topRow | int | Indice della riga in alto a sinistra. |
| superiore | int | Rappresenta lo spostamento verticale della forma dalla sua riga sinistra, in unità di pixel. |
| leftColumn | int | Indice della colonna in alto a sinistra. |
| sinistra | int | Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra, in unità di pixel. |
| altezza | int | Rappresenta l'altezza della forma, in unità di pixel. |
| larghezza | int | Rappresenta la larghezza della forma, in unità di pixel. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - Returns a Shape object that represents the new WordArt object.
### addTextEffectInChart(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int top, int left, int height, int width) {#addTextEffectInChart-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-}
```
public Shape addTextEffectInChart(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int top, int left, int height, int width)
```


Inserisce un oggetto WordArt nel grafico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| effect | int | [MsoPresetTextEffect](../../com.aspose.cells/msopresettexteffect). Il tipo di effetto di testo predefinito mso. |
| testo | java.lang.String | Il testo WordArt. |
| fontName | java.lang.String | Il nome del carattere. |
| size | int | La dimensione del carattere |
| fontBold | boolean | Indica se il carattere è in grassetto. |
| fontItalic | boolean | Indica se il carattere è in corsivo. |
| superiore | int | Rappresenta lo spostamento verticale della forma dall'angolo in alto a sinistra in unità di 1/4000 dell'area del grafico. |
| sinistra | int | Rappresenta lo spostamento verticale della forma dall'angolo in alto a sinistra in unità di 1/4000 dell'area del grafico. |
| altezza | int | Rappresenta l'altezza della forma, in unità di 1/4000 dell'area del grafico. |
| larghezza | int | Rappresenta la larghezza della forma, in unità di 1/4000 dell'area del grafico. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - Returns a Shape object that represents the new WordArt object.
### addWordArt(int style, String text, int topRow, int top, int leftColumn, int left, int height, int width) {#addWordArt-int-java.lang.String-int-int-int-int-int-int-}
```
public Shape addWordArt(int style, String text, int topRow, int top, int leftColumn, int left, int height, int width)
```


Aggiunge WordArt predefinito da Excel 2007.

**Example**

```
         //add a WordArt
         Shape wordArt2 = shapes.addWordArt(PresetWordArtStyle.WORD_ART_STYLE_1, "WordArt", 3, 0, 3, 0, 50, 200);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). Lo stile WordArt predefinito. |
| testo | java.lang.String | Il testo. |
| topRow | int | Indice della riga in alto a sinistra. |
| superiore | int | Rappresenta lo spostamento verticale della forma dalla sua riga sinistra, in unità di pixel. |
| leftColumn | int | Indice della colonna in alto a sinistra. |
| sinistra | int | Rappresenta lo spostamento orizzontale della forma dalla sua colonna sinistra, in unità di pixel. |
| altezza | int | Rappresenta l'altezza della forma, in unità di pixel. |
| larghezza | int | Rappresenta la larghezza della forma, in unità di pixel. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### clear() {#clear--}
```
public void clear()
```


Cancella tutte le forme nel foglio di lavoro.

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


Restituisce se l'istanza contiene questo oggetto

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | java.lang.Object | oggetto di test |

**Returns:**
boolean - Se l'istanza contiene questo oggetto
### copyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn) {#copyCommentsInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-}
```
public void copyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn)
```


Copia tutti i commenti nell'intervallo.

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| shapes | [ShapeCollection](../../com.aspose.cells/shapecollection) | Le forme di origine. |
| ca | [CellArea](../../com.aspose.cells/cellarea) | L'intervallo di origine. |
| destRow | int | La riga di inizio dell'intervallo di destinazione. |
| destColumn | int | La colonna di inizio dell'intervallo di destinazione. |

### copyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, boolean isContained) {#copyInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-boolean-}
```
public void copyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, boolean isContained)
```


Copia le forme nell'intervallo nell'intervallo di destinazione.

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceShapes | [ShapeCollection](../../com.aspose.cells/shapecollection) | Forme di origine. |
| ca | [CellArea](../../com.aspose.cells/cellarea) | L'intervallo di origine. |
| destRow | int | L'indice di riga di destinazione dell'intervallo di destinazione. |
| destColumn | int | La colonna di destinazione dell'intervallo di destinazione. |
| isContained | boolean | Indica se copiare solo le forme contenute nell'intervallo. Se true, copia solo le forme nell'intervallo. Altrimenti, funziona come MS Office. |

### deleteInRange(CellArea ca) {#deleteInRange-com.aspose.cells.CellArea-}
```
public void deleteInRange(CellArea ca)
```


Elimina le forme nell'intervallo. Le forme dei commenti non saranno eliminate.

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | L'intervallo. Se le forme sono contenute nell'intervallo, verranno rimosse. |

### deleteShape(Shape shape) {#deleteShape-com.aspose.cells.Shape-}
```
public void deleteShape(Shape shape)
```


Elimina una forma. Se la forma è nel gruppo o è una forma di commento, non verrà eliminata.

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| shape | [Shape](../../com.aspose.cells/shape) |  |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### find(String what, int previous, FindOptions findOptions) {#find-java.lang.String-int-com.aspose.cells.FindOptions-}
```
public int find(String what, int previous, FindOptions findOptions)
```


Trova la forma per testo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cosa | java.lang.String | Il testo da cercare. |
| precedente | int | L'indice della forma precedente contiene lo stesso testo. -1 se la ricerca parte dall'inizio. |
| findOptions | [FindOptions](../../com.aspose.cells/findoptions) | Opzioni di ricerca |

**Returns:**
int - L'indice della forma trovata, -1 se non viene trovata alcuna forma.
### get(int index) {#get-int-}
```
public Shape get(int index)
```


Ottiene l'oggetto [Shape](../../com.aspose.cells/shape) all'indice specifico nella lista.

**Example**

```
         //get the first shape
         Shape shape = shapes.get(0);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### get(String name) {#get-java.lang.String-}
```
public Shape get(String name)
```


Ottiene l'oggetto [Shape](../../com.aspose.cells/shape) per nome della forma.

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Il nome della forma. |

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


Ottiene il numero di elementi contenuti nell'istanza di CollectionBase.

**Returns:**
int - Il numero di elementi contenuti nell'istanza di CollectionBase.
### group(Shape[] groupItems) {#group-com.aspose.cells.Shape---}
```
public GroupShape group(Shape[] groupItems)
```


Raggruppa le forme.

**Remarks**

La forma in groupItems non dovrebbe essere raggruppata. La forma deve trovarsi in questa collezione Shapes.

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| groupItems | [Shape\[\]](../../com.aspose.cells/shape) | gli elementi del gruppo. |

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


Determina l'indice di un elemento specifico nell'istanza di CollectionBase.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | java.lang.Object | Determina l'indice di un elemento specifico nell'istanza di CollectionBase. |

**Returns:**
int - L'indice del valore se trovato nella lista; altrimenti, -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Restituisce un enumeratore che itera attraverso l'istanza di CollectionBase.

**Returns:**
java.util.Iterator - Un iteratore per l'istanza di CollectionBase.
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


Rimuovi la forma.

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| shape | [Shape](../../com.aspose.cells/shape) |  |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Rimuovi la forma.

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice della forma. |

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


Separa gli elementi della forma.

**Remarks**

Se la forma di gruppo è raggruppata da un'altra forma di gruppo, non verrà eseguita alcuna operazione.

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| group | [GroupShape](../../com.aspose.cells/groupshape) | La forma di gruppo. |

### updateSelectedValue() {#updateSelectedValue--}
```
public void updateSelectedValue()
```


Aggiorna il valore selezionato con il valore della cella collegata o dell'intervallo della forma.

### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

