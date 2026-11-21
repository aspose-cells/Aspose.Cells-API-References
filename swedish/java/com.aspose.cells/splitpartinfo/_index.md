---
title: "SplitPartInfo"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar informationen för en in-/utdata för flera in-/utdata, såsom aktuell sida som ska renderas vid konvertering av kalkylblad till bild."
type: docs
url: /sv/java/com.aspose.cells/splitpartinfo/
---

**Inheritance:**
java.lang.Object
```
public class SplitPartInfo
```

Representerar informationen för en in-/utmatning för flera in-/utmatningar, såsom aktuell sida som ska renderas vid konvertering av kalkylblad till bild.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPartIndex()](#getPartIndex--) | Index för aktuell del i sekvensen (0‑baserad) |
| [getSheetIndex()](#getSheetIndex--) | Index för bladet där den aktuella delen finns. -1 betyder att det bara finns ett blad. |
| [getSheetName()](#getSheetName--) | Namn på bladet där den aktuella delen finns. |
| [hashCode()](#hashCode--) |  |
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
### getPartIndex() {#getPartIndex--}
```
public int getPartIndex()
```


Index för aktuell del i sekvensen (0‑baserad). -1 betyder att det inte finns flera delar så resultatet är enstaka.

**Remarks**

Om flera blad måste bearbetas och varje blad bearbetas (splittras) separat, startar del‑index alltid från 0 för varje blad. Till exempel, vid konvertering av arbetsbok till bilder, representerar det utskrifts‑sidindex för det blad som för närvarande bearbetas. Och -1 betyder att det bara finns en sida för det aktuella bladet.

**Returns:**
int
### getSheetIndex() {#getSheetIndex--}
```
public int getSheetIndex()
```


Index för bladet där den aktuella delen finns. -1 betyder att det bara finns ett blad.

**Returns:**
int
### getSheetName() {#getSheetName--}
```
public String getSheetName()
```


Namn på bladet där den aktuella delen finns.

**Remarks**

Kan vara null i vissa situationer, till exempel när hela arbetsboken renderas till tiff‑bild.

**Returns:**
java.lang.String
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

