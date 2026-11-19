---
title: "UnionRange"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente une plage d'union."
type: docs
url: /fr/java/com.aspose.cells/unionrange/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class UnionRange implements Iterable
```

Représente une plage d'union.
## Méthodes

| Méthode | Description |
| --- | --- |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Applique des formats à une plage entière. |
| [copy(UnionRange range, PasteOptions options)](#copy-com.aspose.cells.UnionRange-com.aspose.cells.PasteOptions-) | Copie la plage avec les options de collage spécial. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellCount()](#getCellCount--) | Obtient le nombre total de cellules dans la plage. |
| [getClass()](#getClass--) |  |
| [getColumnCount()](#getColumnCount--) | Obtient le nombre de lignes dans la plage. |
| [getFirstColumn()](#getFirstColumn--) | Obtient l’indice de la première colonne de la plage. |
| [getFirstRow()](#getFirstRow--) | Obtient l’indice de la première ligne de la plage. |
| [getHyperlinks()](#getHyperlinks--) | Obtient tous les hyperliens dans la plage. |
| [getName()](#getName--) | Obtient le nom de la plage. |
| [getRangeCount()](#getRangeCount--) | Obtient le nombre de plages. |
| [getRanges()](#getRanges--) | Obtient toutes les plages d'union. |
| [getRefersTo()](#getRefersTo--) | Obtient la référence de la plage. |
| [getRowCount()](#getRowCount--) | Obtient le nombre de lignes dans la plage. |
| [getValue()](#getValue--) | Obtient les valeurs de la plage. |
| [hasRange()](#hasRange--) | Indique si cela possède une plage. |
| [hashCode()](#hashCode--) |  |
| [intersect(Range[] ranges)](#intersect-com.aspose.cells.Range---) | Intersecte une autre plage. |
| [intersect(UnionRange unionRange)](#intersect-com.aspose.cells.UnionRange-) | Intersecte une autre plage. |
| [intersect(String range)](#intersect-java.lang.String-) | Intersecte une autre plage. |
| [iterator()](#iterator--) | Obtient l'énumérateur des cellules de cette Range. |
| [merge()](#merge--) | Combine une plage de cellules en une seule cellule. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | Insère une valeur dans la plage, le cas échéant la valeur sera convertie en un autre type de données et le format numérique de la cellule sera réinitialisé. |
| [setName(String value)](#setName-java.lang.String-) | Définit le nom de la plage. |
| [setOutlineBorders(int borderStyle, Color borderColor)](#setOutlineBorders-int-com.aspose.cells.Color-) | Définit les bordures extérieures autour d'une plage de cellules avec le même style et la même couleur de bordure. |
| [setOutlineBorders(int[] borderStyles, Color[] borderColors)](#setOutlineBorders-int---com.aspose.cells.Color---) | Définit les bordures extérieures autour d'une plage de cellules. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Définit le style de la plage. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Définit les valeurs de la plage. |
| [toString()](#toString--) |  |
| [unMerge()](#unMerge--) | Démarque les cellules fusionnées de cette plage. |
| [union(Range[] ranges)](#union-com.aspose.cells.Range---) | Union des plages. |
| [union(UnionRange unionRange)](#union-com.aspose.cells.UnionRange-) | Union d'une autre plage. |
| [union(String range)](#union-java.lang.String-) | Union d'une autre plage. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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

### copy(UnionRange range, PasteOptions options) {#copy-com.aspose.cells.UnionRange-com.aspose.cells.PasteOptions-}
```
public void copy(UnionRange range, PasteOptions options)
```


Copie la plage avec les options de collage spécial.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| range | [UnionRange](../../com.aspose.cells/unionrange) | La plage source. |
| options | [PasteOptions](../../com.aspose.cells/pasteoptions) | Les options de collage spécial. |

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
### getCellCount() {#getCellCount--}
```
public int getCellCount()
```


Obtient le nombre total de cellules dans la plage.

**Returns:**
int
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


Obtient le nombre de lignes dans la plage.

**Remarks**

N'affecte que lorsqu'il ne contient qu'une seule plage.

**Returns:**
int
### getFirstColumn() {#getFirstColumn--}
```
public int getFirstColumn()
```


Obtient l’indice de la première colonne de la plage.

**Remarks**

N'affecte que lorsqu'il ne contient qu'une seule plage.

**Returns:**
int
### getFirstRow() {#getFirstRow--}
```
public int getFirstRow()
```


Obtient l’indice de la première ligne de la plage.

**Remarks**

N'affecte que lorsqu'il ne contient qu'une seule plage.

**Returns:**
int
### getHyperlinks() {#getHyperlinks--}
```
public Hyperlink[] getHyperlinks()
```


Obtient tous les hyperliens dans la plage.

**Returns:**
com.aspose.cells.Hyperlink[]
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
### getRangeCount() {#getRangeCount--}
```
public int getRangeCount()
```


Obtient le nombre de plages.

**Returns:**
int
### getRanges() {#getRanges--}
```
public Range[] getRanges()
```


Obtient toutes les plages d'union.

**Returns:**
com.aspose.cells.Range[]
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

**Remarks**

N'affecte que lorsqu'il ne contient qu'une seule plage.

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Obtient les valeurs de la plage.

**Returns:**
java.lang.Object
### hasRange() {#hasRange--}
```
public boolean hasRange()
```


Indique si cela possède une plage.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### intersect(Range[] ranges) {#intersect-com.aspose.cells.Range---}
```
public UnionRange intersect(Range[] ranges)
```


Intersecte une autre plage.

**Remarks**

Si les deux plages d'union ne sont pas intersectées, renvoie null.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ranges | [Range\[\]](../../com.aspose.cells/range) | La plage. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange)
### intersect(UnionRange unionRange) {#intersect-com.aspose.cells.UnionRange-}
```
public UnionRange intersect(UnionRange unionRange)
```


Intersecte une autre plage.

**Remarks**

Si les deux plages d'union ne sont pas intersectées, renvoie null.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| unionRange | [UnionRange](../../com.aspose.cells/unionrange) | La plage. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange)
### intersect(String range) {#intersect-java.lang.String-}
```
public UnionRange intersect(String range)
```


Intersecte une autre plage.

**Remarks**

Si les deux plages d'union ne sont pas intersectées, renvoie null.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| plage | java.lang.String | La plage. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange)
### iterator() {#iterator--}
```
public Iterator iterator()
```


Obtient l'énumérateur des cellules de cette Range.

**Remarks**

Lors du parcours des éléments à l'aide de l'énumérateur retourné, la collection de cellules ne doit pas être modifiée (par exemple des opérations qui créeraient de nouvelles Cell/Row ou supprimeraient des Cell/Row existantes). Sinon, l'énumérateur pourrait ne pas être capable de parcourir correctement toutes les cellules (certains éléments pourraient être parcourus plusieurs fois ou être ignorés).

**Returns:**
java.util.Iterator - L'énumérateur de cellules
### merge() {#merge--}
```
public void merge()
```


Combine une plage de cellules en une seule cellule.

**Remarks**

Référez la cellule fusionnée via l'adresse de la cellule en haut à gauche de la plage.

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

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


Définit le style de la plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | L'objet Style. |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Définit les valeurs de la plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.Object |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unMerge() {#unMerge--}
```
public void unMerge()
```


Démarque les cellules fusionnées de cette plage.

### union(Range[] ranges) {#union-com.aspose.cells.Range---}
```
public UnionRange union(Range[] ranges)
```


Union des plages.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ranges | [Range\[\]](../../com.aspose.cells/range) | Les plages. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - 
### union(UnionRange unionRange) {#union-com.aspose.cells.UnionRange-}
```
public UnionRange union(UnionRange unionRange)
```


Union d'une autre plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| unionRange | [UnionRange](../../com.aspose.cells/unionrange) | La plage. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - 
### union(String range) {#union-java.lang.String-}
```
public UnionRange union(String range)
```


Union d'une autre plage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| plage | java.lang.String | La plage. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - 
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

