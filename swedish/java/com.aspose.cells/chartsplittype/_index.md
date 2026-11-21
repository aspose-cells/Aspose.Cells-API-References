---
title: "ChartSplitType"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar hur de två sektionerna i antingen ett paj‑i‑paj‑diagram eller ett stapel‑i‑paj‑diagram delas."
type: docs
url: /sv/java/com.aspose.cells/chartsplittype/
---

**Inheritance:**
java.lang.Object
```
public final class ChartSplitType
```

Representerar hur de två sektionerna i antingen ett paj‑i‑paj‑diagram eller ett stapel‑i‑paj‑diagram delas.
## Fält

| Fält | Beskrivning |
| --- | --- |
| [AUTO](#AUTO) | Representerar datapunkterna som ska delas med standardmekanismen för denna diagramtyp. |
| [CUSTOM](#CUSTOM) | Representerar datapunkterna som ska delas mellan pajdiagrammet och det andra diagrammet enligt de anpassade delningsvärdena. |
| [PERCENT_VALUE](#PERCENT-VALUE) | Representerar datapunkterna som ska delas mellan pajdiagrammet och det andra diagrammet genom att placera de punkter med en procentandel mindre än Split Position-procenten i det andra diagrammet. |
| [POSITION](#POSITION) | Representerar datapunkterna. |
| [VALUE](#VALUE) | Representerar att datapunkterna ska delas mellan pajdiagrammet och det andra diagrammet genom att placera datapunkterna med värde mindre än Split Position i det andra diagrammet. |
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
### AUTO {#AUTO}
```
public static final int AUTO
```


Representerar datapunkterna som ska delas med standardmekanismen för denna diagramtyp.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället Series.IsAutoSplit-egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med september 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### CUSTOM {#CUSTOM}
```
public static final int CUSTOM
```


Representerar datapunkterna som ska delas mellan pajdiagrammet och det andra diagrammet enligt de anpassade delningsvärdena.

### PERCENT_VALUE {#PERCENT-VALUE}
```
public static final int PERCENT_VALUE
```


Representerar datapunkterna som ska delas mellan pajdiagrammet och det andra diagrammet genom att placera de punkter med en procentandel mindre än Split Position-procenten i det andra diagrammet.

### POSITION {#POSITION}
```
public static final int POSITION
```


Representerar datapunkterna. Datapunkterna ska delas mellan pajdiagrammet och det andra diagrammet genom att placera den sista split positionen för datapunkterna i det andra diagrammet.

### VALUE {#VALUE}
```
public static final int VALUE
```


Representerar att datapunkterna ska delas mellan pajdiagrammet och det andra diagrammet genom att placera datapunkterna med värde mindre än Split Position i det andra diagrammet.

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

