---
title: "GridNameCollection"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt eine Sammlung von Objekten."
type: docs
url: /de/java/com.aspose.gridweb/gridnamecollection/
---

**Inheritance:**
java.lang.Object
```
public class GridNameCollection
```

Kapselt eine Sammlung von [GridName](../../com.aspose.gridweb/gridname)-Objekten.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(int sheetIndex, String text, String refersTo)](#add-int-java.lang.String-java.lang.String-) | Definiert einen neuen Namen im angegebenen Blatt. |
| [add(String text, String refersTo)](#add-java.lang.String-java.lang.String-) | Definiert einen neuen globalen Namen. |
| [clear()](#clear--) | Entfernt alle Namen; |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Ruft das [GridName](../../com.aspose.gridweb/gridname)-Element am angegebenen Index ab. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ruft die Größe des Enumerators ab. |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Ruft den Zeilen-Enumerator ab. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String[] names)](#remove-java.lang.String---) | Entfernt ein Array von Namen. |
| [removeAt(int index)](#removeAt-int-) | Entfernt den Namen am angegebenen Index. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int sheetIndex, String text, String refersTo) {#add-int-java.lang.String-java.lang.String-}
```
public int add(int sheetIndex, String text, String refersTo)
```


Definiert einen neuen Namen im angegebenen Blatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetIndex | int | Der Blattindex, in dem der Name angewendet wird. |
| Text | java.lang.String | Namens-Text. Er darf keinen Blattnamen enthalten. |
| refersTo | java.lang.String | Die Formel, auf die der Name verweist. Sie muss einen Blattnamen enthalten, z. B. 'sheet hello!'A1:B2. |

**Returns:**
int – Index des Namensobjekts.
### add(String text, String refersTo) {#add-java.lang.String-java.lang.String-}
```
public int add(String text, String refersTo)
```


Definiert einen neuen globalen Namen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Text | java.lang.String | Namens-Text. Er kann einen Blattnamen enthalten. |
| refersTo | java.lang.String | Die Formel, auf die der Name verweist. Sie muss einen Blattnamen enthalten, z. B. 'sheet hello!'A1:B2. |

**Returns:**
int – Index des Namensobjekts.
### clear() {#clear--}
```
public void clear()
```


Entfernt alle Namen;

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
public GridName get(int index)
```


Ruft das [GridName](../../com.aspose.gridweb/gridname)-Element am angegebenen Index ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der nullbasierte Index des Elements. |

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


Ruft die Größe des Enumerators ab.

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


Ruft den Zeilen-Enumerator ab.

**Returns:**
java.util.Iterator – Der Zeilen-Enumerator.
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


Entfernt ein Array von Namen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Namen | java.lang.String[] | Der Text der Namen. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Entfernt den Namen am angegebenen Index.

**Remarks**

Stellen Sie bitte sicher, dass der Name nicht von anderen Formeln referenziert wird, bevor Sie die Methode aufrufen. Und falls der Name referenziert wird, setzen Sie bitte nur Name.RefersTo auf null.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int |  |

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

