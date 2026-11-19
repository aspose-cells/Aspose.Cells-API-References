---
title: "RowCollection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Collecte les objets qui représentent les lignes individuelles d’une feuille de calcul."
type: docs
url: /fr/java/com.aspose.cells/rowcollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class RowCollection implements Iterable
```

Collecte les [Row](../../com.aspose.cells/row) qui représentent les lignes individuelles d’une feuille de calcul.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
          //Get first row
         Row row = worksheet.getCells().getRows().get(0);
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [clear()](#clear--) | Efface toutes les lignes et cellules. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int rowIndex)](#get-int-) | Obtient un objet [Row](../../com.aspose.cells/row) par l’indice de ligne donné. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtient le nombre de lignes dans cette collection. |
| [getRowByIndex(int index)](#getRowByIndex-int-) | Obtient l’objet de ligne par la position dans la liste. |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Obtient un énumérateur qui parcourt les lignes de cette collection |
| [iterator(boolean reversed, boolean sync)](#iterator-boolean-boolean-) | Obtient un énumérateur qui parcourt les lignes de cette collection |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Supprime l’élément de ligne à l’indice (position) spécifié dans cette collection. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### clear() {#clear--}
```
public void clear()
```


Efface toutes les lignes et cellules.

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
### get(int rowIndex) {#get-int-}
```
public Row get(int rowIndex)
```


Obtient un objet [Row](../../com.aspose.cells/row) par l’indice de ligne donné. L’objet Row de l’indice de ligne donné sera instancié s’il n’existe pas auparavant.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | int |  |

**Returns:**
[Row](../../com.aspose.cells/row)
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


Obtient le nombre de lignes dans cette collection.

**Returns:**
int
### getRowByIndex(int index) {#getRowByIndex-int-}
```
public Row getRowByIndex(int index)
```


Obtient l’objet de ligne par la position dans la liste.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | La position. |

**Returns:**
[Row](../../com.aspose.cells/row) - The Row object at given position.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### iterator() {#iterator--}
```
public Iterator iterator()
```


Obtient un énumérateur qui parcourt les lignes de cette collection

**Example**

```
         Workbook workbook = new Workbook("template.xlsx");
         	Cells cells = workbook.getWorksheets().get(0).getCells();
 
         	Iterator en = cells.getRows().iterator();
         	while (en.hasNext())
         	{
         	    Row row = (Row)en.next();
         	    System.out.println(row.getIndex() + ": " + row.getHeight());
         	}
```

**Returns:**
java.util.Iterator - L'énumérateur de lignes qui parcourra toutes les lignes existantes dans cette collection.
### iterator(boolean reversed, boolean sync) {#iterator-boolean-boolean-}
```
public Iterator iterator(boolean reversed, boolean sync)
```


Obtient un énumérateur qui parcourt les lignes de cette collection

**Remarks**

Si la collection de lignes est modifiée (par des opérations pouvant entraîner la création d'une nouvelle Row ou la suppression d'une Row existante) pendant le parcours avec l'énumérateur, un énumérateur synchronisé doit être utilisé à la place d'un énumérateur normal afin que le parcours puisse continuer à partir de la position immédiatement après celle qui a été parcourue par le dernier MoveNext(). Cependant, en plus de l'avantage qu'aucun élément ne soit sauté ou parcouru plusieurs fois, l'inconvénient de l'énumérateur synchronisé est que les performances seront légèrement dégradées par rapport à un énumérateur normal.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| inversé | boolean | si les lignes sont énumérées dans l'ordre inversé |
| synchroniser | boolean | si l'énumérateur retourné doit vérifier la modification de la collection de lignes et rester synchronisé avec celle-ci. |

**Returns:**
java.util.Iterator - L'énumérateur de lignes qui parcourra toutes les lignes existantes dans cette collection.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Supprime l’élément de ligne à l’indice (position) spécifié dans cette collection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | indice basé sur zéro (position, pas [Row.getIndex()](../../com.aspose.cells/row\#getIndex--)) de l'élément de ligne existant dans cette collection. |

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

