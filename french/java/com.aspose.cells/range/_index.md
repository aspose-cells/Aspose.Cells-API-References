---
title: "Range"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Encapsule l'objet qui représente une plage de cellules dans une feuille de calcul."
type: docs
url: /fr/java/com.aspose.cells/range/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Range implements Iterable
```

Encapsule l'objet qui représente une plage de cellules dans une feuille de calcul.

**Remarks**

La classe Range d\u00e9signe une région d\'une feuille de calcul Excel. Avec cela, vous pouvez formater et définir la valeur de la plage. Et vous pouvez également copier simplement une plage d\'Excel.

**Example**

L\'exemple suivant montre comment créer une plage et définir la valeur de la plage d\'Excel.

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
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [Range(CellArea ca, Cells cells)](#Range-com.aspose.cells.CellArea-com.aspose.cells.Cells-) | Constructeur de classe. |
| [Range(int firstRow, int firstColumn, int rowNumber, int columnNumber, Cells cells)](#Range-int-int-int-int-com.aspose.cells.Cells-) | Constructeur de classe. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [addHyperlink(String address, String textToDisplay, String screenTip)](#addHyperlink-java.lang.String-java.lang.String-java.lang.String-) | Ajoute un hyperlien à une cellule spécifiée ou à une plage de cellules. |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Applique des formats à une plage entière. |
| [autoFill(Range target)](#autoFill-com.aspose.cells.Range-) | Remplit automatiquement la plage cible. |
| [autoFill(Range target, int autoFillType)](#autoFill-com.aspose.cells.Range-int-) | Remplit automatiquement la plage cible. |
| [clear()](#clear--) | Efface cette plage. |
| [clearComments()](#clearComments--) | Efface les commentaires de cette plage. |
| [clearContents()](#clearContents--) | Efface le contenu de cette plage. |
| [clearFormats()](#clearFormats--) | Efface les formats de cette plage. |
| [clearHyperlinks(boolean clearFormat)](#clearHyperlinks-boolean-) | Supprime uniquement les hyperliens. |
| [copy(Range range)](#copy-com.aspose.cells.Range-) | Copie les données (y compris les formules), le formatage, les objets de dessin, etc., depuis une plage source. |
| [copy(Range range, PasteOptions options)](#copy-com.aspose.cells.Range-com.aspose.cells.PasteOptions-) | Copie la plage avec les options de collage spécial. |
| [copyData(Range range)](#copyData-com.aspose.cells.Range-) | Copie les données de cellules (y compris les formules) depuis une plage source. |
| [copyStyle(Range range)](#copyStyle-com.aspose.cells.Range-) | Copie les paramètres de style d’une plage source. |
| [copyValue(Range range)](#copyValue-com.aspose.cells.Range-) | Copie la valeur de la cellule d’une plage source. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int rowOffset, int columnOffset)](#get-int-int-) | Obtient l’objet [Cell](../../com.aspose.cells/cell) dans cette plage. |
| [getAddress()](#getAddress--) | Obtient l’adresse de la plage. |
| [getCellOrNull(int rowOffset, int columnOffset)](#getCellOrNull-int-int-) | Obtient l’objet [Cell](../../com.aspose.cells/cell) ou null dans cette plage. |
| [getClass()](#getClass--) |  |
| [getColumnCount()](#getColumnCount--) | Obtient le nombre de colonnes dans la plage. |
| [getColumnWidth()](#getColumnWidth--) | Définit ou obtient la largeur de colonne de cette plage |
| [getCurrentRegion()](#getCurrentRegion--) | Renvoie un objet Range qui représente la région actuelle. |
| [getEntireColumn()](#getEntireColumn--) | Obtient un objet Range qui représente la colonne entière (ou les colonnes) contenant la plage spécifiée. |
| [getEntireRow()](#getEntireRow--) | Obtient un objet Range qui représente la ligne entière (ou les lignes) contenant la plage spécifiée. |
| [getFirstColumn()](#getFirstColumn--) | Obtient l’indice de la première colonne de la plage. |
| [getFirstRow()](#getFirstRow--) | Obtient l’indice de la première ligne de la plage. |
| [getHeight()](#getHeight--) | Obtient la largeur d’une plage en points. |
| [getHyperlinks()](#getHyperlinks--) | Obtient tous les hyperliens dans la plage. |
| [getLeft()](#getLeft--) | Obtient la distance, en points, du bord gauche de la colonne A au bord gauche de la plage. |
| [getName()](#getName--) | Obtient le nom de la plage. |
| [getOffset(int rowOffset, int columnOffset)](#getOffset-int-int-) | Obtient la plage [Range](../../com.aspose.cells/range) par décalage. |
| [getRefersTo()](#getRefersTo--) | Obtient la référence de la plage. |
| [getRowCount()](#getRowCount--) | Obtient le nombre de lignes dans la plage. |
| [getRowHeight()](#getRowHeight--) | Définit ou obtient la hauteur des lignes dans cette plage |
| [getTop()](#getTop--) | Obtient la distance, en points, du bord supérieur de la ligne 1 au bord supérieur de la plage. |
| [getValue()](#getValue--) | Obtient la valeur de la plage. |
| [getWidth()](#getWidth--) | Obtient la largeur d’une plage en points. |
| [getWorksheet()](#getWorksheet--) | Obtient l’objet [getWorksheet()](../../com.aspose.cells/range\#getWorksheet--) qui contient cette plage. |
| [hashCode()](#hashCode--) |  |
| [intersect(Range range)](#intersect-com.aspose.cells.Range-) | Renvoie un objet [Range](../../com.aspose.cells/range) qui représente l’intersection rectangulaire de deux plages. |
| [isBlank()](#isBlank--) | Indique si la plage contient des valeurs. |
| [isIntersect(Range range)](#isIntersect-com.aspose.cells.Range-) | Indique si la plage intersecte. |
| [iterator()](#iterator--) | Obtient l'énumérateur des cellules de cette Range. |
| [merge()](#merge--) | Combine une plage de cellules en une seule cellule. |
| [moveTo(int destRow, int destColumn)](#moveTo-int-int-) | Déplace la plage actuelle vers la plage dest. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | Insère une valeur dans la plage, le cas échéant la valeur sera convertie en un autre type de données et le format numérique de la cellule sera réinitialisé. |
| [setColumnWidth(double value)](#setColumnWidth-double-) | Définit ou obtient la largeur de colonne de cette plage |
| [setInsideBorders(int borderEdge, int lineStyle, CellsColor borderColor)](#setInsideBorders-int-int-com.aspose.cells.CellsColor-) | Définit les bordures internes de la plage. |
| [setName(String value)](#setName-java.lang.String-) | Définit le nom de la plage. |
| [setOutlineBorder(int borderEdge, int borderStyle, CellsColor borderColor)](#setOutlineBorder-int-int-com.aspose.cells.CellsColor-) | Définit la bordure extérieure autour d'une plage de cellules. |
| [setOutlineBorder(int borderEdge, int borderStyle, Color borderColor)](#setOutlineBorder-int-int-com.aspose.cells.Color-) | Définit la bordure extérieure autour d'une plage de cellules. |
| [setOutlineBorders(int borderStyle, CellsColor borderColor)](#setOutlineBorders-int-com.aspose.cells.CellsColor-) | Définit les bordures extérieures autour d'une plage de cellules avec le même style et la même couleur de bordure. |
| [setOutlineBorders(int borderStyle, Color borderColor)](#setOutlineBorders-int-com.aspose.cells.Color-) | Définit les bordures extérieures autour d'une plage de cellules avec le même style et la même couleur de bordure. |
| [setOutlineBorders(int[] borderStyles, Color[] borderColors)](#setOutlineBorders-int---com.aspose.cells.Color---) | Définit les bordures extérieures autour d'une plage de cellules. |
| [setRowHeight(double value)](#setRowHeight-double-) | Définit ou obtient la hauteur des lignes dans cette plage |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Définit le style de la plage. |
| [setStyle(Style style, boolean explicitFlag)](#setStyle-com.aspose.cells.Style-boolean-) | Applique le style de la cellule. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Définit la valeur de la plage. |
| [toHtml(HtmlSaveOptions saveOptions)](#toHtml-com.aspose.cells.HtmlSaveOptions-) | Convertit la plage en HTML. |
| [toImage(ImageOrPrintOptions options)](#toImage-com.aspose.cells.ImageOrPrintOptions-) | Convertit la plage en image. |
| [toJson(JsonSaveOptions options)](#toJson-com.aspose.cells.JsonSaveOptions-) | Convertit la plage en valeur JSON. |
| [toString()](#toString--) | Renvoie une chaîne représentant l'objet Range actuel. |
| [transpose()](#transpose--) | Transpose (fait pivoter) les données des lignes aux colonnes ou inversement. |
| [unMerge()](#unMerge--) | Démarque les cellules fusionnées de cette plage. |
| [union(Range range)](#union-com.aspose.cells.Range-) | Renvoie l'union de deux plages. |
| [unionRang(Range range)](#unionRang-com.aspose.cells.Range-) | Renvoie le résultat de l'union de deux plages. |
| [unionRanges(Range[] ranges)](#unionRanges-com.aspose.cells.Range---) | Renvoie le résultat de l'union de deux plages. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Range(CellArea ca, Cells cells) {#Range-com.aspose.cells.CellArea-com.aspose.cells.Cells-}
```
public Range(CellArea ca, Cells cells)
```


Constructeur de classe.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | La plage. |
| cells | [Cells](../../com.aspose.cells/cells) |  |

### Range(int firstRow, int firstColumn, int rowNumber, int columnNumber, Cells cells) {#Range-int-int-int-int-com.aspose.cells.Cells-}
```
public Range(int firstRow, int firstColumn, int rowNumber, int columnNumber, Cells cells)
```


Constructeur de classe.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| firstRow | int | Première ligne de cette plage (index zéro) |
| firstColumn | int | Première colonne de cette plage (base zéro) |
| rowNumber | int | Nombre de lignes (index à partir de 1) |
| columnNumber | int | Nombre de colonnes (base 1) |
| cells | [Cells](../../com.aspose.cells/cells) | L'objet Range appartient à cet objet Cells |

### addHyperlink(String address, String textToDisplay, String screenTip) {#addHyperlink-java.lang.String-java.lang.String-java.lang.String-}
```
public Hyperlink addHyperlink(String address, String textToDisplay, String screenTip)
```


Ajoute un hyperlien à une cellule spécifiée ou à une plage de cellules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| adresse | java.lang.String | Adresse du lien hypertexte. |
| textToDisplay | java.lang.String | Le texte à afficher pour le lien hypertexte spécifié. |
| screenTip | java.lang.String | Le texte d’infobulle pour le lien hypertexte spécifié. |

**Returns:**
[Hyperlink](../../com.aspose.cells/hyperlink) - [Hyperlink](../../com.aspose.cells/hyperlink) object.
### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


Applique des formats à une plage entière.

**Remarks**

Chaque cellule de cette plage contiendra un objet [Style](../../com.aspose.cells/style). Ainsi, cette méthode consomme beaucoup de mémoire. Veuillez l'utiliser avec précaution.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | L'objet de style qui sera appliqué. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Drapeaux qui indiquent les propriétés de formatage appliquées. |

### autoFill(Range target) {#autoFill-com.aspose.cells.Range-}
```
public void autoFill(Range target)
```


Remplit automatiquement la plage cible.

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
| Paramètre | Type | Description |
| --- | --- | --- |
| target | [Range](../../com.aspose.cells/range) | la plage cible. |

### autoFill(Range target, int autoFillType) {#autoFill-com.aspose.cells.Range-int-}
```
public void autoFill(Range target, int autoFillType)
```


Remplit automatiquement la plage cible.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| target | [Range](../../com.aspose.cells/range) | La plage ciblée. |
| autoFillType | int | [AutoFillType](../../com.aspose.cells/autofilltype). Le type de remplissage automatique. |

### clear() {#clear--}
```
public void clear()
```


Efface cette plage.

### clearComments() {#clearComments--}
```
public void clearComments()
```


Efface les commentaires de cette plage.

### clearContents() {#clearContents--}
```
public void clearContents()
```


Efface le contenu de cette plage.

### clearFormats() {#clearFormats--}
```
public void clearFormats()
```


Efface les formats de cette plage.

### clearHyperlinks(boolean clearFormat) {#clearHyperlinks-boolean-}
```
public void clearHyperlinks(boolean clearFormat)
```


Supprime uniquement les hyperliens.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| clearFormat | boolean | Indique si le format des hyperliens doit être effacé. |

### copy(Range range) {#copy-com.aspose.cells.Range-}
```
public void copy(Range range)
```


Copie les données (y compris les formules), le formatage, les objets de dessin, etc., depuis une plage source.

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
| Paramètre | Type | Description |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Objet [Range](../../com.aspose.cells/range) source. |

### copy(Range range, PasteOptions options) {#copy-com.aspose.cells.Range-com.aspose.cells.PasteOptions-}
```
public void copy(Range range, PasteOptions options)
```


Copie la plage avec les options de collage spécial.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | La plage source. |
| options | [PasteOptions](../../com.aspose.cells/pasteoptions) | Les options de collage spécial. |

### copyData(Range range) {#copyData-com.aspose.cells.Range-}
```
public void copyData(Range range)
```


Copie les données de cellules (y compris les formules) depuis une plage source.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Objet [Range](../../com.aspose.cells/range) source. |

### copyStyle(Range range) {#copyStyle-com.aspose.cells.Range-}
```
public void copyStyle(Range range)
```


Copie les paramètres de style d’une plage source.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Objet [Range](../../com.aspose.cells/range) source. |

### copyValue(Range range) {#copyValue-com.aspose.cells.Range-}
```
public void copyValue(Range range)
```


Copie la valeur de la cellule d’une plage source.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Objet [Range](../../com.aspose.cells/range) source. |

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
### get(int rowOffset, int columnOffset) {#get-int-int-}
```
public Cell get(int rowOffset, int columnOffset)
```


Obtient l’objet [Cell](../../com.aspose.cells/cell) dans cette plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowOffset | int | Décalage de ligne dans cette plage, basé sur zéro. |
| columnOffset | int | Décalage de colonne dans cette plage, basé sur zéro. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - [Cell](../../com.aspose.cells/cell) object.
### getAddress() {#getAddress--}
```
public String getAddress()
```


Obtient l’adresse de la plage.

**Returns:**
java.lang.String
### getCellOrNull(int rowOffset, int columnOffset) {#getCellOrNull-int-int-}
```
public Cell getCellOrNull(int rowOffset, int columnOffset)
```


Obtient l’objet [Cell](../../com.aspose.cells/cell) ou null dans cette plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowOffset | int | Décalage de ligne dans cette plage, basé sur zéro. |
| columnOffset | int | Décalage de colonne dans cette plage, basé sur zéro. |

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


Obtient le nombre de colonnes dans la plage.

**Returns:**
int
### getColumnWidth() {#getColumnWidth--}
```
public double getColumnWidth()
```


Définit ou obtient la largeur de colonne de cette plage

**Returns:**
double
### getCurrentRegion() {#getCurrentRegion--}
```
public Range getCurrentRegion()
```


Renvoie un objet Range qui représente la région actuelle. La région actuelle est une plage délimitée par toute combinaison de lignes vides et de colonnes vides.

**Returns:**
[Range](../../com.aspose.cells/range)
### getEntireColumn() {#getEntireColumn--}
```
public Range getEntireColumn()
```


Obtient un objet Range qui représente la colonne entière (ou les colonnes) contenant la plage spécifiée.

**Returns:**
[Range](../../com.aspose.cells/range)
### getEntireRow() {#getEntireRow--}
```
public Range getEntireRow()
```


Obtient un objet Range qui représente la ligne entière (ou les lignes) contenant la plage spécifiée.

**Returns:**
[Range](../../com.aspose.cells/range)
### getFirstColumn() {#getFirstColumn--}
```
public int getFirstColumn()
```


Obtient l’indice de la première colonne de la plage.

**Returns:**
int
### getFirstRow() {#getFirstRow--}
```
public int getFirstRow()
```


Obtient l’indice de la première ligne de la plage.

**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```


Obtient la largeur d’une plage en points.

**Returns:**
double
### getHyperlinks() {#getHyperlinks--}
```
public Hyperlink[] getHyperlinks()
```


Obtient tous les hyperliens dans la plage.

**Returns:**
com.aspose.cells.Hyperlink[]
### getLeft() {#getLeft--}
```
public double getLeft()
```


Obtient la distance, en points, du bord gauche de la colonne A au bord gauche de la plage.

**Returns:**
double
### getName() {#getName--}
```
public String getName()
```


Obtient le nom de la plage.

**Remarks**

La plage nommée est prise en charge. Par exemple,

range.Name = "Sheet1!MyRange";

**Returns:**
java.lang.String
### getOffset(int rowOffset, int columnOffset) {#getOffset-int-int-}
```
public Range getOffset(int rowOffset, int columnOffset)
```


Obtient la plage [Range](../../com.aspose.cells/range) par décalage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowOffset | int | Décalage de ligne dans cette plage, basé sur zéro. |
| columnOffset | int | Décalage de colonne dans cette plage, basé sur zéro. |

**Returns:**
[Range](../../com.aspose.cells/range) - 
### getRefersTo() {#getRefersTo--}
```
public String getRefersTo()
```


Obtient la référence de la plage.

**Returns:**
java.lang.String
### getRowCount() {#getRowCount--}
```
public int getRowCount()
```


Obtient le nombre de lignes dans la plage.

**Returns:**
int
### getRowHeight() {#getRowHeight--}
```
public double getRowHeight()
```


Définit ou obtient la hauteur des lignes dans cette plage

**Returns:**
double
### getTop() {#getTop--}
```
public double getTop()
```


Obtient la distance, en points, du bord supérieur de la ligne 1 au bord supérieur de la plage.

**Returns:**
double
### getValue() {#getValue--}
```
public Object getValue()
```


Obtient la valeur de la plage.

**Remarks**

Si la plage contient plusieurs cellules, l'objet retourné/appliqué doit être Object[][].

**Returns:**
java.lang.Object
### getWidth() {#getWidth--}
```
public double getWidth()
```


Obtient la largeur d’une plage en points.

**Returns:**
double
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Obtient l’objet [getWorksheet()](../../com.aspose.cells/range\#getWorksheet--) qui contient cette plage.

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


Renvoie un objet [Range](../../com.aspose.cells/range) qui représente l’intersection rectangulaire de deux plages.

**Remarks**

Si les deux plages ne se croisent pas, renvoie null.

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
| Paramètre | Type | Description |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | La plage d'intersection. |

**Returns:**
[Range](../../com.aspose.cells/range) - Returns a [Range](../../com.aspose.cells/range) object
### isBlank() {#isBlank--}
```
public boolean isBlank()
```


Indique si la plage contient des valeurs.

**Returns:**
boolean -
### isIntersect(Range range) {#isIntersect-com.aspose.cells.Range-}
```
public boolean isIntersect(Range range)
```


Indique si la plage intersecte.

**Remarks**

Si les deux plages ne sont pas dans la même feuille de calcul, renvoie false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | La plage. |

**Returns:**
booléen - Indique si la plage se intersecte.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Obtient l'énumérateur des cellules de cette Range.

**Remarks**

Lors du parcours des éléments à l'aide de l'énumérateur retourné, la collection de cellules ne doit pas être modifiée (par exemple des opérations qui créeraient de nouvelles Cell/Row ou supprimeraient des Cell/Row existantes). Sinon, l'énumérateur pourrait ne pas être capable de parcourir correctement toutes les cellules (certains éléments pourraient être parcourus plusieurs fois ou être ignorés).

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
java.util.Iterator - L'énumérateur de cellules
### merge() {#merge--}
```
public void merge()
```


Combine une plage de cellules en une seule cellule.

**Remarks**

Référez la cellule fusionnée via l'adresse de la cellule en haut à gauche de la plage.

### moveTo(int destRow, int destColumn) {#moveTo-int-int-}
```
public void moveTo(int destRow, int destColumn)
```


Déplace la plage actuelle vers la plage dest.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| destRow | int | La ligne de départ de la plage de destination. |
| destColumn | int | La colonne de départ de la plage de destination. |

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


Insère une valeur dans la plage, le cas échéant la valeur sera convertie en un autre type de données et le format numérique de la cellule sera réinitialisé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| stringValue | java.lang.String | Valeur d'entrée |
| isConverted | boolean | True : converti en un autre type de données si approprié. |
| setStyle | boolean | True : définir le format numérique dans le style de la cellule lors de la conversion en un autre type de données |

### setColumnWidth(double value) {#setColumnWidth-double-}
```
public void setColumnWidth(double value)
```


Définit ou obtient la largeur de colonne de cette plage

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setInsideBorders(int borderEdge, int lineStyle, CellsColor borderColor) {#setInsideBorders-int-int-com.aspose.cells.CellsColor-}
```
public void setInsideBorders(int borderEdge, int lineStyle, CellsColor borderColor)
```


Définit les bordures internes de la plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| borderEdge | int | [BorderType](../../com.aspose.cells/bordertype). À l'intérieur du type de bordure, seules les valeurs [BorderType.VERTICAL](../../com.aspose.cells/bordertype\#VERTICAL) et [BorderType.HORIZONTAL](../../com.aspose.cells/bordertype\#HORIZONTAL) sont autorisées. |
| lineStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Le style de bordure. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | La couleur de la bordure. |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Définit le nom de la plage.

**Remarks**

La plage nommée est prise en charge. Par exemple,

range.Name = "Sheet1!MyRange";

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setOutlineBorder(int borderEdge, int borderStyle, CellsColor borderColor) {#setOutlineBorder-int-int-com.aspose.cells.CellsColor-}
```
public void setOutlineBorder(int borderEdge, int borderStyle, CellsColor borderColor)
```


Définit la bordure extérieure autour d'une plage de cellules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| borderEdge | int | [BorderType](../../com.aspose.cells/bordertype). Bord de la bordure. |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Style de bordure. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | Couleur de la bordure. |

### setOutlineBorder(int borderEdge, int borderStyle, Color borderColor) {#setOutlineBorder-int-int-com.aspose.cells.Color-}
```
public void setOutlineBorder(int borderEdge, int borderStyle, Color borderColor)
```


Définit la bordure extérieure autour d'une plage de cellules.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| borderEdge | int | [BorderType](../../com.aspose.cells/bordertype). Bord de la bordure. |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Style de bordure. |
| borderColor | [Color](../../com.aspose.cells/color) | Couleur de la bordure. |

### setOutlineBorders(int borderStyle, CellsColor borderColor) {#setOutlineBorders-int-com.aspose.cells.CellsColor-}
```
public void setOutlineBorders(int borderStyle, CellsColor borderColor)
```


Définit les bordures extérieures autour d'une plage de cellules avec le même style et la même couleur de bordure.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Style de bordure. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | Couleur de la bordure. |

### setOutlineBorders(int borderStyle, Color borderColor) {#setOutlineBorders-int-com.aspose.cells.Color-}
```
public void setOutlineBorders(int borderStyle, Color borderColor)
```


Définit les bordures extérieures autour d'une plage de cellules avec le même style et la même couleur de bordure.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Style de bordure. |
| borderColor | [Color](../../com.aspose.cells/color) | Couleur de la bordure. |

### setOutlineBorders(int[] borderStyles, Color[] borderColors) {#setOutlineBorders-int---com.aspose.cells.Color---}
```
public void setOutlineBorders(int[] borderStyles, Color[] borderColors)
```


Définit les bordures extérieures autour d'une plage de cellules.

**Remarks**

La longueur de borderStyles et de borderStyles doit être de 4. L'ordre de borderStyles et de borderStyles doit être haut,bas,gauche,droite.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| borderStyles | int[] | [CellBorderType](../../com.aspose.cells/cellbordertype). Styles de bordure. |
| borderColors | [Color\[\]](../../com.aspose.cells/color) | Couleurs des bordures. |

### setRowHeight(double value) {#setRowHeight-double-}
```
public void setRowHeight(double value)
```


Définit ou obtient la hauteur des lignes dans cette plage

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


Définit le style de la plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | L'objet Style. |

### setStyle(Style style, boolean explicitFlag) {#setStyle-com.aspose.cells.Style-boolean-}
```
public void setStyle(Style style, boolean explicitFlag)
```


Applique le style de la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Le style de cellule. |
| explicitFlag | boolean | Vrai, uniquement en écrasant le formatage qui est explicitement défini. |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Définit la valeur de la plage.

**Remarks**

Si la plage contient plusieurs cellules, l'objet retourné/appliqué doit être Object[][].

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.Object |  |

### toHtml(HtmlSaveOptions saveOptions) {#toHtml-com.aspose.cells.HtmlSaveOptions-}
```
public byte[] toHtml(HtmlSaveOptions saveOptions)
```


Convertit la plage en HTML.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| saveOptions | [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions) | Options pour convertir la plage en HTML. |

**Returns:**
byte[] -
### toImage(ImageOrPrintOptions options) {#toImage-com.aspose.cells.ImageOrPrintOptions-}
```
public byte[] toImage(ImageOrPrintOptions options)
```


Convertit la plage en image.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | Les options pour convertir cette plage en image |

**Returns:**
byte[] -
### toJson(JsonSaveOptions options) {#toJson-com.aspose.cells.JsonSaveOptions-}
```
public String toJson(JsonSaveOptions options)
```


Convertit la plage en valeur JSON.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| options | [JsonSaveOptions](../../com.aspose.cells/jsonsaveoptions) | Les options de conversion |

**Returns:**
java.lang.String -
### toString() {#toString--}
```
public String toString()
```


Renvoie une chaîne représentant l'objet Range actuel.

**Returns:**
java.lang.String -
### transpose() {#transpose--}
```
public void transpose()
```


Transpose (fait pivoter) les données des lignes aux colonnes ou inversement.

### unMerge() {#unMerge--}
```
public void unMerge()
```


Démarque les cellules fusionnées de cette plage.

### union(Range range) {#union-com.aspose.cells.Range-}
```
public ArrayList union(Range range)
```


Renvoie l'union de deux plages.

**Remarks**

REMARQUE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode Range.UnionRanges(). Cette méthode sera supprimée 12 mois plus tard, à compter de novembre 2023. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | La plage |

**Returns:**
java.util.ArrayList - L'union de deux plages.
### unionRang(Range range) {#unionRang-com.aspose.cells.Range-}
```
public Range[] unionRang(Range range)
```


Renvoie le résultat de l'union de deux plages.

**Remarks**

REMARQUE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode Range.UnionRanges(). Cette méthode sera supprimée 12 mois plus tard, à compter de mai 2024. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | La plage |

**Returns:**
com.aspose.cells.Range[] - L'union de deux plages.
### unionRanges(Range[] ranges) {#unionRanges-com.aspose.cells.Range---}
```
public UnionRange unionRanges(Range[] ranges)
```


Renvoie le résultat de l'union de deux plages.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ranges | [Range\[\]](../../com.aspose.cells/range) | La plage |

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

