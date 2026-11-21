---
title: "PivotPageFields"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar pivotsidans objekt om pivottabellens datakälla är konsolideringsområden."
type: docs
url: /sv/java/com.aspose.cells/pivotpagefields/
---

**Inheritance:**
java.lang.Object
```
public class PivotPageFields
```

Representerar pivotsidans objekt om pivottabellens datakälla är konsolideringsområden. Den kan endast innehålla upp till 4 objekt.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [PivotPageFields()](#PivotPageFields--) | Representerar pivotsidans fältobjekt. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [addIdentify(int rangeIndex, int[] pageItemIndex)](#addIdentify-int-int---) | Anger vilken objektetikett i varje sidfält som ska användas för att identifiera dataintervallet. |
| [addPageField(String[] pageItems)](#addPageField-java.lang.String---) | Lägger till ett sidfält. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPageFieldCount()](#getPageFieldCount--) | Hämtar antalet sidfält. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotPageFields() {#PivotPageFields--}
```
public PivotPageFields()
```


Representerar pivotsidans fältobjekt.

### addIdentify(int rangeIndex, int[] pageItemIndex) {#addIdentify-int-int---}
```
public void addIdentify(int rangeIndex, int[] pageItemIndex)
```


Anger vilken objektetikett i varje sidfält som ska användas för att identifiera dataintervallet. pageItemIndex.Length måste vara lika med PageFieldCount, så lägg till sidfältet först.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rangeIndex | int | Index för konsolideringsdataintervallet. |
| pageItemIndex | int[] | Sidobjektets index i varje sidfält. pageItemIndex[2] = 1 betyder att det andra objektet i det tredje fältet används för att identifiera detta intervall. pageItemIndex[1] = -1 betyder att inget objekt i det andra fältet används för att identifiera detta intervall och MS kommer automatiskt att skapa ett \"blank\" objekt i det andra fältet för att identifiera detta intervall. |

### addPageField(String[] pageItems) {#addPageField-java.lang.String---}
```
public void addPageField(String[] pageItems)
```


Lägger till ett sidfält.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageItems | java.lang.String[] | Sidfältets objektetikett |

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
### getPageFieldCount() {#getPageFieldCount--}
```
public int getPageFieldCount()
```


Hämtar antalet sidfält.

**Returns:**
int
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

