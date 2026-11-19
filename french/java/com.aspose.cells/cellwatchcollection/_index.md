---
title: "CellWatchCollection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente la collection de cellules de cette feuille de calcul surveillées dans la fenêtre de surveillance."
type: docs
url: /fr/java/com.aspose.cells/cellwatchcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class CellWatchCollection extends CollectionBase
```

Représente la collection de cellules de cette feuille de calcul surveillées dans la « watch window ».

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         // Get the first Worksheet.
         Worksheet sheet = workbook.getWorksheets().get(0);
         // Add Cell Watch Item into the watch window
         sheet.getCellWatches().add("B2");
```
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [CellWatchCollection()](#CellWatchCollection--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(int row, int column)](#add-int-int-) | Ajoute [CellWatch](../../com.aspose.cells/cellwatch) avec une ligne et une colonne. |
| [add(Object o)](#add-java.lang.Object-) | Ajoute un élément à l'instance CollectionBase. |
| [add(String cellName)](#add-java.lang.String-) | Ajoute [CellWatch](../../com.aspose.cells/cellwatch) avec le nom de la cellule. |
| [clear()](#clear--) | Supprime tous les objets de l'instance CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Renvoie si l'instance contient cet objet |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtient et définit [CellWatch](../../com.aspose.cells/cellwatch) par indice. |
| [get(String cellName)](#get-java.lang.String-) | Obtient et définit [CellWatch](../../com.aspose.cells/cellwatch) par le nom de la cellule. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtient le nombre d'éléments contenus dans l'instance CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Détermine l'index d'un élément spécifique dans l'instance CollectionBase. |
| [iterator()](#iterator--) | Renvoie un énumérateur qui parcourt l'instance CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Supprime l'élément à l'index spécifié. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CellWatchCollection() {#CellWatchCollection--}
```
public CellWatchCollection()
```


### add(int row, int column) {#add-int-int-}
```
public int add(int row, int column)
```


Ajoute [CellWatch](../../com.aspose.cells/cellwatch) avec une ligne et une colonne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | L'index de ligne. |
| colonne | int | L'index de colonne. |

**Returns:**
int - Retourne la position de cet élément dans la collection.
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
### add(String cellName) {#add-java.lang.String-}
```
public int add(String cellName)
```


Ajoute [CellWatch](../../com.aspose.cells/cellwatch) avec le nom de la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cellName | java.lang.String | Le nom de la cellule. |

**Returns:**
int -
### clear() {#clear--}
```
public void clear()
```


Supprime tous les objets de l'instance CollectionBase.

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
### get(int index) {#get-int-}
```
public CellWatch get(int index)
```


Obtient et définit [CellWatch](../../com.aspose.cells/cellwatch) par indice.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index. |

**Returns:**
[CellWatch](../../com.aspose.cells/cellwatch) - 
### get(String cellName) {#get-java.lang.String-}
```
public CellWatch get(String cellName)
```


Obtient et définit [CellWatch](../../com.aspose.cells/cellwatch) par le nom de la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cellName | java.lang.String | Le nom de la cellule. |

**Returns:**
[CellWatch](../../com.aspose.cells/cellwatch) - 
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




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Supprime l'élément à l'index spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index basé sur zéro de l'élément à supprimer. |

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

