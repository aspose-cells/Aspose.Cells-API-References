---
title: "GridReferredArea"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar ett refererat område enligt formeln."
type: docs
url: /sv/java/com.aspose.gridjs/gridreferredarea/
---

**Inheritance:**
java.lang.Object
```
public class GridReferredArea
```

Representerar ett refererat område enligt formeln.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getEndColumn()](#getEndColumn--) | Slutkolumnen för området. |
| [getEndRow()](#getEndRow--) | Slutraden för området. |
| [getExternalFileName()](#getExternalFileName--) | Hämta det externa filnamnet om detta är en extern referens. |
| [getSheetName()](#getSheetName--) | Anger vilket blad detta är i |
| [getStartColumn()](#getStartColumn--) | Startkolumnen för området. |
| [getStartRow()](#getStartRow--) | Startraden för området. |
| [getValue(int rowOffset, int colOffset)](#getValue-int-int-) | Hämtar cellvärde med given offset från övre vänstra hörnet av detta område. |
| [getValues()](#getValues--) | Hämtar cellvärden i detta område. |
| [hashCode()](#hashCode--) |  |
| [isArea()](#isArea--) | Anger om detta är ett område. |
| [isExternalLink()](#isExternalLink--) | Anger om detta är en extern länk. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEndColumn() {#getEndColumn--}
```
public int getEndColumn()
```


Slutkolumnen för området.

**Returns:**
int
### getEndRow() {#getEndRow--}
```
public int getEndRow()
```


Slutraden för området.

**Returns:**
int
### getExternalFileName() {#getExternalFileName--}
```
public String getExternalFileName()
```


Hämta det externa filnamnet om detta är en extern referens.

**Returns:**
java.lang.String
### getSheetName() {#getSheetName--}
```
public String getSheetName()
```


Anger vilket blad detta är i

**Returns:**
java.lang.String
### getStartColumn() {#getStartColumn--}
```
public int getStartColumn()
```


Startkolumnen för området.

**Returns:**
int
### getStartRow() {#getStartRow--}
```
public int getStartRow()
```


Startraden för området.

**Returns:**
int
### getValue(int rowOffset, int colOffset) {#getValue-int-int-}
```
public Object getValue(int rowOffset, int colOffset)
```


Hämtar cellvärde med given offset från övre vänstra hörnet av detta område.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowOffset | int | radoffset från startraden för detta område |
| colOffset | int | kolumnoffset från startraden för detta område |

**Returns:**
java.lang.Object - "\#REF!" om detta område är ogiltigt; "\#N/A" om angivet offset ligger utanför detta område; annars returneras cellvärdet på den angivna positionen.
### getValues() {#getValues--}
```
public Object getValues()
```


Hämtar cellvärden i detta område.

**Returns:**
java.lang.Object - Om detta område är ogiltigt returneras "\#REF!"; Om detta område är en enda cell returneras cellvärdesobjektet; Annars returneras en array med alla värden i detta område.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isArea() {#isArea--}
```
public boolean isArea()
```


Anger om detta är ett område.

**Remarks**

Om detta inte är ett område påverkas endast StartRow och StartColumn.

**Returns:**
boolean
### isExternalLink() {#isExternalLink--}
```
public boolean isExternalLink()
```


Anger om detta är en extern länk.

**Returns:**
boolean
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

