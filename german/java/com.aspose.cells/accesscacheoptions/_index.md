---
title: "AccessCacheOptions"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Cache‑Optionen für den Datenzugriff."
type: docs
url: /de/java/com.aspose.cells/accesscacheoptions/
---

**Inheritance:**
java.lang.Object
```
public final class AccessCacheOptions
```

Cache-Optionen für den Datenzugriff. Mehrere Optionen können mit dem "\|"‑Operator kombiniert werden.

**Remarks**

Für einige Funktionen erfordert der Zugriff auf große Datensätze viele wiederholte und komplexe Vorgänge wie Suche, Berechnung, ...etc und diese Vorgänge benötigen zusätzliche Zeit. In üblichen Situationen bleiben alle abhängigen Daten während des Zugriffs unverändert, sodass einige Caches erstellt und verwendet werden können, um die Zugriffsleistung zu verbessern. Zu diesem Zweck stellen wir diese API bereit, damit der Benutzer angeben kann, welche Art von Datenzugriff durch einen möglichen Caching‑Mechanismus optimiert werden soll.

Bitte beachten Sie, dass für verschiedene Optionen unterschiedliche Datensätze möglicherweise als "read-only" (schreibgeschützt) erforderlich sind. Und die Leistungsfähigkeit des Datenzugriffs hängt von vielen Aspekten ab; die Verwendung eines Caching‑Mechanismus garantiert nicht, dass die Leistung verbessert wird. In manchen Situationen, z. B. wenn der zuzugreifende Datensatz klein ist, kann die Nutzung eines Caches sogar mehr Zeit benötigen, da das Caching selbst ebenfalls zusätzlichen Aufwand erfordert.
## Felder

| Feld | Beschreibung |
| --- | --- |
| [ALL](#ALL) | Wenden Sie alle möglichen Optimierungen für alle Arten des Datenzugriffs in der Arbeitsmappe an. |
| [CALCULATE_FORMULA](#CALCULATE-FORMULA) | Wenden Sie mögliche Optimierungen für die Berechnung von Formeln an. |
| [CELLS_DATA](#CELLS-DATA) | Wenden Sie mögliche Optimierungen für das Abrufen von Zellwerten an. |
| [CELL_DISPLAY](#CELL-DISPLAY) | Wenden Sie mögliche Optimierungen für das Abrufen von darstellungsbezogenen Ergebnissen von Zellen an([Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--), [Cell.getStyle()](../../com.aspose.cells/cell\#getStyle--), [Cell.getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--), etc.). |
| [CONDITIONAL_FORMATTING](#CONDITIONAL-FORMATTING) | Wenden Sie mögliche Optimierungen für das Abrufen von Formatierungsergebnissen bedingter Formatierungen an. |
| [GET_FORMULA](#GET-FORMULA) | Wenden Sie mögliche Optimierungen für das Abrufen von Formeln an. |
| [NONE](#NONE) | Kein Cache für jeglichen Datenzugriff. |
| [POSITION_AND_SIZE](#POSITION-AND-SIZE) | Wenden Sie mögliche Optimierungen für das Abrufen der Position und Größe von Objekten (wie Shape) an. |
| [SET_FORMULA](#SET-FORMULA) | Wenden Sie mögliche Optimierungen für das Festlegen von Formeln an. |
| [VALIDATION](#VALIDATION) | Wenden Sie mögliche Optimierungen für das Abrufen von Validierungsergebnissen an. |
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
### ALL {#ALL}
```
public static final int ALL
```


Wenden Sie alle möglichen Optimierungen für alle Arten des Datenzugriffs in der Arbeitsmappe an. Alle Einstellungen und Daten sollten während des optimierten Zugriffs nicht geändert werden.

### CALCULATE_FORMULA {#CALCULATE-FORMULA}
```
public static final int CALCULATE_FORMULA
```


Wenden Sie mögliche Optimierungen für die Berechnung von Formeln an. Zieldaten sollten während des optimierten Zugriffs nicht geändert werden, es sollten auch keine neuen Objekte (Cell, Row usw.) erstellt werden (wie durch [Cells.get(int,int)](../../com.aspose.cells/cells\#get-int-int-)).

### CELLS_DATA {#CELLS-DATA}
```
public static final int CELLS_DATA
```


Wenden Sie mögliche Optimierungen für das Abrufen von Zellwerten an. Zieldaten (Daten und Einstellungen von Cell, Row) sollten während des optimierten Zugriffs nicht geändert werden, es sollten auch keine neuen Cell/Row-Objekte erstellt werden (wie durch [Cells.get(int,int)](../../com.aspose.cells/cells\#get-int-int-)).

### CELL_DISPLAY {#CELL-DISPLAY}
```
public static final int CELL_DISPLAY
```


Wenden Sie mögliche Optimierungen für das Abrufen von darstellungsbezogenen Ergebnissen von Zellen an([Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--), [Cell.getStyle()](../../com.aspose.cells/cell\#getStyle--), [Cell.getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--), etc.). Zieldaten und stilbezogene Objekte (Cell/Row/Column-Stile, Spaltenbreite usw.) sollten während des optimierten Zugriffs nicht geändert werden.

### CONDITIONAL_FORMATTING {#CONDITIONAL-FORMATTING}
```
public static final int CONDITIONAL_FORMATTING
```


Wenden Sie mögliche Optimierungen für das Abrufen von Formatierungsergebnissen bedingter Formatierungen an. Alle Daten und Einstellungen, die das Ergebnis bedingter Formatierungen beeinflussen können (Einstellungen der bedingten Formatierungen, abhängige Zellwerte usw.), sollten während des optimierten Zugriffs nicht geändert werden.

### GET_FORMULA {#GET-FORMULA}
```
public static final int GET_FORMULA
```


Wenden Sie mögliche Optimierungen für das Abrufen von Formeln an. Alle Daten und Einstellungen, die den Formelausdruck beeinflussen können (Arbeitsblattname, Name-Text, Tabellenspalte usw.), sollten während des optimierten Zugriffs nicht geändert werden.

### NONE {#NONE}
```
public static final int NONE
```


Kein Cache für jeglichen Datenzugriff.

### POSITION_AND_SIZE {#POSITION-AND-SIZE}
```
public static final int POSITION_AND_SIZE
```


Wenden Sie mögliche Optimierungen für das Abrufen der Position und Größe von Objekten (wie Shape) an. Zeilenhöhen- und Spaltenbreiteneinstellungen sollten während des optimierten Zugriffs nicht geändert werden.

### SET_FORMULA {#SET-FORMULA}
```
public static final int SET_FORMULA
```


Wenden Sie mögliche Optimierungen für das Festlegen von Formeln an. Alle Daten und Einstellungen, die den Formelausdruck beeinflussen können (Arbeitsblattname, Name-Text, Tabellenspalte usw.), sollten während des optimierten Zugriffs nicht geändert werden.

### VALIDATION {#VALIDATION}
```
public static final int VALIDATION
```


Mögliche Optimierung für das Erhalten des Validierungsergebnisses anwenden. Alle Daten und Einstellungen, die das Ergebnis der Validierung (Einstellungen der Validierung, abhängige Zellenwerte usw.) beeinflussen könnten, sollten während des optimierten Zugriffs nicht geändert werden.

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

