---
title: "TxtLoadStyleStrategy"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Gibt an, wie der Stil für geparste Werte angewendet wird, wenn ein Zeichenfolgenwert in eine Zahl oder ein Datum/Uhrzeit konvertiert wird."
type: docs
url: /de/java/com.aspose.cells/txtloadstylestrategy/
---

**Inheritance:**
java.lang.Object
```
public final class TxtLoadStyleStrategy
```

Gibt an, wie der Stil für geparste Werte angewendet wird, wenn ein Zeichenfolgenwert in eine Zahl oder ein Datum/Uhrzeit konvertiert wird.
## Felder

| Feld | Beschreibung |
| --- | --- |
| [BUILT_IN](#BUILT-IN) | Setzt den Stil als integrierte Zahl/Datum‑Uhrzeit, wenn der geparste Wert reine numerische/Datum‑Uhrzeit‑Werte sind. |
| [EXACT_FORMAT](#EXACT-FORMAT) | Legt das genaue benutzerdefinierte Format für den geparsten Wert fest, sodass der formatierte Wert dem ursprünglichen Eingabewert entspricht. |
| [NONE](#NONE) | Setzt keinen Stil für den geparsten Wert. |
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
### BUILT_IN {#BUILT-IN}
```
public static final int BUILT_IN
```


Setzt den Stil als integrierte Zahl/Datum‑Uhrzeit, wenn der geparste Wert reine numerische/Datum‑Uhrzeit‑Werte sind.

**Remarks**

Wenn MS Excel Datum‑Uhrzeit‑ oder numerische Werte gemäß der Benutzereingabe (z. B. einer CSV‑Datei) parst, kann die Formatierung dieser Werte geändert werden, z. B. führende/abschließende Nullen bei Zahlen, Reihenfolge von Jahr/Monat/Tag bei Datum‑Uhrzeit, … usw. Dieser Typ dient zur Simulation des Verhaltens von MS Excel.

### EXACT_FORMAT {#EXACT-FORMAT}
```
public static final int EXACT_FORMAT
```


Legt das genaue benutzerdefinierte Format für den geparsten Wert fest, sodass der formatierte Wert dem ursprünglichen Eingabewert entspricht.

### NONE {#NONE}
```
public static final int NONE
```


Setzt keinen Stil für den geparsten Wert.

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

