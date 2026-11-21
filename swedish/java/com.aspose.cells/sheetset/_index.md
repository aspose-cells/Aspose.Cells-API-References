---
title: "SheetSet"
second_title: "Aspose.Cells för Java API-referens"
description: "Beskriver en uppsättning blad."
type: docs
url: /sv/java/com.aspose.cells/sheetset/
---

**Inheritance:**
java.lang.Object
```
public class SheetSet
```

Beskriver en uppsättning blad.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [SheetSet(int[] sheetIndexes)](#SheetSet-int---) | Skapar en bladuppsättning baserad på exakta bladindex. |
| [SheetSet(String[] sheetNames)](#SheetSet-java.lang.String---) | Skapar en bladuppsättning baserad på exakta bladnamn. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActive()](#getActive--) | Hämtar en uppsättning med det aktiva bladet i arbetsboken. |
| [getAll()](#getAll--) | Hämtar en uppsättning med alla blad i arbetsboken i deras ursprungliga ordning. |
| [getClass()](#getClass--) |  |
| [getVisible()](#getVisible--) | Hämtar en uppsättning med synliga blad i arbetsboken i deras ursprungliga ordning. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SheetSet(int[] sheetIndexes) {#SheetSet-int---}
```
public SheetSet(int[] sheetIndexes)
```


Skapar en bladuppsättning baserad på exakta bladindex.

**Remarks**

Om ett blad påträffas som inte finns i arbetsboken kommer ett undantag att kastas under rendering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetIndexes | int[] | nollbaserade bladindex. |

### SheetSet(String[] sheetNames) {#SheetSet-java.lang.String---}
```
public SheetSet(String[] sheetNames)
```


Skapar en bladuppsättning baserad på exakta bladnamn.

**Remarks**

Om ett blad påträffas som inte finns i arbetsboken kommer ett undantag att kastas under rendering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetNames | java.lang.String[] | bladnamn. |

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
### getActive() {#getActive--}
```
public static SheetSet getActive()
```


Hämtar en uppsättning med det aktiva bladet i arbetsboken.

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getAll() {#getAll--}
```
public static SheetSet getAll()
```


Hämtar en uppsättning med alla blad i arbetsboken i deras ursprungliga ordning.

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getVisible() {#getVisible--}
```
public static SheetSet getVisible()
```


Hämtar en uppsättning med synliga blad i arbetsboken i deras ursprungliga ordning.

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
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

