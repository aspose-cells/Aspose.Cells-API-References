---
title: "SessionMode"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt den Sitzungsmodus des Rasters dar."
type: docs
url: /de/java/com.aspose.gridweb/sessionmode/
---

**Inheritance:**
java.lang.Object
```
public final class SessionMode
```

Stellt den Sitzungsmodus des Rasters dar.
## Felder

| Feld | Beschreibung |
| --- | --- |
| [CUSTOM](#CUSTOM) | Verwendet das LoadCustomData‑Ereignis, um die Blattdaten des Rasters manuell zu laden. |
| [FILE](#FILE) | Verwendet die Systemdatei, um die Blattdaten des Rasters automatisch zu speichern/wiederherzustellen; der Benutzer muss SessionStorePath festlegen, um das Dateiverzeichnis anzugeben. |
| [SESSION](#SESSION) | Verwendet die Systemsitzung, um die Blattdaten des Rasters automatisch zu speichern/wiederherzustellen. |
| [VIEW_STATE](#VIEW-STATE) | Verwendet den ViewState der Seite, um die Blattdaten des Rasters automatisch zu speichern/wiederherzustellen. |
## Methoden

| Methode | Beschreibung |
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


Verwendet das LoadCustomData‑Ereignis, um die Blattdaten des Rasters manuell zu laden. Und verwendet das SheetDataUpdated‑Ereignis, um die Blattdaten des Rasters zu speichern.

### FILE {#FILE}
```
public static final int FILE
```


Verwendet die Systemdatei, um die Blattdaten des Rasters automatisch zu speichern/wiederherzustellen; der Benutzer muss SessionStorePath festlegen, um das Dateiverzeichnis anzugeben.

### SESSION {#SESSION}
```
public static final int SESSION
```


Verwendet die Systemsitzung, um die Blattdaten des Rasters automatisch zu speichern/wiederherzustellen.

### VIEW_STATE {#VIEW-STATE}
```
public static final int VIEW_STATE
```


Verwendet den ViewState der Seite, um die Blattdaten des Rasters automatisch zu speichern/wiederherzustellen.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

