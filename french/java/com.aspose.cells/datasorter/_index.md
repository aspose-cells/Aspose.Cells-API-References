---
title: "DataSorter"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Description résumée pour DataSorter."
type: docs
url: /fr/java/com.aspose.cells/datasorter/
---

**Inheritance:**
java.lang.Object
```
public class DataSorter
```

Description résumée pour DataSorter.

**Example**

```
         //Instantiate a new Workbook object.
         Workbook workbook = new Workbook("Book1.xls");
         //Get the workbook datasorter object.
         DataSorter sorter = workbook.getDataSorter();
         //Set the first order for datasorter object.
         sorter.setOrder1(com.aspose.cells.SortOrder.DESCENDING);
         //Define the first key.
         sorter.setKey1(0);
         //Set the second order for datasorter object.
         sorter.setOrder2(com.aspose.cells.SortOrder.ASCENDING);
         //Define the second key.
         sorter.setKey2(1);
         //Create a cells area (range).
         CellArea ca = new CellArea();
         //Specify the start row index.
         ca.StartRow = 0;
         //Specify the start column index.
         ca.StartColumn = 0;
         //Specify the last row index.
         ca.EndRow = 13;
         //Specify the last column index.
         ca.EndColumn = 1;
         //Sort data in the specified data range (A1:B14)
         sorter.sort(workbook.getWorksheets().get(0).getCells(), ca);
         //Save the excel file.
         workbook.save("outBook.xls");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [addColorKey(int key, int type, int order, Color color)](#addColorKey-int-int-int-com.aspose.cells.Color-) | Ajoute une clé de tri couleur. |
| [addKey(int key, int order)](#addKey-int-int-) | Ajoute l'index de colonne triée et l'ordre de tri. |
| [addKey(int key, int type, int order, Object customList)](#addKey-int-int-int-java.lang.Object-) | Ajoute l'index de colonne triée et l'ordre de tri avec une liste de tri personnalisée. |
| [addKey(int key, int order, String customList)](#addKey-int-int-java.lang.String-) | Ajoute l'index de colonne triée et l'ordre de tri avec une liste de tri personnalisée. |
| [addKey(int key, int order, String[] customList)](#addKey-int-int-java.lang.String---) | Ajoute l'index de colonne triée et l'ordre de tri avec une liste de tri personnalisée. |
| [clear()](#clear--) | Efface tous les paramètres. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCaseSensitive()](#getCaseSensitive--) | Obtient si la comparaison de chaîne est sensible à la casse. |
| [getClass()](#getClass--) |  |
| [getKey1()](#getKey1--) | Représente l'index de la première colonne triée (position absolue, la colonne A est 0, B est 1, ...). |
| [getKey2()](#getKey2--) | Représente l'index de la deuxième colonne triée (position absolue, la colonne A est 0, B est 1, ...). |
| [getKey3()](#getKey3--) | Représente l'index de la troisième colonne triée (position absolue, la colonne A est 0, B est 1, ...). |
| [getKeys()](#getKeys--) | Obtient la liste des clés du trieur de données. |
| [getOrder1()](#getOrder1--) | Représente l'ordre de tri de la première clé. |
| [getOrder2()](#getOrder2--) | Représente l'ordre de tri de la deuxième clé. |
| [getOrder3()](#getOrder3--) | Représente l'ordre de tri de la troisième clé. |
| [getSortAsNumber()](#getSortAsNumber--) | Indique si le tri concerne tout ce qui ressemble à un nombre. |
| [getSortLeftToRight()](#getSortLeftToRight--) | Vrai signifie que l'orientation du tri est de gauche à droite. |
| [hasHeaders()](#hasHeaders--) | Représente si la plage possède des en-têtes. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCaseSensitive(boolean value)](#setCaseSensitive-boolean-) | Définit si la comparaison de chaîne est sensible à la casse. |
| [setHasHeaders(boolean value)](#setHasHeaders-boolean-) | Représente si la plage possède des en-têtes. |
| [setKey1(int value)](#setKey1-int-) | Représente l'index de la première colonne triée (position absolue, la colonne A est 0, B est 1, ...). |
| [setKey2(int value)](#setKey2-int-) | Représente l'index de la deuxième colonne triée (position absolue, la colonne A est 0, B est 1, ...). |
| [setKey3(int value)](#setKey3-int-) | Représente l'index de la troisième colonne triée (position absolue, la colonne A est 0, B est 1, ...). |
| [setOrder1(int value)](#setOrder1-int-) | Représente l'ordre de tri de la première clé. |
| [setOrder2(int value)](#setOrder2-int-) | Représente l'ordre de tri de la deuxième clé. |
| [setOrder3(int value)](#setOrder3-int-) | Représente l'ordre de tri de la troisième clé. |
| [setSortAsNumber(boolean value)](#setSortAsNumber-boolean-) | Indique si le tri concerne tout ce qui ressemble à un nombre. |
| [setSortLeftToRight(boolean value)](#setSortLeftToRight-boolean-) | Vrai signifie que l'orientation du tri est de gauche à droite. |
| [sort()](#sort--) | Trie les données dans la plage. |
| [sort(Cells cells, CellArea area)](#sort-com.aspose.cells.Cells-com.aspose.cells.CellArea-) | Trier les données de la zone. |
| [sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn)](#sort-com.aspose.cells.Cells-int-int-int-int-) | Trie les données de la zone. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addColorKey(int key, int type, int order, Color color) {#addColorKey-int-int-int-com.aspose.cells.Color-}
```
public void addColorKey(int key, int type, int order, Color color)
```


Ajoute une clé de tri couleur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| clé | int | L'index de la colonne triée (position absolue, la colonne A est 0, B est 1, ...) |
| type | int | [SortOnType](../../com.aspose.cells/sortontype). Le type de valeur de couleur triée. |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). L'ordre de tri. |
| color | [Color](../../com.aspose.cells/color) | La couleur de tri personnalisée. |

### addKey(int key, int order) {#addKey-int-int-}
```
public void addKey(int key, int order)
```


Ajoute l'index de colonne triée et l'ordre de tri.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| clé | int | L'index de la colonne triée (position absolue, la colonne A est 0, B est 1, ...) |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). L'ordre de tri |

### addKey(int key, int type, int order, Object customList) {#addKey-int-int-int-java.lang.Object-}
```
public void addKey(int key, int type, int order, Object customList)
```


Ajoute l'index de colonne triée et l'ordre de tri avec une liste de tri personnalisée.

**Remarks**

Si le type est SortOnType.CellColor ou SortOnType.FontColor, le customList est Color.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| clé | int | L'index de la colonne triée (position absolue, la colonne A est 0, B est 1, ...) |
| type | int | [SortOnType](../../com.aspose.cells/sortontype). Le type de valeur triée. |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). L'ordre de tri. |
| customList | java.lang.Object | La liste de tri personnalisée. |

### addKey(int key, int order, String customList) {#addKey-int-int-java.lang.String-}
```
public void addKey(int key, int order, String customList)
```


Ajoute l'index de colonne triée et l'ordre de tri avec une liste de tri personnalisée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| clé | int | L'index de la colonne triée (position absolue, la colonne A est 0, B est 1, ...) |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). L'ordre de tri. |
| customList | java.lang.String | La liste de tri personnalisée. |

### addKey(int key, int order, String[] customList) {#addKey-int-int-java.lang.String---}
```
public void addKey(int key, int order, String[] customList)
```


Ajoute l'index de colonne triée et l'ordre de tri avec une liste de tri personnalisée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| clé | int | L'index de la colonne triée (position absolue, la colonne A est 0, B est 1, ...) |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). L'ordre de tri. |
| customList | java.lang.String[] | La liste de tri personnalisée. |

### clear() {#clear--}
```
public void clear()
```


Efface tous les paramètres.

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
### getCaseSensitive() {#getCaseSensitive--}
```
public boolean getCaseSensitive()
```


Obtient si la comparaison de chaîne est sensible à la casse.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getKey1() {#getKey1--}
```
public int getKey1()
```


Représente l'index de la première colonne triée (position absolue, la colonne A est 0, B est 1, ...).

**Returns:**
int
### getKey2() {#getKey2--}
```
public int getKey2()
```


Représente l'index de la deuxième colonne triée (position absolue, la colonne A est 0, B est 1, ...).

**Returns:**
int
### getKey3() {#getKey3--}
```
public int getKey3()
```


Représente l'index de la troisième colonne triée (position absolue, la colonne A est 0, B est 1, ...).

**Returns:**
int
### getKeys() {#getKeys--}
```
public DataSorterKeyCollection getKeys()
```


Obtient la liste des clés du trieur de données.

**Returns:**
[DataSorterKeyCollection](../../com.aspose.cells/datasorterkeycollection)
### getOrder1() {#getOrder1--}
```
public int getOrder1()
```


Représente l'ordre de tri de la première clé.

Voir le [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### getOrder2() {#getOrder2--}
```
public int getOrder2()
```


Représente l'ordre de tri de la deuxième clé.

Voir le [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### getOrder3() {#getOrder3--}
```
public int getOrder3()
```


Représente l'ordre de tri de la troisième clé.

Voir le [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### getSortAsNumber() {#getSortAsNumber--}
```
public boolean getSortAsNumber()
```


Indique si le tri concerne tout ce qui ressemble à un nombre.

**Returns:**
boolean
### getSortLeftToRight() {#getSortLeftToRight--}
```
public boolean getSortLeftToRight()
```


True signifie que l'orientation du tri est de gauche à droite. False signifie que l'orientation du tri est de haut en bas. La valeur par défaut est false.

**Returns:**
boolean
### hasHeaders() {#hasHeaders--}
```
public boolean hasHeaders()
```


Représente si la plage possède des en-têtes.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setCaseSensitive(boolean value) {#setCaseSensitive-boolean-}
```
public void setCaseSensitive(boolean value)
```


Définit si la comparaison de chaîne est sensible à la casse.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHasHeaders(boolean value) {#setHasHeaders-boolean-}
```
public void setHasHeaders(boolean value)
```


Représente si la plage possède des en-têtes.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setKey1(int value) {#setKey1-int-}
```
public void setKey1(int value)
```


Représente l'index de la première colonne triée (position absolue, la colonne A est 0, B est 1, ...).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setKey2(int value) {#setKey2-int-}
```
public void setKey2(int value)
```


Représente l'index de la deuxième colonne triée (position absolue, la colonne A est 0, B est 1, ...).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setKey3(int value) {#setKey3-int-}
```
public void setKey3(int value)
```


Représente l'index de la troisième colonne triée (position absolue, la colonne A est 0, B est 1, ...).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setOrder1(int value) {#setOrder1-int-}
```
public void setOrder1(int value)
```


Représente l'ordre de tri de la première clé.

Voir le [SortOrder](../../com.aspose.cells/sortorder).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setOrder2(int value) {#setOrder2-int-}
```
public void setOrder2(int value)
```


Représente l'ordre de tri de la deuxième clé.

Voir le [SortOrder](../../com.aspose.cells/sortorder).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setOrder3(int value) {#setOrder3-int-}
```
public void setOrder3(int value)
```


Représente l'ordre de tri de la troisième clé.

Voir le [SortOrder](../../com.aspose.cells/sortorder).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setSortAsNumber(boolean value) {#setSortAsNumber-boolean-}
```
public void setSortAsNumber(boolean value)
```


Indique si le tri concerne tout ce qui ressemble à un nombre.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSortLeftToRight(boolean value) {#setSortLeftToRight-boolean-}
```
public void setSortLeftToRight(boolean value)
```


True signifie que l'orientation du tri est de gauche à droite. False signifie que l'orientation du tri est de haut en bas. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### sort() {#sort--}
```
public int[] sort()
```


Trie les données dans la plage.

**Returns:**
int[] - les indices originaux (position absolue, par exemple, la colonne A est 0, B est 1, ...) des lignes/colonnes triées. Si aucune ligne/colonne n'a besoin d'être déplacée par cette opération de tri, null sera retourné.
### sort(Cells cells, CellArea area) {#sort-com.aspose.cells.Cells-com.aspose.cells.CellArea-}
```
public int[] sort(Cells cells, CellArea area)
```


Trier les données de la zone.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cells | [Cells](../../com.aspose.cells/cells) | Les cellules contiennent la zone de données. |
| area | [CellArea](../../com.aspose.cells/cellarea) | La zone à trier |

**Returns:**
int[] - les indices originaux (position absolue, par exemple, la colonne A est 0, B est 1, ...) des lignes/colonnes triées. Si aucune ligne/colonne n'a besoin d'être déplacée par cette opération de tri, null sera retourné.
### sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn) {#sort-com.aspose.cells.Cells-int-int-int-int-}
```
public int[] sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn)
```


Trie les données de la zone.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cells | [Cells](../../com.aspose.cells/cells) | Les cellules contiennent la zone de données. |
| startRow | int | La ligne de départ de la zone. |
| startColumn | int | La colonne de départ de la zone. |
| endRow | int | La ligne de fin de la zone. |
| endColumn | int | La colonne de fin de la zone. |

**Returns:**
int[] - les indices originaux (position absolue, par exemple, la colonne A est 0, B est 1, ...) des lignes/colonnes triées. Si aucune ligne/colonne n'a besoin d'être déplacée par cette opération de tri, null sera retourné.
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

