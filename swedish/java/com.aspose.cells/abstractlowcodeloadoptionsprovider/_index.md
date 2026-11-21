---
title: "AbstractLowCodeLoadOptionsProvider"
second_title: "Aspose.Cells för Java API-referens"
description: "Implementering för att tillhandahålla flera inläsningsalternativ för processer som använder flera indata, såsom mallfiler."
type: docs
url: /sv/java/com.aspose.cells/abstractlowcodeloadoptionsprovider/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractLowCodeLoadOptionsProvider
```

Implementering för att tillhandahålla flera inläsningsalternativ för processer som använder flera indata (t.ex. mallfiler).

**Remarks**

Till exempel kräver funktionen [SpreadsheetMerger](../../com.aspose.cells/spreadsheetmerger) flera mallfiler för att slå samman.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [AbstractLowCodeLoadOptionsProvider()](#AbstractLowCodeLoadOptionsProvider--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finish(LowCodeLoadOptions part)](#finish-com.aspose.cells.LowCodeLoadOptions-) | Frigör resurser efter att ha bearbetat den aktuella delen av indata. |
| [getClass()](#getClass--) |  |
| [getCurrent()](#getCurrent--) | Hämtar inläsningsalternativen från vilka data för den för närvarande bearbetade delen ska läsas in. |
| [hashCode()](#hashCode--) |  |
| [moveNext()](#moveNext--) | Kontrollerar om det finns mer indata. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractLowCodeLoadOptionsProvider() {#AbstractLowCodeLoadOptionsProvider--}
```
public AbstractLowCodeLoadOptionsProvider()
```


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
### finish(LowCodeLoadOptions part) {#finish-com.aspose.cells.LowCodeLoadOptions-}
```
public void finish(LowCodeLoadOptions part)
```


Frigör resurser efter att ha bearbetat den aktuella delen av indata.

**Remarks**

Som standard stänger den här metoden bara strömmen som anges av [LowCodeLoadOptions.getInputStream()](../../com.aspose.cells/lowcodeloadoptions\#getInputStream--) direkt (om inläsningsalternativen specificerade en Ström som källa). Användaren kan skriva över den här metoden för att styra hur resurser frigörs enligt deras krav och implementeringen av [getCurrent()](../../com.aspose.cells/abstractlowcodeloadoptionsprovider\#getCurrent--).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| part | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | inläsningsalternativen som används för den för närvarande delade delen. |

### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCurrent() {#getCurrent--}
```
public abstract LowCodeLoadOptions getCurrent()
```


Hämtar inläsningsalternativen från vilka data för den för närvarande bearbetade delen ska läsas in.

**Returns:**
[LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### moveNext() {#moveNext--}
```
public abstract boolean moveNext()
```


Kontrollerar om det finns mer indata.

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

