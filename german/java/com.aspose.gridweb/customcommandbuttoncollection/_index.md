---
title: "CustomCommandButtonCollection"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Sammlung von CustomCommandButton dar."
type: docs
url: /de/java/com.aspose.gridweb/customcommandbuttoncollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.CollectionBase](../../com.aspose.gridweb/collectionbase)
```
public class CustomCommandButtonCollection extends CollectionBase
```

Stellt die Sammlung von CustomCommandButton dar.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         CustomCommandButton button = new CustomCommandButton();
         button.setCommand("MyCommand");
         button.setImageUrl("images/button1.gif");
         GridWeb1.getCustomCommandButtons().add(button);
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(Object value)](#add-java.lang.Object-) | Fügt ein benutzerdefiniertes CommandButton-Objekt zur Sammlung hinzu. |
| [clear()](#clear--) | Leert die Sammlung. |
| [contains(Object value)](#contains-java.lang.Object-) | Gibt an, ob das benutzerdefinierte CommandButton-Objekt in der Sammlung ist. |
| [copyTo(Object[] array, int index)](#copyTo-java.lang.Object---int-) | Kopiert die Sammlung in ein Array. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Ruft ein benutzerdefiniertes CommandButton-Objekt am Index ab. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ruft die Anzahl der Sammlung ab. |
| [getSyncRoot()](#getSyncRoot--) | Nur intern verwendet. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object value)](#indexOf-java.lang.Object-) | Ruft den Index der Schaltfläche ab. |
| [insert(int index, Object value)](#insert-int-java.lang.Object-) | Fügt eine Schaltfläche am Index ein. |
| [isFixedSize()](#isFixedSize--) | Nur intern verwendet. |
| [isReadOnly()](#isReadOnly--) | Nur intern verwendet. |
| [isSynchronized()](#isSynchronized--) | Nur intern verwendet. |
| [iterator()](#iterator--) | Gibt ein IEnumerator-Objekt der Sammlung zurück. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Object value)](#remove-java.lang.Object-) | Entfernt das benutzerdefinierte Befehls-Schaltflächenobjekt. |
| [removeAt(int index)](#removeAt-int-) | Entfernt am Index. |
| [set(int index, CustomCommandButton value)](#set-int-com.aspose.gridweb.CustomCommandButton-) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Object value) {#add-java.lang.Object-}
```
public int add(Object value)
```


Fügt ein benutzerdefiniertes CommandButton-Objekt zur Sammlung hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.Object | Das benutzerdefinierte Befehls-Schaltflächenobjekt. |

**Returns:**
int - Der Index.
### clear() {#clear--}
```
public void clear()
```


Leert die Sammlung.

### contains(Object value) {#contains-java.lang.Object-}
```
public boolean contains(Object value)
```


Gibt an, ob das benutzerdefinierte CommandButton-Objekt in der Sammlung ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.Object | Gibt an, ob das benutzerdefinierte CommandButton-Objekt in der Sammlung ist. |

**Returns:**
boolean – true oder false.
### copyTo(Object[] array, int index) {#copyTo-java.lang.Object---int-}
```
public void copyTo(Object[] array, int index)
```


Kopiert die Sammlung in ein Array.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Array | java.lang.Object[] | Das Array. |
| Index | int | Der Startindex des Arrays. |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### get(int index) {#get-int-}
```
public CustomCommandButton get(int index)
```


Ruft ein benutzerdefiniertes CommandButton-Objekt am Index ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int |  |

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


Ruft die Anzahl der Sammlung ab.

**Returns:**
int
### getSyncRoot() {#getSyncRoot--}
```
public Object getSyncRoot()
```


Nur intern verwendet.

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


Ruft den Index der Schaltfläche ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.Object | Das Schaltflächenobjekt. |

**Returns:**
int - Der Index.
### insert(int index, Object value) {#insert-int-java.lang.Object-}
```
public void insert(int index, Object value)
```


Fügt eine Schaltfläche am Index ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Index. |
| Wert | java.lang.Object | Das CustomCommandButton-Objekt. |

### isFixedSize() {#isFixedSize--}
```
public boolean isFixedSize()
```


Nur intern verwendet.

**Returns:**
boolean
### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


Nur intern verwendet.

**Returns:**
boolean
### isSynchronized() {#isSynchronized--}
```
public boolean isSynchronized()
```


Nur intern verwendet.

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


Gibt ein IEnumerator-Objekt der Sammlung zurück.

**Returns:**
java.util.Iterator – das IEnumerator-Objekt.
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


Entfernt das benutzerdefinierte Befehls-Schaltflächenobjekt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.Object | Das benutzerdefinierte Befehls-Schaltflächenobjekt. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Entfernt am Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Index. |

### set(int index, CustomCommandButton value) {#set-int-com.aspose.gridweb.CustomCommandButton-}
```
public void set(int index, CustomCommandButton value)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int |  |
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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

