---
title: "RenameStrategy"
second_title: "Aspose.Cells för Java API-referens"
description: "Strategialternativ för duplicerade kolumnnamn."
type: docs
url: /sv/java/com.aspose.cells/renamestrategy/
---

**Inheritance:**
java.lang.Object
```
public final class RenameStrategy
```

Strategialternativ för duplicerade kolumnnamn.

**Remarks**

När du bearbetar data med rubriker kräver vissa scenarier att rubrikerna inte dupliceras för alla kolumner. Till exempel, när du exporterar data till en datatabell och rubriken ska användas som datatabellens kolumnnamn, är duplicerade rubrikvärden ogiltiga. För sådana situationer kan användaren bestämma hur de ska hanteras genom att ange denna strategi.
## Fält

| Fält | Beskrivning |
| --- | --- |
| [DIGIT](#DIGIT) | Namngiven med siffra. |
| [EXCEPTION](#EXCEPTION) | Kastar undantag. |
| [LETTER](#LETTER) | Namngiven med bokstav.. |
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
### DIGIT {#DIGIT}
```
public static final int DIGIT
```


Namngiven med siffra. Duplicerade namn blir ...1, ...2, osv.

### EXCEPTION {#EXCEPTION}
```
public static final int EXCEPTION
```


Kastar undantag.

### LETTER {#LETTER}
```
public static final int LETTER
```


Namngiven med bokstav.. Duplicerade namn blir ...A, ...B, osv.

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

