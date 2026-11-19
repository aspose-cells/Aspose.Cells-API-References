---
title: "HorizontalPageBreakCollection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Encapsule une collection d'objets."
type: docs
url: /fr/java/com.aspose.cells/horizontalpagebreakcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class HorizontalPageBreakCollection extends CollectionBase
```

Encapsule une collection d'objets [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak).

**Example**

```
         Workbook excel = new Workbook();
 
         //Add a pagebreak at G5
         excel.getWorksheets().get(0).getHorizontalPageBreaks().add("G5");
         excel.getWorksheets().get(0).getVerticalPageBreaks().add("G5");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(int row)](#add-int-) | Ajoute un saut de page horizontal à la collection. |
| [add(int row, int column)](#add-int-int-) | Ajoute un saut de page horizontal à la collection. |
| [add(int row, int startColumn, int endColumn)](#add-int-int-int-) | Ajoute un saut de page horizontal à la collection. |
| [add(Object o)](#add-java.lang.Object-) | Ajoute un élément à l'instance CollectionBase. |
| [add(String cellName)](#add-java.lang.String-) | Ajoute un saut de page horizontal à la collection. |
| [clear()](#clear--) | Supprime tous les objets de l'instance CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Renvoie si l'instance contient cet objet |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtient l'élément [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) à l'index spécifié. |
| [get(String cellName)](#get-java.lang.String-) | Obtient l'élément [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) avec le nom de cellule spécifié. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtient le nombre d'éléments contenus dans l'instance CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Détermine l'index d'un élément spécifique dans l'instance CollectionBase. |
| [iterator()](#iterator--) | Renvoie un énumérateur qui parcourt l'instance CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Supprime l'élément HPageBreak à un nom spécifié. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int row) {#add-int-}
```
public int add(int row)
```


Ajoute un saut de page horizontal à la collection.

**Remarks**

Le saut de page est ajouté en haut à gauche de la cellule. Veuillez définir simultanément un saut de page horizontal et un saut de page vertical.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | Indice de ligne de cellule, basé sur zéro. |

**Returns:**
int - index de l'objet [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak).
### add(int row, int column) {#add-int-int-}
```
public int add(int row, int column)
```


Ajoute un saut de page horizontal à la collection.

**Remarks**

Le saut de page est ajouté en haut à gauche de la cellule. Veuillez définir simultanément un saut de page horizontal et un saut de page vertical.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | Indice de ligne de cellule, basé sur zéro. |
| colonne | int | Indice de colonne de cellule, basé sur zéro. |

**Returns:**
int - index de l'objet [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak).
### add(int row, int startColumn, int endColumn) {#add-int-int-int-}
```
public int add(int row, int startColumn, int endColumn)
```


Ajoute un saut de page horizontal à la collection.

**Remarks**

Cette méthode est utilisée pour ajouter un saut de page horizontal dans une zone d'impression.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | int | Indice de ligne, basé à zéro. |
| startColumn | int | Indice de colonne de départ, basé à zéro. |
| endColumn | int | Indice de colonne de fin, basé à zéro. |

**Returns:**
int - index de l'objet [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak).
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


Ajoute un saut de page horizontal à la collection.

**Remarks**

Le saut de page est ajouté en haut à gauche de la cellule. Veuillez définir simultanément un saut de page horizontal et un saut de page vertical.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cellName | java.lang.String | Nom de cellule. |

**Returns:**
int - index de l'objet [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak).
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
public HorizontalPageBreak get(int index)
```


Obtient l'élément [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) à l'index spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index de base zéro de l'élément. |

**Returns:**
[HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) - The element at the specified index.
### get(String cellName) {#get-java.lang.String-}
```
public HorizontalPageBreak get(String cellName)
```


Obtient l'élément [HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) avec le nom de cellule spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cellName | java.lang.String | Nom de cellule. |

**Returns:**
[HorizontalPageBreak](../../com.aspose.cells/horizontalpagebreak) - The element with the specified cell name.
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


Supprime l'élément HPageBreak à un nom spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | Indice d'élément, basé sur zéro. |

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

