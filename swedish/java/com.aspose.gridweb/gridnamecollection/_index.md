---
title: "GridNameCollection"
second_title: "Aspose.Cells för Java API-referens"
description: "Inkapslar en samling av objekt."
type: docs
url: /sv/java/com.aspose.gridweb/gridnamecollection/
---

**Inheritance:**
java.lang.Object
```
public class GridNameCollection
```

Inkapslar en samling av [GridName](../../com.aspose.gridweb/gridname) objekt.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(int sheetIndex, String text, String refersTo)](#add-int-java.lang.String-java.lang.String-) | Definierar ett nytt namn i det angivna bladet. |
| [add(String text, String refersTo)](#add-java.lang.String-java.lang.String-) | Definierar ett nytt globalt namn. |
| [clear()](#clear--) | Tar bort alla namn; |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Hämtar [GridName](../../com.aspose.gridweb/gridname)-elementet på det angivna indexet. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Hämtar storleken på enumeratorn |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Hämtar enumerator för rader |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String[] names)](#remove-java.lang.String---) | Ta bort en array av namn. |
| [removeAt(int index)](#removeAt-int-) | Ta bort namnet på det specifika indexet. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int sheetIndex, String text, String refersTo) {#add-int-java.lang.String-java.lang.String-}
```
public int add(int sheetIndex, String text, String refersTo)
```


Definierar ett nytt namn i det angivna bladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetIndex | int | Bladindexet där namnet tillämpas. |
| text | java.lang.String | Namnetext. Det kan inte ha bladnamn. |
| refersTo | java.lang.String | Formeln som namnet är definierat att referera till. Den måste ha bladnamn. t.ex. 'sheet hello!'A1:B2. |

**Returns:**
int - Namnobjektets index.
### add(String text, String refersTo) {#add-java.lang.String-java.lang.String-}
```
public int add(String text, String refersTo)
```


Definierar ett nytt globalt namn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| text | java.lang.String | Namnetext. Det kan ha bladnamn. |
| refersTo | java.lang.String | Formeln som namnet är definierat att referera till. Den måste ha ett bladnamn. t.ex. 'sheet hello!'A1:B2. |

**Returns:**
int - Namnobjektets index.
### clear() {#clear--}
```
public void clear()
```


Tar bort alla namn;

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### get(int index) {#get-int-}
```
public GridName get(int index)
```


Hämtar [GridName](../../com.aspose.gridweb/gridname)-elementet på det angivna indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Det nollbaserade indexet för elementet. |

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


Hämtar storleken på enumeratorn

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


Hämtar enumerator för rader

**Returns:**
java.util.Iterator - Enumeratör för rader
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


Ta bort en array av namn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | java.lang.String[] | Texten för namnen. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Ta bort namnet på det specifika indexet.

**Remarks**

Se till att namnet inte refereras av andra formler innan metoden anropas. Och om namnet refereras, ange endast Name.RefersTo till null.

**Parameters:**
| Parameter | Typ | Beskrivning |
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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

