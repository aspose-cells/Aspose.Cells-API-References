---
title: "GridNameCollection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Encapsule une collection d'objets."
type: docs
url: /fr/java/com.aspose.gridweb/gridnamecollection/
---

**Inheritance:**
java.lang.Object
```
public class GridNameCollection
```

Encapsule une collection d'objets [GridName](../../com.aspose.gridweb/gridname).
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(int sheetIndex, String text, String refersTo)](#add-int-java.lang.String-java.lang.String-) | Définit un nouveau nom dans la feuille spécifiée. |
| [add(String text, String refersTo)](#add-java.lang.String-java.lang.String-) | Définit un nouveau nom global. |
| [clear()](#clear--) | Supprime tous les noms ; |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtient l'élément [GridName](../../com.aspose.gridweb/gridname) à l'index spécifié. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtient la taille de l'énumérateur |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Obtient l'énumérateur des lignes |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String[] names)](#remove-java.lang.String---) | Supprime un tableau de noms. |
| [removeAt(int index)](#removeAt-int-) | Supprime le nom à l'index spécifié. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int sheetIndex, String text, String refersTo) {#add-int-java.lang.String-java.lang.String-}
```
public int add(int sheetIndex, String text, String refersTo)
```


Définit un nouveau nom dans la feuille spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sheetIndex | int | L'index de feuille dans lequel le nom est appliqué. |
| texte | java.lang.String | Texte du nom. Il ne peut pas contenir de nom de feuille. |
| refersTo | java.lang.String | La formule à laquelle le nom est défini pour faire référence. Elle doit contenir un nom de feuille, par ex. 'sheet hello!'A1:B2. |

**Returns:**
int - index de l'objet Name.
### add(String text, String refersTo) {#add-java.lang.String-java.lang.String-}
```
public int add(String text, String refersTo)
```


Définit un nouveau nom global.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| texte | java.lang.String | Texte du nom. Il peut contenir un nom de feuille. |
| refersTo | java.lang.String | La formule à laquelle le nom est défini pour faire référence. Elle doit contenir un nom de feuille, par ex. 'sheet hello!'A1:B2. |

**Returns:**
int - index de l'objet Name.
### clear() {#clear--}
```
public void clear()
```


Supprime tous les noms ;

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
public GridName get(int index)
```


Obtient l'élément [GridName](../../com.aspose.gridweb/gridname) à l'index spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index de base zéro de l'élément. |

**Returns:**
[GridName](../../com.aspose.gridweb/gridname) - The element at the specified index.
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


Obtient la taille de l'énumérateur

**Returns:**
int
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


Obtient l'énumérateur des lignes

**Returns:**
java.util.Iterator - L'énumérateur des lignes
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### remove(String[] names) {#remove-java.lang.String---}
```
public void remove(String[] names)
```


Supprime un tableau de noms.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| noms | java.lang.String[] | Le texte des noms. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Supprime le nom à l'index spécifié.

**Remarks**

Veuillez vous assurer que le nom n'est pas référencé par d'autres formules avant d'appeler la méthode. Et si le nom est référencé, veuillez uniquement définir Name.RefersTo à null.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int |  |

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

