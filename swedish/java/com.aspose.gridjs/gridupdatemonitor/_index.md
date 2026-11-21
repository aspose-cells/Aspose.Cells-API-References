---
title: "GridUpdateMonitor"
second_title: "Aspose.Cells för Java API-referens"
description: "Övervakar så att användaren kan följa förändringen av uppdateringsoperationen."
type: docs
url: /sv/java/com.aspose.gridjs/gridupdatemonitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class GridUpdateMonitor
```

Övervakar så att användaren kan följa förändringen av uppdateringsoperationen.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [GridUpdateMonitor()](#GridUpdateMonitor--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [afterUpdate(String op, String uid, ArrayList cells)](#afterUpdate-java.lang.String-java.lang.String-java.util.ArrayList-) | efter uppdateringsoperation |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridUpdateMonitor() {#GridUpdateMonitor--}
```
public GridUpdateMonitor()
```


### afterUpdate(String op, String uid, ArrayList cells) {#afterUpdate-java.lang.String-java.lang.String-java.util.ArrayList-}
```
public abstract void afterUpdate(String op, String uid, ArrayList cells)
```


efter uppdateringsoperation

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| op | java.lang.String | JSON-strängen för uppdateringsoperationen |
| uid | java.lang.String | Det unika id-et för filcachen. |
| celler | java.util.ArrayList | Den uppdaterade celllistan, inkluderar celler som har stiländring, värdeändring eller formelförändring |

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

