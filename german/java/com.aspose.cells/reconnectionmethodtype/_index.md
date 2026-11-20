---
title: "ReConnectionMethodType"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Gibt an, was die Tabellenkalkulationsanwendung tun soll, wenn eine Verbindung fehlschlägt."
type: docs
url: /de/java/com.aspose.cells/reconnectionmethodtype/
---

**Inheritance:**
java.lang.Object
```
public final class ReConnectionMethodType
```

Gibt an, was die Tabellenkalkulationsanwendung tun soll, wenn eine Verbindung fehlschlägt.
## Felder

| Feld | Beschreibung |
| --- | --- |
| [ALWAYS](#ALWAYS) | Bei jeder Aktualisierung die aktualisierten Verbindungsinformationen aus der externen Verbindungsdatei abrufen, falls verfügbar, und diese anstelle der vorhandenen Verbindungsinformationen verwenden. |
| [NEVER](#NEVER) | Nie die aktualisierten Verbindungsinformationen aus der externen Verbindungsdatei abrufen, selbst wenn sie verfügbar ist und selbst wenn die vorhandenen Verbindungsinformationen ungültig sind. |
| [REQUIRED](#REQUIRED) | Bei einer Aktualisierung die vorhandenen Verbindungsinformationen verwenden und, falls sie sich als ungültig erweisen, die aktualisierten Verbindungsinformationen, falls verfügbar, aus der externen Verbindungsdatei abrufen. |
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
### ALWAYS {#ALWAYS}
```
public static final int ALWAYS
```


Bei jeder Aktualisierung die aktualisierten Verbindungsinformationen aus der externen Verbindungsdatei abrufen, falls verfügbar, und diese anstelle der vorhandenen Verbindungsinformationen verwenden. In diesem Fall schlägt die Datenaktualisierung fehl, wenn die externe Verbindungsdatei nicht verfügbar ist.

### NEVER {#NEVER}
```
public static final int NEVER
```


Nie die aktualisierten Verbindungsinformationen aus der externen Verbindungsdatei abrufen, selbst wenn sie verfügbar ist und selbst wenn die vorhandenen Verbindungsinformationen ungültig sind.

### REQUIRED {#REQUIRED}
```
public static final int REQUIRED
```


Bei einer Aktualisierung die vorhandenen Verbindungsinformationen verwenden und, falls sie sich als ungültig erweisen, die aktualisierten Verbindungsinformationen, falls verfügbar, aus der externen Verbindungsdatei abrufen.

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

