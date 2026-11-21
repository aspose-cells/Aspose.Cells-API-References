---
title: "AboveAverage"
second_title: "Aspose.Cells för Java API-referens"
description: "Beskriv regeln för villkorsformatering AboveAverage."
type: docs
url: /sv/java/com.aspose.cells/aboveaverage/
---

**Inheritance:**
java.lang.Object
```
public class AboveAverage
```

Beskriv regeln för villkorsstyrd formatering AboveAverage. Denna villkorsstyrda formateringsregel markerar celler som är över eller under genomsnittet för alla värden i intervallet.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [AboveAverage()](#AboveAverage--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getStdDev()](#getStdDev--) | Hämtar antalet standardavvikelser som ska inkluderas över eller under genomsnittet i regeln för villkorsstyrd formatering. |
| [hashCode()](#hashCode--) |  |
| [isAboveAverage()](#isAboveAverage--) | Hämtar flaggan som indikerar om regeln är en "above average"-regel. |
| [isEqualAverage()](#isEqualAverage--) | Hämtar flaggan som indikerar om kriterierna 'aboveAverage' och 'belowAverage' är inklusiva för själva genomsnittet, eller exkluderar det värdet. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAboveAverage(boolean value)](#setAboveAverage-boolean-) | Ställer in flaggan som indikerar om regeln är en "above average"-regel. |
| [setEqualAverage(boolean value)](#setEqualAverage-boolean-) | Ställer in flaggan som indikerar om kriterierna 'aboveAverage' och 'belowAverage' är inklusiva för själva genomsnittet, eller exkluderar det värdet. |
| [setStdDev(int value)](#setStdDev-int-) | Ställer in antalet standardavvikelser som ska inkluderas över eller under genomsnittet i regeln för villkorsstyrd formatering. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AboveAverage() {#AboveAverage--}
```
public AboveAverage()
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getStdDev() {#getStdDev--}
```
public int getStdDev()
```


Hämtar antalet standardavvikelser som ska inkluderas över eller under genomsnittet i regeln för villkorsstyrd formatering. Inmatningsvärdet måste ligga mellan 0 och 3 (inklusive 0 och 3). Att sätta detta värde till 0 betyder att stdDev inte är angivet. Standardvärdet är 0.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAboveAverage() {#isAboveAverage--}
```
public boolean isAboveAverage()
```


Hämtar flaggan som indikerar om regeln är en "above average"-regel. 'true' indikerar 'above average'. Standardvärdet är true.

**Returns:**
boolean
### isEqualAverage() {#isEqualAverage--}
```
public boolean isEqualAverage()
```


Hämtar flaggan som indikerar om kriterierna 'aboveAverage' och 'belowAverage' är inklusiva för själva genomsnittet, eller exkluderar det värdet. 'true' indikerar att genomsnittsvärdet ska inkluderas i kriterierna. Standardvärdet är false.

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




### setAboveAverage(boolean value) {#setAboveAverage-boolean-}
```
public void setAboveAverage(boolean value)
```


Ställer in flaggan som indikerar om regeln är en "above average"-regel. 'true' indikerar 'above average'. Standardvärdet är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEqualAverage(boolean value) {#setEqualAverage-boolean-}
```
public void setEqualAverage(boolean value)
```


Ställer in flaggan som indikerar om kriterierna 'aboveAverage' och 'belowAverage' är inklusiva för själva genomsnittet, eller exkluderar det värdet. 'true' indikerar att genomsnittsvärdet ska inkluderas i kriterierna. Standardvärdet är false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setStdDev(int value) {#setStdDev-int-}
```
public void setStdDev(int value)
```


Ställer in antalet standardavvikelser som ska inkluderas över eller under genomsnittet i regeln för villkorsstyrd formatering. Inmatningsvärdet måste ligga mellan 0 och 3 (inklusive 0 och 3). Att sätta detta värde till 0 betyder att stdDev inte är angivet. Standardvärdet är 0.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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

