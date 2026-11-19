---
title: "ShapeCollection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente toutes les formes dans une feuille de calcul/graphique."
type: docs
url: /fr/java/com.aspose.cells/shapecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ShapeCollection extends CollectionBase
```

Représente toutes les formes dans une feuille de calcul/graphique.

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
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Ajoute un élément à l'instance CollectionBase. |
| [addActiveXControl(int type, int topRow, int top, int leftColumn, int left, int width, int height)](#addActiveXControl-int-int-int-int-int-int-int-) | Crée un contrôle Activex. |
| [addArc(int topRow, int top, int leftColumn, int left, int height, int width)](#addArc-int-int-int-int-int-int-) | Ajoute un ArcShape à la feuille de calcul. |
| [addAutoShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)](#addAutoShape-int-int-int-int-int-int-int-) | Ajoute un AutoShape à la feuille de calcul. |
| [addAutoShapeInChart(int type, int top, int left, int height, int width)](#addAutoShapeInChart-int-int-int-int-int-) | Ajoute un AutoShape au graphique. |
| [addButton(int topRow, int top, int leftColumn, int left, int height, int width)](#addButton-int-int-int-int-int-int-) | Ajoute un bouton à la feuille de calcul. |
| [addCheckBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addCheckBox-int-int-int-int-int-int-) | Ajoute une case à cocher à la feuille de calcul. |
| [addComboBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addComboBox-int-int-int-int-int-int-) | Ajoute une ComboBox à la feuille de calcul. |
| [addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left)](#addCopy-com.aspose.cells.Shape-int-int-int-int-) | Ajoute et copie une forme à la feuille de calcul. |
| [addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left, CopyOptions copyOptions)](#addCopy-com.aspose.cells.Shape-int-int-int-int-com.aspose.cells.CopyOptions-) | Ajoute et copie une forme à la feuille de calcul. |
| [addEquation(int topRow, int top, int leftColumn, int left, int height, int width)](#addEquation-int-int-int-int-int-int-) | Ajoute un objet d'équation à la feuille de calcul. |
| [addFreeFloatingShape(int type, int top, int left, int height, int width, byte[] imageData, boolean isOriginalSize)](#addFreeFloatingShape-int-int-int-int-int-byte---boolean-) | Ajoute une forme flottante libre à la feuille de calcul. S'applique uniquement aux formes ligne/image. |
| [addFreeform(int topRow, int top, int leftColumn, int left, int height, int width, ShapePath[] paths)](#addFreeform-int-int-int-int-int-int-com.aspose.cells.ShapePath---) | Ajoute une forme libre à la feuille de calcul. |
| [addGroupBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addGroupBox-int-int-int-int-int-int-) | Ajoute une GroupBox à la feuille de calcul. |
| [addIcons(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageByteData, byte[] compatibleImageData)](#addIcons-int-int-int-int-int-int-byte---byte---) | Ajoute une image svg. |
| [addLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, int width, String latex)](#addLaTeXEquation-int-int-int-int-int-int-java.lang.String-) | Ajoute un objet d'équation à la feuille de calcul en utilisant des chaînes au format LaTeX. |
| [addLabel(int topRow, int top, int leftColumn, int left, int height, int width)](#addLabel-int-int-int-int-int-int-) | Ajoute une étiquette à la feuille de calcul. |
| [addLabelInChart(int top, int left, int height, int width)](#addLabelInChart-int-int-int-int-) | Ajoute une étiquette au graphique. |
| [addLine(int topRow, int top, int leftColumn, int left, int height, int width)](#addLine-int-int-int-int-int-int-) | Ajoute un LineShape à la feuille de calcul. |
| [addLinkedPicture(int topRow, int leftColumn, int height, int width, String sourceFullName)](#addLinkedPicture-int-int-int-int-java.lang.String-) | Ajoute une image liée. |
| [addListBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addListBox-int-int-int-int-int-int-) | Ajoute une ListBox à la feuille de calcul. |
| [addOleObject(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageData)](#addOleObject-int-int-int-int-int-int-byte---) | Ajoute un OleObject. |
| [addOleObjectWithLinkedImage(int topRow, int leftColumn, int height, int width, String sourceFullName)](#addOleObjectWithLinkedImage-int-int-int-int-java.lang.String-) | Ajoute une image liée. |
| [addOval(int topRow, int top, int leftColumn, int left, int height, int width)](#addOval-int-int-int-int-int-int-) | Ajoute un Oval à la feuille de calcul. |
| [addPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream)](#addPicture-int-int-int-int-java.io.InputStream-) | Ajoute une image à la collection. |
| [addPicture(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale)](#addPicture-int-int-java.io.InputStream-int-int-) | Ajoute une image à la collection. |
| [addPictureInChart(int top, int left, InputStream stream, int widthScale, int heightScale)](#addPictureInChart-int-int-java.io.InputStream-int-int-) | Ajoute une image au graphique. |
| [addRadioButton(int topRow, int top, int leftColumn, int left, int height, int width)](#addRadioButton-int-int-int-int-int-int-) | Ajoute un RadioButton à la feuille de calcul. |
| [addRectangle(int topRow, int top, int leftColumn, int left, int height, int width)](#addRectangle-int-int-int-int-int-int-) | Ajoute un RectangleShape à la feuille de calcul. |
| [addScrollBar(int topRow, int top, int leftColumn, int left, int height, int width)](#addScrollBar-int-int-int-int-int-int-) | Ajoute une ScrollBar à la feuille de calcul. |
| [addShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)](#addShape-int-int-int-int-int-int-int-) | Ajoute une Shape à la feuille de calcul. |
| [addShapeInChart(int type, int placement, int left, int top, int right, int bottom)](#addShapeInChart-int-int-int-int-int-int-) | Ajoute une forme au graphique. Toutes les unités sont de 1/4000 de la zone du graphique. |
| [addShapeInChart(int type, int placement, int left, int top, int right, int bottom, byte[] imageData)](#addShapeInChart-int-int-int-int-int-int-byte---) | Ajoute une forme au graphique. Toutes les unités sont de 1/4000 de la zone du graphique. |
| [addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom)](#addShapeInChartByScale-int-int-double-double-double-double-) | Ajoute une forme au graphique. |
| [addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom, byte[] imageData)](#addShapeInChartByScale-int-int-double-double-double-double-byte---) | Ajoute une forme au graphique. Toutes les unités sont de 1/4000 de la zone du graphique. |
| [addSignatureLine(int topRow, int leftColumn, SignatureLine signatureLine)](#addSignatureLine-int-int-com.aspose.cells.SignatureLine-) | Ajoute une ligne de signature à la feuille de calcul. |
| [addSpinner(int topRow, int top, int leftColumn, int left, int height, int width)](#addSpinner-int-int-int-int-int-int-) | Ajoute un Spinner à la feuille de calcul. |
| [addSvg(int topRow, int top, int leftColumn, int left, int height, int width, byte[] svgData, byte[] compatibleImageData)](#addSvg-int-int-int-int-int-int-byte---byte---) | Ajoute une image svg. |
| [addTextBox(int topRow, int top, int leftColumn, int left, int height, int width)](#addTextBox-int-int-int-int-int-int-) | Ajoute une zone de texte à la feuille de calcul. |
| [addTextBoxInChart(int top, int left, int height, int width)](#addTextBoxInChart-int-int-int-int-) | Ajoute une zone de texte au graphique. |
| [addTextEffect(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int topRow, int top, int leftColumn, int left, int height, int width)](#addTextEffect-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-int-int-) | Insère un objet WordArt. |
| [addTextEffectInChart(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int top, int left, int height, int width)](#addTextEffectInChart-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-) | Insère un objet WordArt au graphique |
| [addWordArt(int style, String text, int topRow, int top, int leftColumn, int left, int height, int width)](#addWordArt-int-java.lang.String-int-int-int-int-int-int-) | Ajoute le WordArt prédéfini depuis Excel 2007. |
| [clear()](#clear--) | Efface toutes les formes de la feuille de calcul. |
| [contains(Object o)](#contains-java.lang.Object-) | Renvoie si l'instance contient cet objet |
| [copyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn)](#copyCommentsInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-) | Copie tous les commentaires de la plage. |
| [copyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, boolean isContained)](#copyInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-boolean-) | Copie les formes de la plage vers la plage de destination. |
| [deleteInRange(CellArea ca)](#deleteInRange-com.aspose.cells.CellArea-) | Supprime les formes de la plage. Les formes de commentaire ne seront pas supprimées. |
| [deleteShape(Shape shape)](#deleteShape-com.aspose.cells.Shape-) | Supprime une forme. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [find(String what, int previous, FindOptions findOptions)](#find-java.lang.String-int-com.aspose.cells.FindOptions-) | Trouve la forme par texte |
| [get(int index)](#get-int-) | Obtient l'objet [Shape](../../com.aspose.cells/shape) à l'index spécifique dans la liste. |
| [get(String name)](#get-java.lang.String-) | Obtient l'objet [Shape](../../com.aspose.cells/shape) par le nom de la forme. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtient le nombre d'éléments contenus dans l'instance CollectionBase. |
| [group(Shape[] groupItems)](#group-com.aspose.cells.Shape---) | Regroupe les formes. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Détermine l'index d'un élément spécifique dans l'instance CollectionBase. |
| [iterator()](#iterator--) | Renvoie un énumérateur qui parcourt l'instance CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Shape shape)](#remove-com.aspose.cells.Shape-) | Supprime la forme. |
| [removeAt(int index)](#removeAt-int-) | Supprime la forme. |
| [toString()](#toString--) |  |
| [ungroup(GroupShape group)](#ungroup-com.aspose.cells.GroupShape-) | Dégroupe les éléments de forme. |
| [updateSelectedValue()](#updateSelectedValue--) | Met à jour la valeur sélectionnée avec la valeur de la cellule liée ou de la plage de la forme. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Ajoute un élément à l'instance CollectionBase.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | L'objet à ajouter à l'instance CollectionBase. |

**Returns:**
int - La position dans laquelle le nouvel élément a été inséré.
### addActiveXControl(int type, int topRow, int top, int leftColumn, int left, int width, int height) {#addActiveXControl-int-int-int-int-int-int-int-}
```
public Shape addActiveXControl(int type, int topRow, int top, int leftColumn, int left, int width, int height)
```


Crée un contrôle Activex.

**Example**

```
         //add an ActiveX control
         Shape activeXControl = shapes.addActiveXControl(com.aspose.cells.ControlType.CHECK_BOX, 1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [ControlType](../../com.aspose.cells/controltype). Le type du contrôle. |
| topRow | int | Indice de ligne en haut à gauche. |
| haut | int | Représente le décalage vertical de Shape par rapport à sa ligne de gauche, en unité de pixel. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| gauche | int | Représente le décalage horizontal de Shape par rapport à sa colonne de gauche, en unité de pixel. |
| largeur | int | Représente la largeur de Shape, en unité de pixel. |
| hauteur | int | Représente la hauteur de Shape, en unité de pixel. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### addArc(int topRow, int top, int leftColumn, int left, int height, int width) {#addArc-int-int-int-int-int-int-}
```
public ArcShape addArc(int topRow, int top, int leftColumn, int left, int height, int width)
```


Ajoute un ArcShape à la feuille de calcul.

**Example**

```
         //add a arc
         ArcShape arcShape = shapes.addArc(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | int | Indice de ligne en haut à gauche. |
| haut | int | Représente le décalage vertical d'ArcShape par rapport à sa ligne de gauche, en unité de pixel. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| gauche | int | Représente le décalage horizontal d'ArcShape par rapport à sa colonne de gauche, en unité de pixel. |
| hauteur | int | Représente la hauteur d'ArcShape, en unité de pixel. |
| largeur | int | Représente la largeur d'ArcShape, en unité de pixel. |

**Returns:**
[ArcShape](../../com.aspose.cells/arcshape) - A ArcShape object.
### addAutoShape(int type, int topRow, int top, int leftColumn, int left, int height, int width) {#addAutoShape-int-int-int-int-int-int-int-}
```
public Shape addAutoShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)
```


Ajoute un AutoShape à la feuille de calcul.

**Remarks**

Le type ne peut pas être Chart/Comment/Picture/OleObject/Polygon/DialogBox

**Example**

```
         //Adds a AutoShape to the worksheet.
         Shape autoShape = shapes.addAutoShape(AutoShapeType.CUBE, 1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [AutoShapeType](../../com.aspose.cells/autoshapetype). Type de forme automatique. |
| topRow | int | Indice de ligne en haut à gauche. |
| haut | int | Représente le décalage vertical de Shape par rapport à sa ligne de gauche, en unité de pixel. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| gauche | int | Représente le décalage horizontal de Shape par rapport à sa colonne de gauche, en unité de pixel. |
| hauteur | int | Représente la hauteur de Shape, en unité de pixel. |
| largeur | int | Représente la largeur de Shape, en unité de pixel. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - A Shape object.
### addAutoShapeInChart(int type, int top, int left, int height, int width) {#addAutoShapeInChart-int-int-int-int-int-}
```
public Shape addAutoShapeInChart(int type, int top, int left, int height, int width)
```


Ajoute un AutoShape au graphique.

**Remarks**

Le type ne peut pas être Chart/Comment/Picture/OleObject/Polygon/DialogBox

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [AutoShapeType](../../com.aspose.cells/autoshapetype). Type de forme automatique. |
| haut | int | Représente le décalage vertical de textbox depuis le coin supérieur gauche en unités de 1/4000 de la zone du graphique. |
| gauche | int | Représente le décalage vertical de textbox depuis le coin supérieur gauche en unités de 1/4000 de la zone du graphique. |
| hauteur | int | Représente la hauteur de textbox, en unités de 1/4000 de la zone du graphique. |
| largeur | int | Représente la largeur de textbox, en unités de 1/4000 de la zone du graphique. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - Returns a shape object.
### addButton(int topRow, int top, int leftColumn, int left, int height, int width) {#addButton-int-int-int-int-int-int-}
```
public Button addButton(int topRow, int top, int leftColumn, int left, int height, int width)
```


Ajoute un bouton à la feuille de calcul.

**Example**

```
         //add a button
         Button button = shapes.addButton(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | int | Indice de ligne en haut à gauche. |
| haut | int | Représente le décalage vertical de Button par rapport à sa ligne de gauche, en unité de pixel. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| gauche | int | Représente le décalage horizontal de Button par rapport à sa colonne de gauche, en unité de pixel. |
| hauteur | int | Représente la hauteur de Button, en unité de pixel. |
| largeur | int | Représente la largeur de Button, en unité de pixel. |

**Returns:**
[Button](../../com.aspose.cells/button) - A Button object.
### addCheckBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addCheckBox-int-int-int-int-int-int-}
```
public CheckBox addCheckBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Ajoute une case à cocher à la feuille de calcul.

**Example**

```
         //add a CheckBox
         CheckBox checkBox = shapes.addCheckBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | int | Indice de ligne en haut à gauche. |
| haut | int | Représente le décalage vertical de checkbox par rapport à sa ligne supérieure, en unité de pixel. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| gauche | int | Représente le décalage horizontal de textbox par rapport à sa colonne de gauche, en unité de pixel. |
| hauteur | int | Hauteur de textbox, en unité de pixel. |
| largeur | int | Largeur de textbox, en unité de pixel. |

**Returns:**
[CheckBox](../../com.aspose.cells/checkbox) - The new CheckBox object index.
### addComboBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addComboBox-int-int-int-int-int-int-}
```
public ComboBox addComboBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Ajoute une ComboBox à la feuille de calcul.

**Example**

```
         //add a combo box
         ComboBox comboBox = shapes.addComboBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | int | Indice de ligne en haut à gauche. |
| haut | int | Représente le décalage vertical de ComboBox par rapport à sa ligne de gauche, en unité de pixel. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| gauche | int | Représente le décalage horizontal de ComboBox par rapport à sa colonne de gauche, en unité de pixel. |
| hauteur | int | Représente la hauteur du ComboBox, en unité de pixel. |
| largeur | int | Représente la largeur du ComboBox, en unité de pixel. |

**Returns:**
[ComboBox](../../com.aspose.cells/combobox) - A ComboBox object.
### addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left) {#addCopy-com.aspose.cells.Shape-int-int-int-int-}
```
public Shape addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left)
```


Ajoute et copie une forme à la feuille de calcul.

**Example**

```
         //add a shape
         RectangleShape rectangle = shapes.addRectangle(2, 0, 2, 0, 130, 130);
         //Adds and copies a shape.
         shapes.addCopy(rectangle, 7, 0, 7, 0);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceShape | [Shape](../../com.aspose.cells/shape) | Forme source. |
| topRow | int | L'index de la ligne supérieure. |
| haut | int | Représente le décalage vertical depuis sa ligne supérieure, en unité de pixel. |
| leftColumn | int | L'index de la colonne de gauche. |
| gauche | int | Représente le décalage horizontal depuis sa colonne de gauche, en unité de pixel. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - The new [Shape](../../com.aspose.cells/shape) object.
### addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left, CopyOptions copyOptions) {#addCopy-com.aspose.cells.Shape-int-int-int-int-com.aspose.cells.CopyOptions-}
```
public Shape addCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left, CopyOptions copyOptions)
```


Ajoute et copie une forme à la feuille de calcul.

**Example**

```
         //add a shape
         RectangleShape rectangle = shapes.addRectangle(2, 0, 2, 0, 130, 130);
         //Adds and copies a shape.
         shapes.addCopy(rectangle, 7, 0, 7, 0);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceShape | [Shape](../../com.aspose.cells/shape) | Forme source. |
| topRow | int | L'index de la ligne supérieure. |
| haut | int | Représente le décalage vertical depuis sa ligne supérieure, en unité de pixel. |
| leftColumn | int | L'index de la colonne de gauche. |
| gauche | int | Représente le décalage horizontal depuis sa colonne de gauche, en unité de pixel. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | Les options de copie des formes. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - The new [Shape](../../com.aspose.cells/shape) object.
### addEquation(int topRow, int top, int leftColumn, int left, int height, int width) {#addEquation-int-int-int-int-int-int-}
```
public TextBox addEquation(int topRow, int top, int leftColumn, int left, int height, int width)
```


Ajoute un objet d'équation à la feuille de calcul.

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
| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | int | L'index de la ligne supérieure. |
| haut | int | Le décalage vertical de sa ligne supérieure, en unité de pixel. |
| leftColumn | int | L'index de la colonne de gauche. |
| gauche | int | Le décalage horizontal depuis sa colonne de gauche, en unité de pixel. |
| hauteur | int | La hauteur de l'équation, en unité de pixel. |
| largeur | int | La largeur de l'équation, en unité de pixel. |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - 
### addFreeFloatingShape(int type, int top, int left, int height, int width, byte[] imageData, boolean isOriginalSize) {#addFreeFloatingShape-int-int-int-int-int-byte---boolean-}
```
public Shape addFreeFloatingShape(int type, int top, int left, int height, int width, byte[] imageData, boolean isOriginalSize)
```


Ajoute une forme flottante libre à la feuille de calcul. S'applique uniquement aux formes ligne/image.

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
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Le type de forme. |
| haut | int | Représente le décalage vertical de la forme depuis la ligne supérieure de la feuille de calcul, en unité de pixel. |
| gauche | int | Représente le décalage horizontal de la forme depuis la colonne de gauche de la feuille de calcul, en unité de pixel. |
| hauteur | int | Représente la hauteur de LineShape, en unité de pixel. |
| largeur | int | Représente la largeur de LineShape, en unité de pixel. |
| imageData | byte[] | Les données d'image, ne s'appliquent qu'à l'image. |
| isOriginalSize | boolean | Indique si la forme utilise la taille originale lorsque la forme est une image. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### addFreeform(int topRow, int top, int leftColumn, int left, int height, int width, ShapePath[] paths) {#addFreeform-int-int-int-int-int-int-com.aspose.cells.ShapePath---}
```
public Shape addFreeform(int topRow, int top, int leftColumn, int left, int height, int width, ShapePath[] paths)
```


Ajoute une forme libre à la feuille de calcul.

**Remarks**

Remarque : la largeur et la hauteur dans les paramètres peuvent être n'importe quelles valeurs entières positives, et non la largeur et la hauteur totales du tableau ShapePath spécifié par \\u9225\\u6a96aths'. La relation entre elles est une relation d'échelle-remplissage, c'est-à-dire que chaque objet ShapePath sera mis à l'échelle en fonction de la largeur et de la hauteur. Ainsi, lorsqu'il y a plusieurs objets dans les 'paths', chaque objet ShapePath doit être conçu de manière raisonnable pour répondre aux attentes. Lorsqu'il n'y a qu'un seul objet ShapePath et qu'il n'existe aucune autre exigence, passer la largeur et la hauteur de l'objet comme valeurs de paramètres \\u9225\\u5b27\\u20ac\\u5a94s constitue une bonne solution.

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
| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | int | Indice de ligne en haut à gauche. |
| haut | int | Représente le décalage vertical de la forme libre depuis sa ligne gauche, en unité de pixel. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| gauche | int | Représente le décalage horizontal de la forme libre depuis sa colonne de gauche, en unité de pixel. |
| hauteur | int | Représente la hauteur de la forme libre, en unité de pixel. |
| largeur | int | Représente la largeur de la forme libre, en unité de pixel. |
| paths | [ShapePath\[\]](../../com.aspose.cells/shapepath) | Représente un chemin défini par l'utilisateur |

**Returns:**
[Shape](../../com.aspose.cells/shape) - A freeform shape.
### addGroupBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addGroupBox-int-int-int-int-int-int-}
```
public GroupBox addGroupBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Ajoute une GroupBox à la feuille de calcul.

**Example**

```
         //add a group box
         GroupBox groupBox = shapes.addGroupBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | int | Indice de ligne en haut à gauche. |
| haut | int | Représente le décalage vertical du GroupBox par rapport à sa ligne de gauche, en unité de pixel. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| gauche | int | Représente le décalage horizontal du GroupBox par rapport à sa colonne de gauche, en unité de pixel. |
| hauteur | int | Représente la hauteur du GroupBox, en unité de pixel. |
| largeur | int | Représente la largeur du GroupBox, en unité de pixel. |

**Returns:**
[GroupBox](../../com.aspose.cells/groupbox) - A GroupBox object.
### addIcons(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageByteData, byte[] compatibleImageData) {#addIcons-int-int-int-int-int-int-byte---byte---}
```
public Picture addIcons(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageByteData, byte[] compatibleImageData)
```


Ajoute une image svg.

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
| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | int | Indice de ligne en haut à gauche. |
| haut | int | Représente le décalage vertical de shape depuis sa ligne de gauche, en unité de pixel. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| gauche | int | Le décalage horizontal de shape depuis sa colonne de gauche, en unité de pixel. |
| hauteur | int | La hauteur de shape, en unité de pixel. |
| largeur | int | La largeur de shape, en unité de pixel. |
| imageByteData | byte[] | Les données d'octets de l'image. |
| compatibleImageData | byte[] | Données d'image converties depuis le SVG afin d'être compatibles avec Excel 2016 ou les versions antérieures. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - 
### addLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, int width, String latex) {#addLaTeXEquation-int-int-int-int-int-int-java.lang.String-}
```
public TextBox addLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, int width, String latex)
```


Ajoute un objet d'équation à la feuille de calcul en utilisant des chaînes au format LaTeX.

**Example**

```
         // LaTeX format string.
         String latex = "\\alpha +  \\frac{\\partial^2}{\\partial x_1\\partial x_2}y - \\left ( a + b \\right )+_{a}^{b}\\beta";
         // Adds an equation object to the worksheet.
         TextBox textBox = shapes.addLaTeXEquation(1, 0, 1, 0, 100, 300, latex);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | int | L'index de la ligne supérieure. |
| haut | int | Le décalage vertical de sa ligne supérieure, en unité de pixel. |
| leftColumn | int | L'index de la colonne de gauche. |
| gauche | int | Le décalage horizontal depuis sa colonne de gauche, en unité de pixel. |
| hauteur | int | La hauteur de l'équation, en unité de pixel. |
| largeur | int | La largeur de l'équation, en unité de pixel. |
| latex | java.lang.String | Chaîne de format LaTeX |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - 
### addLabel(int topRow, int top, int leftColumn, int left, int height, int width) {#addLabel-int-int-int-int-int-int-}
```
public Label addLabel(int topRow, int top, int leftColumn, int left, int height, int width)
```


Ajoute une étiquette à la feuille de calcul.

**Example**

```
         //add a label
         Label label = shapes.addLabel(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | int | Indice de ligne en haut à gauche. |
| haut | int | Représente le décalage vertical du Label par rapport à sa ligne de gauche, en unité de pixel. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| gauche | int | Représente le décalage horizontal du Label par rapport à sa colonne de gauche, en unité de pixel. |
| hauteur | int | Représente la hauteur du Label, en unité de pixel. |
| largeur | int | Représente la largeur du Label, en unité de pixel. |

**Returns:**
[Label](../../com.aspose.cells/label) - A Label object.
### addLabelInChart(int top, int left, int height, int width) {#addLabelInChart-int-int-int-int-}
```
public Label addLabelInChart(int top, int left, int height, int width)
```


Ajoute une étiquette au graphique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| haut | int | Représente le décalage vertical du label depuis le coin supérieur gauche, en unités de 1/4000 de la zone du graphique. |
| gauche | int | Représente le décalage vertical du label depuis le coin supérieur gauche, en unités de 1/4000 de la zone du graphique. |
| hauteur | int | Représente la hauteur du label, en unités de 1/4000 de la zone du graphique. |
| largeur | int | Représente la largeur du label, en unités de 1/4000 de la zone du graphique. |

**Returns:**
[Label](../../com.aspose.cells/label) - A new Label object.
### addLine(int topRow, int top, int leftColumn, int left, int height, int width) {#addLine-int-int-int-int-int-int-}
```
public LineShape addLine(int topRow, int top, int leftColumn, int left, int height, int width)
```


Ajoute un LineShape à la feuille de calcul.

**Example**

```
         // add a line object
         LineShape lineShape = shapes.addLine(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | int | Indice de ligne en haut à gauche. |
| haut | int | Représente le décalage vertical du LineShape depuis sa ligne de gauche, en unité de pixel. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| gauche | int | Représente le décalage horizontal du LineShape depuis sa colonne de gauche, en unité de pixel. |
| hauteur | int | Représente la hauteur de LineShape, en unité de pixel. |
| largeur | int | Représente la largeur de LineShape, en unité de pixel. |

**Returns:**
[LineShape](../../com.aspose.cells/lineshape) - A LineShape object.
### addLinkedPicture(int topRow, int leftColumn, int height, int width, String sourceFullName) {#addLinkedPicture-int-int-int-int-java.lang.String-}
```
public Picture addLinkedPicture(int topRow, int leftColumn, int height, int width, String sourceFullName)
```


Ajoute une image liée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | int | Indice de ligne en haut à gauche. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| hauteur | int | La hauteur de la forme. En unité de pixels. |
| largeur | int | La largeur de la forme. En unité de pixels |
| sourceFullName | java.lang.String | Le chemin et le nom du fichier source pour l'image liée |

**Returns:**
[Picture](../../com.aspose.cells/picture) - [Picture](../../com.aspose.cells/picture) Picture object.
### addListBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addListBox-int-int-int-int-int-int-}
```
public ListBox addListBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Ajoute une ListBox à la feuille de calcul.

**Example**

```
         //add a list box
         ListBox listBox = shapes.addListBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | int | Indice de ligne en haut à gauche. |
| haut | int | Représente le décalage vertical de ListBox par rapport à sa rangée de gauche, en unité de pixel. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| gauche | int | Représente le décalage horizontal de ListBox par rapport à sa colonne de gauche, en unité de pixel. |
| hauteur | int | Représente la hauteur de ListBox, en unité de pixel. |
| largeur | int | Représente la largeur de ListBox, en unité de pixel. |

**Returns:**
[ListBox](../../com.aspose.cells/listbox) - A ListBox object.
### addOleObject(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageData) {#addOleObject-int-int-int-int-int-int-byte---}
```
public OleObject addOleObject(int topRow, int top, int leftColumn, int left, int height, int width, byte[] imageData)
```


Ajoute un OleObject.

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
| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | int |  |
| haut | int |  |
| leftColumn | int |  |
| gauche | int |  |
| hauteur | int |  |
| largeur | int |  |
| imageData | byte[] |  |

**Returns:**
[OleObject](../../com.aspose.cells/oleobject) - 
### addOleObjectWithLinkedImage(int topRow, int leftColumn, int height, int width, String sourceFullName) {#addOleObjectWithLinkedImage-int-int-int-int-java.lang.String-}
```
public OleObject addOleObjectWithLinkedImage(int topRow, int leftColumn, int height, int width, String sourceFullName)
```


Ajoute une image liée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | int | Indice de ligne en haut à gauche. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| hauteur | int | La hauteur de la forme. En unité de pixels. |
| largeur | int | La largeur de la forme. En unité de pixels |
| sourceFullName | java.lang.String | Le chemin et le nom du fichier source pour l'image liée |

**Returns:**
[OleObject](../../com.aspose.cells/oleobject) - [Picture](../../com.aspose.cells/picture) Picture object.
### addOval(int topRow, int top, int leftColumn, int left, int height, int width) {#addOval-int-int-int-int-int-int-}
```
public Oval addOval(int topRow, int top, int leftColumn, int left, int height, int width)
```


Ajoute un Oval à la feuille de calcul.

**Example**

```
         //add a oval
         Oval oval = shapes.addOval(1, 0, 1, 0, 50, 50);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | int | Indice de ligne en haut à gauche. |
| haut | int | Représente le décalage vertical d'Oval par rapport à sa rangée de gauche, en unité de pixel. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| gauche | int | Représente le décalage horizontal d'Oval par rapport à sa colonne de gauche, en unité de pixel. |
| hauteur | int | Représente la hauteur d'Oval, en unité de pixel. |
| largeur | int | Représente la largeur d'Oval, en unité de pixel. |

**Returns:**
[Oval](../../com.aspose.cells/oval) - A Oval object.
### addPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream) {#addPicture-int-int-int-int-java.io.InputStream-}
```
public Picture addPicture(int topRow, int leftColumn, int bottomRow, int rightColumn, InputStream stream)
```


Ajoute une image à la collection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | int | Indice de ligne en haut à gauche. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| bottomRow | int | Indice de ligne en bas à droite |
| rightColumn | int | Indice de colonne en bas à droite |
| stream | java.io.InputStream | Objet de flux contenant les données de l'image. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - [Picture](../../com.aspose.cells/picture) Picture object.
### addPicture(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale) {#addPicture-int-int-java.io.InputStream-int-int-}
```
public Picture addPicture(int topRow, int leftColumn, InputStream stream, int widthScale, int heightScale)
```


Ajoute une image à la collection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | int | Indice de ligne en haut à gauche. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| stream | java.io.InputStream | Objet de flux contenant les données de l'image. |
| widthScale | int | Échelle de la largeur de l'image, en pourcentage. |
| heightScale | int | Échelle de la hauteur de l'image, en pourcentage. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - [Picture](../../com.aspose.cells/picture) Picture object.
### addPictureInChart(int top, int left, InputStream stream, int widthScale, int heightScale) {#addPictureInChart-int-int-java.io.InputStream-int-int-}
```
public Picture addPictureInChart(int top, int left, InputStream stream, int widthScale, int heightScale)
```


Ajoute une image au graphique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| haut | int | Représente le décalage vertical de la forme depuis le coin supérieur gauche en unités de 1/4000 de la zone du graphique. |
| gauche | int | Représente le décalage horizontal de la forme depuis le coin supérieur gauche en unités de 1/4000 de la zone du graphique. |
| stream | java.io.InputStream | Objet de flux contenant les données de l'image. |
| widthScale | int | Échelle de la largeur de l'image, en pourcentage. |
| heightScale | int | Échelle de la hauteur de l'image, en pourcentage. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - Returns a Picture object.
### addRadioButton(int topRow, int top, int leftColumn, int left, int height, int width) {#addRadioButton-int-int-int-int-int-int-}
```
public RadioButton addRadioButton(int topRow, int top, int leftColumn, int left, int height, int width)
```


Ajoute un RadioButton à la feuille de calcul.

**Example**

```
         //add a radio button
         RadioButton radioButton = shapes.addRadioButton(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | int | Indice de ligne en haut à gauche. |
| haut | int | Représente le décalage vertical de RadioButton par rapport à sa rangée de gauche, en unité de pixel. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| gauche | int | Représente le décalage horizontal de RadioButton par rapport à sa colonne de gauche, en unité de pixel. |
| hauteur | int | Représente la hauteur de RadioButton, en unité de pixel. |
| largeur | int | Représente la largeur de RadioButton, en unité de pixel. |

**Returns:**
[RadioButton](../../com.aspose.cells/radiobutton) - A RadioButton object.
### addRectangle(int topRow, int top, int leftColumn, int left, int height, int width) {#addRectangle-int-int-int-int-int-int-}
```
public RectangleShape addRectangle(int topRow, int top, int leftColumn, int left, int height, int width)
```


Ajoute un RectangleShape à la feuille de calcul.

**Example**

```
         // add a rectangle
         RectangleShape rectangleShape = shapes.addRectangle(2, 0, 2, 0, 130, 130);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | int | Indice de ligne en haut à gauche. |
| haut | int | Représente le décalage vertical de RectangleShape par rapport à sa rangée de gauche, en unité de pixel. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| gauche | int | Représente le décalage horizontal de RectangleShape par rapport à sa colonne de gauche, en unité de pixel. |
| hauteur | int | Représente la hauteur de RectangleShape, en unité de pixel. |
| largeur | int | Représente la largeur de RectangleShape, en unité de pixel. |

**Returns:**
[RectangleShape](../../com.aspose.cells/rectangleshape) - A RectangleShape object.
### addScrollBar(int topRow, int top, int leftColumn, int left, int height, int width) {#addScrollBar-int-int-int-int-int-int-}
```
public ScrollBar addScrollBar(int topRow, int top, int leftColumn, int left, int height, int width)
```


Ajoute une ScrollBar à la feuille de calcul.

**Example**

```
         //add a scroll bar
         ScrollBar scrollBar = shapes.addScrollBar(1, 0, 1, 0, 100, 20);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | int | Indice de ligne en haut à gauche. |
| haut | int | Représente le décalage vertical de ScrollBar par rapport à sa rangée de gauche, en unité de pixel. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| gauche | int | Représente le décalage horizontal de ScrollBar par rapport à sa colonne de gauche, en unité de pixel. |
| hauteur | int | Représente la hauteur de ScrollBar, en unité de pixel. |
| largeur | int | Représente la largeur de ScrollBar, en unité de pixel. |

**Returns:**
[ScrollBar](../../com.aspose.cells/scrollbar) - A ScrollBar object.
### addShape(int type, int topRow, int top, int leftColumn, int left, int height, int width) {#addShape-int-int-int-int-int-int-int-}
```
public Shape addShape(int type, int topRow, int top, int leftColumn, int left, int height, int width)
```


Ajoute une Shape à la feuille de calcul.

**Remarks**

Le type ne peut pas être Chart/Comment/Picture/OleObject/Polygon/DialogBox

**Example**

```
         //Add a shape of the specified type
         Shape shapeByType = shapes.addShape(MsoDrawingType.CELLS_DRAWING, 1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Type de dessin Mso. |
| topRow | int | Indice de ligne en haut à gauche. |
| haut | int | Représente le décalage vertical de Shape par rapport à sa ligne de gauche, en unité de pixel. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| gauche | int | Représente le décalage horizontal de Shape par rapport à sa colonne de gauche, en unité de pixel. |
| hauteur | int | Représente la hauteur de Shape, en unité de pixel. |
| largeur | int | Représente la largeur de Shape, en unité de pixel. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - A Shape object.
### addShapeInChart(int type, int placement, int left, int top, int right, int bottom) {#addShapeInChart-int-int-int-int-int-int-}
```
public Shape addShapeInChart(int type, int placement, int left, int top, int right, int bottom)
```


Ajoute une forme au graphique. Toutes les unités sont de 1/4000 de la zone du graphique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Le type de dessin. |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype). le type de placement. |
| gauche | int | En unité de 1/4000 de la largeur de la zone du graphique. |
| haut | int | En unité de 1/4000 de la hauteur de la zone du graphique. |
| droite | int | En unité de 1/4000 de la largeur de la zone du graphique. |
| bas | int | En unité de 1/4000 de la hauteur de la zone du graphique. |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addShapeInChart(int type, int placement, int left, int top, int right, int bottom, byte[] imageData) {#addShapeInChart-int-int-int-int-int-int-byte---}
```
public Shape addShapeInChart(int type, int placement, int left, int top, int right, int bottom, byte[] imageData)
```


Ajoute une forme au graphique. Toutes les unités sont de 1/4000 de la zone du graphique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Le type de dessin. |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype). le type de placement. |
| gauche | int | En unité de 1/4000 de la largeur de la zone du graphique. |
| haut | int | En unité de 1/4000 de la hauteur de la zone du graphique. |
| droite | int | En unité de 1/4000 de la largeur de la zone du graphique. |
| bas | int | En unité de 1/4000 de la hauteur de la zone du graphique. |
| imageData | byte[] | Si la forme n'est pas une image ou un objet ole, imageData doit être nul. |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom) {#addShapeInChartByScale-int-int-double-double-double-double-}
```
public Shape addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom)
```


Ajoutez une forme au graphique. Toutes les unités sont à l'échelle en pourcentage de la zone du graphique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Le type de dessin. |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype). le type de placement. |
| gauche | double | L'unité est à l'échelle en pourcentage de la largeur de la zone du graphique. |
| haut | double | L'unité est à l'échelle en pourcentage de la hauteur de la zone du graphique. |
| droite | double | L'unité est à l'échelle en pourcentage de la largeur de la zone du graphique. |
| bas | double | L'unité est à l'échelle en pourcentage de la hauteur de la zone du graphique. |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom, byte[] imageData) {#addShapeInChartByScale-int-int-double-double-double-double-byte---}
```
public Shape addShapeInChartByScale(int type, int placement, double left, double top, double right, double bottom, byte[] imageData)
```


Ajoute une forme au graphique. Toutes les unités sont de 1/4000 de la zone du graphique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [MsoDrawingType](../../com.aspose.cells/msodrawingtype). Le type de dessin. |
| placement | int | [PlacementType](../../com.aspose.cells/placementtype). le type de placement. |
| gauche | double | L'unité est à l'échelle en pourcentage de la largeur de la zone du graphique. |
| haut | double | L'unité est à l'échelle en pourcentage de la hauteur de la zone du graphique. |
| droite | double | L'unité est à l'échelle en pourcentage de la largeur de la zone du graphique. |
| bas | double | L'unité est à l'échelle en pourcentage de la hauteur de la zone du graphique. |
| imageData | byte[] | Si la forme n'est pas une image ou un objet ole, imageData doit être nul. |

**Returns:**
[Shape](../../com.aspose.cells/shape)
### addSignatureLine(int topRow, int leftColumn, SignatureLine signatureLine) {#addSignatureLine-int-int-com.aspose.cells.SignatureLine-}
```
public Picture addSignatureLine(int topRow, int leftColumn, SignatureLine signatureLine)
```


Ajoute une ligne de signature à la feuille de calcul.

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
| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | int | Indice de ligne en haut à gauche. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| signatureLine | [SignatureLine](../../com.aspose.cells/signatureline) | Représente un objet de ligne de signature. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - 
### addSpinner(int topRow, int top, int leftColumn, int left, int height, int width) {#addSpinner-int-int-int-int-int-int-}
```
public Spinner addSpinner(int topRow, int top, int leftColumn, int left, int height, int width)
```


Ajoute un Spinner à la feuille de calcul.

**Example**

```
         //add a spinner
         Spinner spinner = shapes.addSpinner(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | int | Indice de ligne en haut à gauche. |
| haut | int | Représente le décalage vertical de Spinner par rapport à sa rangée de gauche, en unité de pixel. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| gauche | int | Représente le décalage horizontal de Spinner par rapport à sa colonne de gauche, en unité de pixel. |
| hauteur | int | Représente la hauteur de Spinner, en unité de pixel. |
| largeur | int | Représente la largeur de Spinner, en unité de pixel. |

**Returns:**
[Spinner](../../com.aspose.cells/spinner) - A Spinner object.
### addSvg(int topRow, int top, int leftColumn, int left, int height, int width, byte[] svgData, byte[] compatibleImageData) {#addSvg-int-int-int-int-int-int-byte---byte---}
```
public Picture addSvg(int topRow, int top, int leftColumn, int left, int height, int width, byte[] svgData, byte[] compatibleImageData)
```


Ajoute une image svg.

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
| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | int | Indice de ligne en haut à gauche. |
| haut | int | Représente le décalage vertical de shape depuis sa ligne de gauche, en unité de pixel. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| gauche | int | Le décalage horizontal de shape depuis sa colonne de gauche, en unité de pixel. |
| hauteur | int | La hauteur de shape, en unité de pixel. |
| largeur | int | La largeur de shape, en unité de pixel. |
| svgData | byte[] | Les données d'image svg. |
| compatibleImageData | byte[] | Données d'image converties depuis le SVG afin d'être compatibles avec Excel 2016 ou les versions antérieures. |

**Returns:**
[Picture](../../com.aspose.cells/picture) - 
### addTextBox(int topRow, int top, int leftColumn, int left, int height, int width) {#addTextBox-int-int-int-int-int-int-}
```
public TextBox addTextBox(int topRow, int top, int leftColumn, int left, int height, int width)
```


Ajoute une zone de texte à la feuille de calcul.

**Example**

```
         //add a TextBox
         TextBox textBox = shapes.addTextBox(1, 0, 1, 0, 100, 50);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | int | Indice de ligne en haut à gauche. |
| haut | int | Représente le décalage vertical de textbox par rapport à sa rangée supérieure, en unité de pixel. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| gauche | int | Représente le décalage horizontal de textbox par rapport à sa colonne de gauche, en unité de pixel. |
| hauteur | int | Représente la hauteur de la zone de texte, en unité de pixel. |
| largeur | int | Représente la largeur de la zone de texte, en unité de pixel. |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - A [TextBox](../../com.aspose.cells/textbox) object.
### addTextBoxInChart(int top, int left, int height, int width) {#addTextBoxInChart-int-int-int-int-}
```
public TextBox addTextBoxInChart(int top, int left, int height, int width)
```


Ajoute une zone de texte au graphique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| haut | int | Représente le décalage vertical de textbox depuis le coin supérieur gauche en unités de 1/4000 de la zone du graphique. |
| gauche | int | Représente le décalage vertical de textbox depuis le coin supérieur gauche en unités de 1/4000 de la zone du graphique. |
| hauteur | int | Représente la hauteur de textbox, en unités de 1/4000 de la zone du graphique. |
| largeur | int | Représente la largeur de textbox, en unités de 1/4000 de la zone du graphique. |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - A TextBox object.
### addTextEffect(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int topRow, int top, int leftColumn, int left, int height, int width) {#addTextEffect-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-int-int-}
```
public Shape addTextEffect(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int topRow, int top, int leftColumn, int left, int height, int width)
```


Insère un objet WordArt.

**Example**

```
         //add a WordArt
         Shape wordArt1 = shapes.addTextEffect(MsoPresetTextEffect.TEXT_EFFECT_10, "WordArt", "arial", 18, false, false, 3, 0, 3, 0, 200, 50);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| effect | int | [MsoPresetTextEffect](../../com.aspose.cells/msopresettexteffect). Le type d'effet de texte prédéfini mso. |
| texte | java.lang.String | Le texte WordArt. |
| fontName | java.lang.String | Le nom de la police. |
| taille | int | La taille de la police |
| fontBold | boolean | Indique si la police est en gras. |
| fontItalic | boolean | Indique si la police est en italique. |
| topRow | int | Indice de ligne en haut à gauche. |
| haut | int | Représente le décalage vertical de shape depuis sa ligne de gauche, en unité de pixel. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| gauche | int | Représente le décalage horizontal de la forme par rapport à sa colonne de gauche, en unité de pixel. |
| hauteur | int | Représente la hauteur de la forme, en unité de pixel. |
| largeur | int | Représente la largeur de la forme, en unité de pixel. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - Returns a Shape object that represents the new WordArt object.
### addTextEffectInChart(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int top, int left, int height, int width) {#addTextEffectInChart-int-java.lang.String-java.lang.String-int-boolean-boolean-int-int-int-int-}
```
public Shape addTextEffectInChart(int effect, String text, String fontName, int size, boolean fontBold, boolean fontItalic, int top, int left, int height, int width)
```


Insère un objet WordArt au graphique

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| effect | int | [MsoPresetTextEffect](../../com.aspose.cells/msopresettexteffect). Le type d'effet de texte prédéfini mso. |
| texte | java.lang.String | Le texte WordArt. |
| fontName | java.lang.String | Le nom de la police. |
| taille | int | La taille de la police |
| fontBold | boolean | Indique si la police est en gras. |
| fontItalic | boolean | Indique si la police est en italique. |
| haut | int | Représente le décalage vertical de la forme depuis le coin supérieur gauche en unités de 1/4000 de la zone du graphique. |
| gauche | int | Représente le décalage vertical de la forme depuis le coin supérieur gauche en unités de 1/4000 de la zone du graphique. |
| hauteur | int | Représente la hauteur de la forme, en unités de 1/4000 de la zone du graphique. |
| largeur | int | Représente la largeur de la forme, en unités de 1/4000 de la zone du graphique. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - Returns a Shape object that represents the new WordArt object.
### addWordArt(int style, String text, int topRow, int top, int leftColumn, int left, int height, int width) {#addWordArt-int-java.lang.String-int-int-int-int-int-int-}
```
public Shape addWordArt(int style, String text, int topRow, int top, int leftColumn, int left, int height, int width)
```


Ajoute le WordArt prédéfini depuis Excel 2007.

**Example**

```
         //add a WordArt
         Shape wordArt2 = shapes.addWordArt(PresetWordArtStyle.WORD_ART_STYLE_1, "WordArt", 3, 0, 3, 0, 50, 200);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). Le style WordArt prédéfini. |
| texte | java.lang.String | Le texte. |
| topRow | int | Indice de ligne en haut à gauche. |
| haut | int | Représente le décalage vertical de shape depuis sa ligne de gauche, en unité de pixel. |
| leftColumn | int | Indice de colonne en haut à gauche. |
| gauche | int | Représente le décalage horizontal de la forme par rapport à sa colonne de gauche, en unité de pixel. |
| hauteur | int | Représente la hauteur de la forme, en unité de pixel. |
| largeur | int | Représente la largeur de la forme, en unité de pixel. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### clear() {#clear--}
```
public void clear()
```


Efface toutes les formes de la feuille de calcul.

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


Renvoie si l'instance contient cet objet

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | objet de test |

**Returns:**
boolean - Si l'instance contient cet objet
### copyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn) {#copyCommentsInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-}
```
public void copyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn)
```


Copie tous les commentaires de la plage.

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
| Paramètre | Type | Description |
| --- | --- | --- |
| shapes | [ShapeCollection](../../com.aspose.cells/shapecollection) | Les formes source. |
| ca | [CellArea](../../com.aspose.cells/cellarea) | La plage source. |
| destRow | int | La ligne de départ de la plage de destination. |
| destColumn | int | La colonne de départ de la plage de destination. |

### copyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, boolean isContained) {#copyInRange-com.aspose.cells.ShapeCollection-com.aspose.cells.CellArea-int-int-boolean-}
```
public void copyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, boolean isContained)
```


Copie les formes de la plage vers la plage de destination.

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
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceShapes | [ShapeCollection](../../com.aspose.cells/shapecollection) | Formes source. |
| ca | [CellArea](../../com.aspose.cells/cellarea) | La plage source. |
| destRow | int | L'index de ligne de destination de la plage de destination. |
| destColumn | int | La colonne de destination de la plage de destination. |
| isContained | boolean | Indique s'il faut uniquement copier les formes qui sont contenues dans la plage. Si vrai, ne copie que les formes dans la plage. Sinon, cela fonctionne comme MS Office. |

### deleteInRange(CellArea ca) {#deleteInRange-com.aspose.cells.CellArea-}
```
public void deleteInRange(CellArea ca)
```


Supprime les formes de la plage. Les formes de commentaire ne seront pas supprimées.

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
| Paramètre | Type | Description |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | La plage. Si les formes sont contenues dans la plage, elles seront supprimées. |

### deleteShape(Shape shape) {#deleteShape-com.aspose.cells.Shape-}
```
public void deleteShape(Shape shape)
```


Supprimer une forme. Si la forme se trouve dans le groupe ou est une forme de commentaire, elle ne sera pas supprimée.

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
| Paramètre | Type | Description |
| --- | --- | --- |
| shape | [Shape](../../com.aspose.cells/shape) |  |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### find(String what, int previous, FindOptions findOptions) {#find-java.lang.String-int-com.aspose.cells.FindOptions-}
```
public int find(String what, int previous, FindOptions findOptions)
```


Trouve la forme par texte

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| quoi | java.lang.String | Le texte à rechercher. |
| précédent | int | L'index de la forme précédente contenant le même texte. -1 si la recherche commence depuis le début. |
| findOptions | [FindOptions](../../com.aspose.cells/findoptions) | Options de recherche |

**Returns:**
int - L'index de la forme trouvée, -1 si aucune forme n'est trouvée.
### get(int index) {#get-int-}
```
public Shape get(int index)
```


Obtient l'objet [Shape](../../com.aspose.cells/shape) à l'index spécifique dans la liste.

**Example**

```
         //get the first shape
         Shape shape = shapes.get(0);
```

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index. |

**Returns:**
[Shape](../../com.aspose.cells/shape) - 
### get(String name) {#get-java.lang.String-}
```
public Shape get(String name)
```


Obtient l'objet [Shape](../../com.aspose.cells/shape) par le nom de la forme.

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
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom de la forme. |

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


Obtient le nombre d'éléments contenus dans l'instance CollectionBase.

**Returns:**
int - Le nombre d'éléments contenus dans l'instance CollectionBase.
### group(Shape[] groupItems) {#group-com.aspose.cells.Shape---}
```
public GroupShape group(Shape[] groupItems)
```


Regroupe les formes.

**Remarks**

La forme dans groupItems ne doit pas être groupée. La forme doit se trouver dans cette collection Shapes.

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
| Paramètre | Type | Description |
| --- | --- | --- |
| groupItems | [Shape\[\]](../../com.aspose.cells/shape) | les éléments du groupe. |

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


Détermine l'index d'un élément spécifique dans l'instance CollectionBase.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | Détermine l'index d'un élément spécifique dans l'instance CollectionBase. |

**Returns:**
int - L'index de la valeur si elle est trouvée dans la liste ; sinon, -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Renvoie un énumérateur qui parcourt l'instance CollectionBase.

**Returns:**
java.util.Iterator - Un itérateur pour l'instance CollectionBase.
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


Supprime la forme.

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
| Paramètre | Type | Description |
| --- | --- | --- |
| shape | [Shape](../../com.aspose.cells/shape) |  |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Supprime la forme.

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
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index de la forme. |

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


Dégroupe les éléments de forme.

**Remarks**

Si la forme de groupe est groupée par une autre forme de groupe, aucune action ne sera effectuée.

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
| Paramètre | Type | Description |
| --- | --- | --- |
| group | [GroupShape](../../com.aspose.cells/groupshape) | La forme de groupe. |

### updateSelectedValue() {#updateSelectedValue--}
```
public void updateSelectedValue()
```


Met à jour la valeur sélectionnée avec la valeur de la cellule liée ou de la plage de la forme.

### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

