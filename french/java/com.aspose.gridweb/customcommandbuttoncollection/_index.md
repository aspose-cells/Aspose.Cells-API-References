---
title: "CustomCommandButtonCollection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente la collection de CustomCommandButton."
type: docs
url: /fr/java/com.aspose.gridweb/customcommandbuttoncollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.CollectionBase](../../com.aspose.gridweb/collectionbase)
```
public class CustomCommandButtonCollection extends CollectionBase
```

Représente la collection de CustomCommandButton.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         CustomCommandButton button = new CustomCommandButton();
         button.setCommand("MyCommand");
         button.setImageUrl("images/button1.gif");
         GridWeb1.getCustomCommandButtons().add(button);
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(Object value)](#add-java.lang.Object-) | Ajoutez un objet bouton de commande personnalisé à la collection. |
| [clear()](#clear--) | Efface la collection. |
| [contains(Object value)](#contains-java.lang.Object-) | Indique si l'objet bouton de commande personnalisé se trouve dans la collection. |
| [copyTo(Object[] array, int index)](#copyTo-java.lang.Object---int-) | Copie la collection dans un tableau. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtient un objet bouton de commande personnalisé à l'index. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtient le nombre d'éléments de la collection. |
| [getSyncRoot()](#getSyncRoot--) | Utilisé uniquement en interne. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object value)](#indexOf-java.lang.Object-) | Obtient l'index du bouton. |
| [insert(int index, Object value)](#insert-int-java.lang.Object-) | Insère un bouton à l'index. |
| [isFixedSize()](#isFixedSize--) | Utilisé uniquement en interne. |
| [isReadOnly()](#isReadOnly--) | Utilisé uniquement en interne. |
| [isSynchronized()](#isSynchronized--) | Utilisé uniquement en interne. |
| [iterator()](#iterator--) | Obtient un objet IEnumerator de la collection. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Object value)](#remove-java.lang.Object-) | Supprime l'objet bouton de commande personnalisé. |
| [removeAt(int index)](#removeAt-int-) | Supprime à l'index. |
| [set(int index, CustomCommandButton value)](#set-int-com.aspose.gridweb.CustomCommandButton-) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Object value) {#add-java.lang.Object-}
```
public int add(Object value)
```


Ajoutez un objet bouton de commande personnalisé à la collection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.Object | L'objet bouton de commande personnalisé. |

**Returns:**
int - L'index.
### clear() {#clear--}
```
public void clear()
```


Efface la collection.

### contains(Object value) {#contains-java.lang.Object-}
```
public boolean contains(Object value)
```


Indique si l'objet bouton de commande personnalisé se trouve dans la collection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.Object | Indique si l'objet bouton de commande personnalisé se trouve dans la collection. |

**Returns:**
boolean - vrai ou faux.
### copyTo(Object[] array, int index) {#copyTo-java.lang.Object---int-}
```
public void copyTo(Object[] array, int index)
```


Copie la collection dans un tableau.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| tableau | java.lang.Object[] | Le tableau. |
| index | int | L'index de départ du tableau. |

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
public CustomCommandButton get(int index)
```


Obtient un objet bouton de commande personnalisé à l'index.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int |  |

**Returns:**
[CustomCommandButton](../../com.aspose.gridweb/customcommandbutton)
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


Obtient le nombre d'éléments de la collection.

**Returns:**
int
### getSyncRoot() {#getSyncRoot--}
```
public Object getSyncRoot()
```


Utilisé uniquement en interne.

**Returns:**
java.lang.Object
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object value) {#indexOf-java.lang.Object-}
```
public int indexOf(Object value)
```


Obtient l'index du bouton.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.Object | L'objet bouton. |

**Returns:**
int - L'index.
### insert(int index, Object value) {#insert-int-java.lang.Object-}
```
public void insert(int index, Object value)
```


Insère un bouton à l'index.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | Index. |
| valeur | java.lang.Object | L'objet CustomCommandButton. |

### isFixedSize() {#isFixedSize--}
```
public boolean isFixedSize()
```


Utilisé uniquement en interne.

**Returns:**
boolean
### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


Utilisé uniquement en interne.

**Returns:**
boolean
### isSynchronized() {#isSynchronized--}
```
public boolean isSynchronized()
```


Utilisé uniquement en interne.

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


Obtient un objet IEnumerator de la collection.

**Returns:**
java.util.Iterator - L'objet IEnumerator.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### remove(Object value) {#remove-java.lang.Object-}
```
public void remove(Object value)
```


Supprime l'objet bouton de commande personnalisé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.Object | L'objet bouton de commande personnalisé. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Supprime à l'index.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | Index. |

### set(int index, CustomCommandButton value) {#set-int-com.aspose.gridweb.CustomCommandButton-}
```
public void set(int index, CustomCommandButton value)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int |  |
| value | [CustomCommandButton](../../com.aspose.gridweb/customcommandbutton) |  |

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

