---
title: "TxtLoadStyleStrategy"
second_title: "Aspose.Cells för Java API-referens"
description: "Anger hur stil ska tillämpas på tolkade värden när en strängvärde konverteras till nummer eller datumtid."
type: docs
url: /sv/java/com.aspose.cells/txtloadstylestrategy/
---

**Inheritance:**
java.lang.Object
```
public final class TxtLoadStyleStrategy
```

Anger hur stil ska tillämpas på tolkade värden när en strängvärde konverteras till nummer eller datumtid.
## Fält

| Fält | Beskrivning |
| --- | --- |
| [BUILT_IN](#BUILT-IN) | Ställ in stilen som inbyggt nummer/datumtid när det analyserade värdet är rena numeriska/datumtidvärden. |
| [EXACT_FORMAT](#EXACT-FORMAT) | Ange det exakta anpassade formatet för det analyserade värdet så att det formaterade värdet blir detsamma som det ursprungliga inmatade. |
| [NONE](#NONE) | Ställer inte in stil för det analyserade värdet. |
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
### BUILT_IN {#BUILT-IN}
```
public static final int BUILT_IN
```


Ställ in stilen som inbyggt nummer/datumtid när det analyserade värdet är rena numeriska/datumtidvärden.

**Remarks**

När MS Excel tolkar datum/tid eller numeriska värden enligt användarens inmatning (t.ex. CSV‑fil) kan formateringen av dessa värden ändras, såsom inledande/slutande nollor i tal, år/månad/dag‑ordning för datum/tid, … osv. Denna typ används för att simulera MS Excels beteende.

### EXACT_FORMAT {#EXACT-FORMAT}
```
public static final int EXACT_FORMAT
```


Ange det exakta anpassade formatet för det analyserade värdet så att det formaterade värdet blir detsamma som det ursprungliga inmatade.

### NONE {#NONE}
```
public static final int NONE
```


Ställer inte in stil för det analyserade värdet.

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

