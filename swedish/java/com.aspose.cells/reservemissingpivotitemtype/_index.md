---
title: "ReserveMissingPivotItemType"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar hur man behåller de saknade pivotelementen."
type: docs
url: /sv/java/com.aspose.cells/reservemissingpivotitemtype/
---

**Inheritance:**
java.lang.Object
```
public final class ReserveMissingPivotItemType
```

Representerar hur man behåller de saknade pivotelementen.
## Fält

| Fält | Beskrivning |
| --- | --- |
| [ALL](#ALL) | Reserverar alla saknade objekt. |
| [DEFAULT](#DEFAULT) | Tar bort gamla saknade pivot-objekt och reserverar raderade objekt från den nya datakällan som saknade objekt. |
| [NONE](#NONE) | Tar bort alla saknade pivot-objekt. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ALL {#ALL}
```
public static final int ALL
```


Reserverar alla saknade objekt.

**Remarks**

I Excel, så länge Excel inte är stängt, behålls de saknade objekten som genererats från den första uppdateringen av pivottabellen, även om du uppdaterar upprepade gånger

### DEFAULT {#DEFAULT}
```
public static final int DEFAULT
```


Tar bort gamla saknade pivot-objekt och reserverar raderade objekt från den nya datakällan som saknade objekt.

### NONE {#NONE}
```
public static final int NONE
```


Tar bort alla saknade pivot-objekt.

**Remarks**

Ordningen för gamla saknade pivotelement kommer att ignoreras.

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

