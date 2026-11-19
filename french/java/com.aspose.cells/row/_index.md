---
title: "Row"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente une ligne unique dans une feuille de calcul."
type: docs
url: /fr/java/com.aspose.cells/row/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Row implements Iterable
```

Représente une ligne unique dans une feuille de calcul.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
         Style style = workbook.createStyle();
 
         //Setting the background color to Blue
         style.setBackgroundColor(Color.getBlue());
 
         //Setting the foreground color to Red
         style.setForegroundColor(Color.getRed());
 
         //setting Background Pattern
         style.setPattern(BackgroundType.DIAGONAL_STRIPE);
 
         //New Style Flag
         StyleFlag styleFlag = new StyleFlag();
 
         //Set All Styles
         styleFlag.setAll(true);
 
          //Get first row
         Row row = worksheet.getCells().getRows().get(0);
          //Apply Style to first row
         row.applyStyle(style, styleFlag);
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Applique des formats à une ligne entière. |
| [copySettings(Row source, boolean checkStyle)](#copySettings-com.aspose.cells.Row-boolean-) | Copie les paramètres de la ligne, tels que le style, la hauteur, la visibilité, ...etc. |
| [equals(Row row)](#equals-com.aspose.cells.Row-) | Vérifie si cet objet fait référence à la même ligne qu'un autre objet ligne. |
| [equals(Object obj)](#equals-java.lang.Object-) | Vérifie si cet objet fait référence à la même ligne qu'un autre. |
| [get(int column)](#get-int-) | Obtient la cellule. |
| [getCellByIndex(int index)](#getCellByIndex-int-) | Obtenez la cellule par un index spécifique dans la collection de cellules de cette ligne. |
| [getCellOrNull(int column)](#getCellOrNull-int-) | Obtient la cellule ou null à l'index spécifié. |
| [getClass()](#getClass--) |  |
| [getFirstCell()](#getFirstCell--) | Obtient le premier objet cellule dans la ligne. |
| [getFirstDataCell()](#getFirstDataCell--) | Obtient la première cellule non vide dans la ligne. |
| [getGroupLevel()](#getGroupLevel--) | Obtient le niveau de groupe de la ligne. |
| [getHeight()](#getHeight--) | Obtient la hauteur de la ligne en points. |
| [getIndex()](#getIndex--) | Obtient l'index de cette ligne. |
| [getLastCell()](#getLastCell--) | Obtient le dernier objet cellule dans la ligne. |
| [getLastDataCell()](#getLastDataCell--) | Obtient la dernière cellule non vide dans la ligne. |
| [getStyle()](#getStyle--) | Obtient le style de cette ligne. |
| [hasCustomStyle()](#hasCustomStyle--) | Indique si cette ligne possède des paramètres de style personnalisés (différents de ceux par défaut hérités du classeur). |
| [hashCode()](#hashCode--) |  |
| [isBlank()](#isBlank--) | Indique si la ligne contient des données |
| [isCollapsed()](#isCollapsed--) | si la ligne est réduite |
| [isHeightMatched()](#isHeightMatched--) | Indique si la hauteur de la ligne correspond au paramètre de police par défaut actuel du classeur. |
| [isHidden()](#isHidden--) | Indique si la ligne est masquée. |
| [iterator()](#iterator--) | Obtient l'énumérateur de cellules |
| [iterator(boolean reversed, boolean sync)](#iterator-boolean-boolean-) | Obtient un énumérateur qui parcourt les cellules de cette ligne. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCollapsed(boolean value)](#setCollapsed-boolean-) | si la ligne est réduite |
| [setGroupLevel(byte value)](#setGroupLevel-byte-) | Obtient le niveau de groupe de la ligne. |
| [setHeight(double value)](#setHeight-double-) | Définit la hauteur de la ligne en points. |
| [setHeightMatched(boolean value)](#setHeightMatched-boolean-) | Indique si la hauteur de la ligne correspond au paramètre de police par défaut actuel du classeur. |
| [setHidden(boolean value)](#setHidden-boolean-) | Indique si la ligne est masquée. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Définit le style de cette ligne. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


Applique des formats à une ligne entière.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | L'objet de style qui sera appliqué. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Drapeaux qui indiquent les propriétés de formatage appliquées. |

### copySettings(Row source, boolean checkStyle) {#copySettings-com.aspose.cells.Row-boolean-}
```
public void copySettings(Row source, boolean checkStyle)
```


Copie les paramètres de la ligne, tels que le style, la hauteur, la visibilité, ...etc.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| source | [Row](../../com.aspose.cells/row) | la ligne source dont les paramètres seront copiés vers celle-ci |
| checkStyle | boolean | si vérifier et rassembler le style. Ne prend effet et n'est nécessaire que lorsque deux objets ligne appartiennent à des classeurs différents et que les styles des deux classeurs sont différents. |

### equals(Row row) {#equals-com.aspose.cells.Row-}
```
public boolean equals(Row row)
```


Vérifie si cet objet fait référence à la même ligne qu'un autre objet ligne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| row | [Row](../../com.aspose.cells/row) | un autre objet ligne |

**Returns:**
booléen - vrai si deux objets ligne font référence à la même ligne.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Vérifie si cet objet fait référence à la même ligne qu'un autre.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | un autre objet |

**Returns:**
booléen - vrai si deux objets font référence à la même ligne.
### get(int column) {#get-int-}
```
public Cell get(int column)
```


Obtient la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| colonne | int | L'index de colonne |

**Returns:**
[Cell](../../com.aspose.cells/cell) - 
### getCellByIndex(int index) {#getCellByIndex-int-}
```
public Cell getCellByIndex(int index)
```


Obtenez la cellule par un index spécifique dans la collection de cellules de cette ligne.

**Remarks**

Pour parcourir toutes les cellules en séquence sans modification, utiliser [iterator()](../../com.aspose.cells/row\#iterator--) offrira de meilleures performances que d'utiliser cette méthode pour obtenir les cellules une par une.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index (position) de la cellule dans la collection de cellules de cette ligne. |

**Returns:**
[Cell](../../com.aspose.cells/cell) - The Cell object at given position.
### getCellOrNull(int column) {#getCellOrNull-int-}
```
public Cell getCellOrNull(int column)
```


Obtient la cellule ou null à l'index spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| colonne | int | L'index de colonne |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Returns the cell object if the cell exists. Or returns null if the cell object does not exist.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFirstCell() {#getFirstCell--}
```
public Cell getFirstCell()
```


Obtient le premier objet cellule dans la ligne.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getFirstDataCell() {#getFirstDataCell--}
```
public Cell getFirstDataCell()
```


Obtient la première cellule non vide dans la ligne.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getGroupLevel() {#getGroupLevel--}
```
public byte getGroupLevel()
```


Obtient le niveau de groupe de la ligne.

**Returns:**
byte
### getHeight() {#getHeight--}
```
public double getHeight()
```


Obtient la hauteur de la ligne en points.

**Returns:**
double
### getIndex() {#getIndex--}
```
public int getIndex()
```


Obtient l'index de cette ligne.

**Returns:**
int
### getLastCell() {#getLastCell--}
```
public Cell getLastCell()
```


Obtient le dernier objet cellule dans la ligne.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getLastDataCell() {#getLastDataCell--}
```
public Cell getLastDataCell()
```


Obtient la dernière cellule non vide dans la ligne.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Obtient le style de cette ligne.

**Remarks**

Modifier directement l'objet de style retourné n'a aucun effet sur cette ligne ou sur les cellules de cette ligne. Vous devez appeler la méthode [applyStyle(Style,StyleFlag)](../../com.aspose.cells/row\#applyStyle-Style-StyleFlag-) ou [setStyle(Style)](../../com.aspose.cells/row\#setStyle-Style-) pour appliquer la modification à cette ligne.

Le style de la ligne est le style qui sera hérité par les cellules de cette ligne (ces cellules qui n'ont pas de paramètres de style personnalisés, comme les cellules existantes qui n'ont pas été explicitement stylisées, ou celles qui n'ont pas été instanciées).

**Returns:**
[Style](../../com.aspose.cells/style)
### hasCustomStyle() {#hasCustomStyle--}
```
public boolean hasCustomStyle()
```


Indique si cette ligne possède des paramètres de style personnalisés (différents de ceux par défaut hérités du classeur).

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBlank() {#isBlank--}
```
public boolean isBlank()
```


Indique si la ligne contient des données

**Returns:**
boolean
### isCollapsed() {#isCollapsed--}
```
public boolean isCollapsed()
```


si la ligne est réduite

**Returns:**
boolean
### isHeightMatched() {#isHeightMatched--}
```
public boolean isHeightMatched()
```


Indique si la hauteur de la ligne correspond au paramètre de police par défaut actuel du classeur. La valeur vraie de cette propriété indique également que la hauteur de la ligne est « automatique » sans valeur de hauteur personnalisée définie par l'utilisateur.

**Remarks**

Lorsque cette propriété est vraie, si le contenu de cette ligne change, la hauteur de la ligne doit généralement être recalculée (par exemple via [Worksheet.autoFitRows()](../../com.aspose.cells/worksheet\#autoFitRows--)) pour obtenir le même résultat que celui affiché dans MS Excel lors de l'ouverture du classeur.

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Indique si la ligne est masquée.

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


Obtient l'énumérateur de cellules

**Example**

```
         Workbook workbook = new Workbook("template.xlsx");
         	Cells cells = workbook.getWorksheets().get(0).getCells();
 
         	Iterator en = cells.getRows().get(1).iterator();
         	while (en.hasNext())
         	{
         	    Cell cell = (Cell)en.next();
         	    System.out.println(cell.getName() + ": " + cell.getValue());
         	}
```

**Returns:**
java.util.Iterator - L'énumérateur de cellules qui parcourra toutes les cellules existantes de cette ligne.
### iterator(boolean reversed, boolean sync) {#iterator-boolean-boolean-}
```
public Iterator iterator(boolean reversed, boolean sync)
```


Obtient un énumérateur qui parcourt les cellules de cette ligne.

**Remarks**

Si la ligne doit être modifiée (par des opérations pouvant entraîner l'instanciation d'une nouvelle Cellule ou la suppression d'une Cellule existante) pendant le parcours avec l'énumérateur, un énumérateur synchronisé doit être utilisé à la place d'un énumérateur normal afin que le parcours puisse reprendre à la position immédiatement après celle qui a été parcourue par le dernier MoveNext(). Cependant, en plus de l'avantage qu'aucun élément ne soit sauté ou parcouru plusieurs fois, l'inconvénient de l'énumérateur synchronisé est que les performances seront légèrement dégradées comparées à un énumérateur normal.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| inversé | boolean | si énumérer les cellules dans l'ordre inverse |
| synchroniser | boolean | si l'énumérateur retourné doit vérifier la modification des cellules dans cette ligne et rester synchronisé avec elle. |

**Returns:**
java.util.Iterator - L'énumérateur de cellules qui parcourra toutes les cellules existantes de cette ligne.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setCollapsed(boolean value) {#setCollapsed-boolean-}
```
public void setCollapsed(boolean value)
```


si la ligne est réduite

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setGroupLevel(byte value) {#setGroupLevel-byte-}
```
public void setGroupLevel(byte value)
```


Obtient le niveau de groupe de la ligne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | byte |  |

### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


Définit la hauteur de la ligne en points.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setHeightMatched(boolean value) {#setHeightMatched-boolean-}
```
public void setHeightMatched(boolean value)
```


Indique si la hauteur de la ligne correspond au paramètre de police par défaut actuel du classeur. La valeur vraie de cette propriété indique également que la hauteur de la ligne est « automatique » sans valeur de hauteur personnalisée définie par l'utilisateur.

**Remarks**

Lorsque cette propriété est vraie, si le contenu de cette ligne change, la hauteur de la ligne doit généralement être recalculée (par exemple via [Worksheet.autoFitRows()](../../com.aspose.cells/worksheet\#autoFitRows--)) pour obtenir le même résultat que celui affiché dans MS Excel lors de l'ouverture du classeur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Indique si la ligne est masquée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


Définit le style de cette ligne.

**Remarks**

Cette méthode définit uniquement le style donné comme style par défaut pour cette ligne, sans modifier les paramètres de style des cellules existantes dans cette ligne. Pour mettre à jour les paramètres de style des cellules existantes avec le style spécifié en même temps, veuillez utiliser [applyStyle(Style,StyleFlag)](../../com.aspose.cells/row\#applyStyle-Style-StyleFlag-)

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | le style à utiliser comme style par défaut pour les cellules de cette ligne. |

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

