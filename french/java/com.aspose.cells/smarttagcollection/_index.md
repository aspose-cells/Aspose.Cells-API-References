---
title: "SmartTagCollection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente toutes les balises intelligentes dans la cellule."
type: docs
url: /fr/java/com.aspose.cells/smarttagcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class SmartTagCollection extends CollectionBase
```

Représente toutes les balises intelligentes dans la cellule.
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Ajoute un élément à l'instance CollectionBase. |
| [add(String uri, String name)](#add-java.lang.String-java.lang.String-) | Ajoute une balise intelligente. |
| [clear()](#clear--) | Supprime tous les objets de l'instance CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Renvoie si l'instance contient cet objet |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtient un objet [SmartTag](../../com.aspose.cells/smarttag) à l'index spécifié |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Obtient la colonne des smart tags de la cellule. |
| [getCount()](#getCount--) | Obtient le nombre d'éléments contenus dans l'instance CollectionBase. |
| [getRow()](#getRow--) | Obtient la ligne des smart tags de la cellule. |
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
### add(String uri, String name) {#add-java.lang.String-java.lang.String-}
```
public int add(String uri, String name)
```


Ajoute une balise intelligente.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| uri | java.lang.String | Spécifie l'URI de l'espace de noms du smart tag |
| name | java.lang.String | Spécifie le nom du smart tag. |

**Returns:**
int - L'index du smart tag dans la liste.
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
public SmartTag get(int index)
```


Obtient un objet [SmartTag](../../com.aspose.cells/smarttag) à l'index spécifié

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index. |

**Returns:**
[SmartTag](../../com.aspose.cells/smarttag) - returns a [SmartTag](../../com.aspose.cells/smarttag) object.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumn() {#getColumn--}
```
public int getColumn()
```


Obtient la colonne des smart tags de la cellule.

**Returns:**
int
### getCount() {#getCount--}
```
public int getCount()
```


Obtient le nombre d'éléments contenus dans l'instance CollectionBase.

**Returns:**
int - Le nombre d'éléments contenus dans l'instance CollectionBase.
### getRow() {#getRow--}
```
public int getRow()
```


Obtient la ligne des smart tags de la cellule.

**Returns:**
int
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

