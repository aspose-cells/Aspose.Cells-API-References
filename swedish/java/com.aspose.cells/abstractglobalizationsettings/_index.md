---
title: "AbstractGlobalizationSettings"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar globaliseringsinställningarna."
type: docs
url: /sv/java/com.aspose.cells/abstractglobalizationsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractGlobalizationSettings
```

Representerar globaliseringsinställningarna.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [AbstractGlobalizationSettings()](#AbstractGlobalizationSettings--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [compare(String v1, String v2, boolean ignoreCase)](#compare-java.lang.String-java.lang.String-boolean-) | Jämför två strängvärden enligt vissa sorteringsregler. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCollationKey(String v, boolean ignoreCase)](#getCollationKey-java.lang.String-boolean-) | Omvandlar strängen till ett jämförbart objekt enligt vissa sorteringsregler. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractGlobalizationSettings() {#AbstractGlobalizationSettings--}
```
public AbstractGlobalizationSettings()
```


### compare(String v1, String v2, boolean ignoreCase) {#compare-java.lang.String-java.lang.String-boolean-}
```
public int compare(String v1, String v2, boolean ignoreCase)
```


Jämför två strängvärden enligt vissa sorteringsregler.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| v1 | java.lang.String | den första strängen |
| v2 | java.lang.String | den andra strängen |
| ignoreCase | boolean | om skiftlägeskänslighet ska ignoreras vid jämförelse av värden |

**Returns:**
int - Heltal som indikerar det lexikala förhållandet mellan de två jämförelseoperanderna
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
### getCollationKey(String v, boolean ignoreCase) {#getCollationKey-java.lang.String-boolean-}
```
public Comparable getCollationKey(String v, boolean ignoreCase)
```


Omvandlar strängen till ett jämförbart objekt enligt vissa sorteringsregler.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| v | java.lang.String | Strängvärdet måste jämföras med andra. |
| ignoreCase | boolean | om skiftlägeskänslighet ska ignoreras vid jämförelse av värden |

**Returns:**
java.lang.Comparable - Objekt kan användas för att jämföra eller sortera strängvärden
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

