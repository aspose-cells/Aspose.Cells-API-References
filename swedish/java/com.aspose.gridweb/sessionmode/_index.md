---
title: "SessionMode"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar sessionsläget för rutnätet."
type: docs
url: /sv/java/com.aspose.gridweb/sessionmode/
---

**Inheritance:**
java.lang.Object
```
public final class SessionMode
```

Representerar sessionsläget för rutnätet.
## Fält

| Fält | Beskrivning |
| --- | --- |
| [CUSTOM](#CUSTOM) | Använder LoadCustomData-händelsen för att ladda gridens bladdata manuellt. |
| [FILE](#FILE) | Använder systemfilen för att lagra/återställa gridens bladdata automatiskt, användaren måste ange SessionStorePath för att specificera filkatalogen. |
| [SESSION](#SESSION) | Använder systemsessionen för att lagra/återställa gridens bladdata automatiskt. |
| [VIEW_STATE](#VIEW-STATE) | Använder sidans viewstate för att lagra/återställa gridens bladdata automatiskt. |
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
### CUSTOM {#CUSTOM}
```
public static final int CUSTOM
```


Använder LoadCustomData-händelsen för att ladda gridens bladdata manuellt. Och använder SheetDataUpdated-händelsen för att spara gridens bladdata.

### FILE {#FILE}
```
public static final int FILE
```


Använder systemfilen för att lagra/återställa gridens bladdata automatiskt, användaren måste ange SessionStorePath för att specificera filkatalogen.

### SESSION {#SESSION}
```
public static final int SESSION
```


Använder systemsessionen för att lagra/återställa gridens bladdata automatiskt.

### VIEW_STATE {#VIEW-STATE}
```
public static final int VIEW_STATE
```


Använder sidans viewstate för att lagra/återställa gridens bladdata automatiskt.

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

