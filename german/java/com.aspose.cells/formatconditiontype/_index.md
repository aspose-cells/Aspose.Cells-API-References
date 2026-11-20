---
title: "FormatConditionType"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Typ der Regel für bedingte Formatierung."
type: docs
url: /de/java/com.aspose.cells/formatconditiontype/
---

**Inheritance:**
java.lang.Object
```
public final class FormatConditionType
```

Typ der Regel für bedingte Formatierung.
## Felder

| Feld | Beschreibung |
| --- | --- |
| [ABOVE_AVERAGE](#ABOVE-AVERAGE) | Diese bedingte Formatierungsregel hebt Zellen hervor, die über oder unter dem Durchschnitt aller Werte im Bereich liegen. |
| [BEGINS_WITH](#BEGINS-WITH) | Diese bedingte Formatierungsregel hebt Zellen im Bereich hervor, die mit dem angegebenen Text beginnen. |
| [CELL_VALUE](#CELL-VALUE) | Diese bedingte Formatierungsregel vergleicht einen Zellenwert mit einem durch eine Formel berechneten Ergebnis unter Verwendung eines Operators. |
| [COLOR_SCALE](#COLOR-SCALE) | Diese bedingte Formatierungsregel erstellt eine abgestufte Farbskala für die Zellen. |
| [CONTAINS_BLANKS](#CONTAINS-BLANKS) | Diese bedingte Formatierungsregel hebt Zellen hervor, die vollständig leer sind. |
| [CONTAINS_ERRORS](#CONTAINS-ERRORS) | Diese bedingte Formatierungsregel hebt Zellen mit Formelfehlern hervor. |
| [CONTAINS_TEXT](#CONTAINS-TEXT) | Diese bedingte Formatierungsregel hebt Zellen hervor, die den angegebenen Text enthalten. |
| [DATA_BAR](#DATA-BAR) | Diese bedingte Formatierungsregel zeigt eine abgestufte Datenleiste im Zellbereich an. |
| [DUPLICATE_VALUES](#DUPLICATE-VALUES) | Diese bedingte Formatierungsregel hebt doppelte Werte hervor. |
| [ENDS_WITH](#ENDS-WITH) | Diese bedingte Formatierungsregel hebt Zellen hervor, die mit dem angegebenen Text enden. |
| [EXPRESSION](#EXPRESSION) | Diese bedingte Formatierungsregel enthält eine zu bewertende Formel. |
| [ICON_SET](#ICON-SET) | Diese bedingte Formatierungsregel wendet Symbole auf Zellen gemäß ihren Werten an. |
| [NOT_CONTAINS_BLANKS](#NOT-CONTAINS-BLANKS) | Diese bedingte Formatierungsregel hebt Zellen hervor, die nicht leer sind. |
| [NOT_CONTAINS_ERRORS](#NOT-CONTAINS-ERRORS) | Diese bedingte Formatierungsregel hebt Zellen ohne Formelfehler hervor. |
| [NOT_CONTAINS_TEXT](#NOT-CONTAINS-TEXT) | Diese bedingte Formatierungsregel hebt Zellen hervor, die den angegebenen Text nicht enthalten. |
| [TIME_PERIOD](#TIME-PERIOD) | Diese bedingte Formatierungsregel hebt Zellen hervor, die Daten im angegebenen Zeitraum enthalten. |
| [TOP_10](#TOP-10) | Diese bedingte Formatierungsregel hebt Zellen hervor, deren Werte in das obere N‑ oder untere N‑Intervall fallen, wie angegeben. |
| [UNIQUE_VALUES](#UNIQUE-VALUES) | Diese bedingte Formatierungsregel hebt eindeutige Werte im Bereich hervor. |
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
### ABOVE_AVERAGE {#ABOVE-AVERAGE}
```
public static final int ABOVE_AVERAGE
```


Diese bedingte Formatierungsregel hebt Zellen hervor, die über oder unter dem Durchschnitt aller Werte im Bereich liegen.

### BEGINS_WITH {#BEGINS-WITH}
```
public static final int BEGINS_WITH
```


Diese bedingte Formatierungsregel hebt Zellen im Bereich hervor, die mit dem angegebenen Text beginnen. Entspricht der Verwendung der LEFT()-Tabellenfunktion und dem Vergleich von Werten.

### CELL_VALUE {#CELL-VALUE}
```
public static final int CELL_VALUE
```


Diese bedingte Formatierungsregel vergleicht einen Zellenwert mit einem durch eine Formel berechneten Ergebnis unter Verwendung eines Operators.

### COLOR_SCALE {#COLOR-SCALE}
```
public static final int COLOR_SCALE
```


Diese bedingte Formatierungsregel erstellt eine abgestufte Farbskala für die Zellen.

### CONTAINS_BLANKS {#CONTAINS-BLANKS}
```
public static final int CONTAINS_BLANKS
```


Diese bedingte Formatierungsregel hebt Zellen hervor, die vollständig leer sind. Entspricht der Verwendung von LEN(TRIM()). Das bedeutet, dass wenn die Zelle nur Zeichen enthält, die TRIM() entfernen würde, sie als leer gilt. Eine leere Zelle wird ebenfalls als leer betrachtet.

### CONTAINS_ERRORS {#CONTAINS-ERRORS}
```
public static final int CONTAINS_ERRORS
```


Diese bedingte Formatierungsregel hebt Zellen mit Formelfehlern hervor. Entspricht der Verwendung der ISERROR()-Tabellenfunktion, um zu bestimmen, ob ein Formelfehler vorliegt.

### CONTAINS_TEXT {#CONTAINS-TEXT}
```
public static final int CONTAINS_TEXT
```


Diese bedingte Formatierungsregel hebt Zellen hervor, die den angegebenen Text enthalten. Entspricht der Verwendung der SEARCH()-Tabellenfunktion, um zu bestimmen, ob die Zelle den Text enthält.

### DATA_BAR {#DATA-BAR}
```
public static final int DATA_BAR
```


Diese bedingte Formatierungsregel zeigt eine abgestufte Datenleiste im Zellbereich an.

### DUPLICATE_VALUES {#DUPLICATE-VALUES}
```
public static final int DUPLICATE_VALUES
```


Diese bedingte Formatierungsregel hebt doppelte Werte hervor.

### ENDS_WITH {#ENDS-WITH}
```
public static final int ENDS_WITH
```


Diese bedingte Formatierungsregel hebt Zellen hervor, die mit dem angegebenen Text enden. Entspricht der Verwendung der RIGHT()-Tabellenfunktion und dem Vergleich von Werten.

### EXPRESSION {#EXPRESSION}
```
public static final int EXPRESSION
```


Diese bedingte Formatierungsregel enthält eine zu bewertende Formel. Wenn das Formelresultat wahr ist, wird die Zelle hervorgehoben.

### ICON_SET {#ICON-SET}
```
public static final int ICON_SET
```


Diese bedingte Formatierungsregel wendet Symbole auf Zellen gemäß ihren Werten an.

### NOT_CONTAINS_BLANKS {#NOT-CONTAINS-BLANKS}
```
public static final int NOT_CONTAINS_BLANKS
```


Diese bedingte Formatierungsregel hebt Zellen hervor, die nicht leer sind. Entspricht der Verwendung von LEN(TRIM()). Das bedeutet, dass wenn die Zelle nur Zeichen enthält, die TRIM() entfernen würde, sie als leer gilt. Eine leere Zelle wird ebenfalls als leer betrachtet.

### NOT_CONTAINS_ERRORS {#NOT-CONTAINS-ERRORS}
```
public static final int NOT_CONTAINS_ERRORS
```


Diese bedingte Formatierungsregel hebt Zellen ohne Formelfehler hervor. Entspricht der Verwendung der ISERROR()-Tabellenfunktion, um zu bestimmen, ob ein Formelfehler vorliegt.

### NOT_CONTAINS_TEXT {#NOT-CONTAINS-TEXT}
```
public static final int NOT_CONTAINS_TEXT
```


Diese bedingte Formatierungsregel hebt Zellen hervor, die den angegebenen Text nicht enthalten. Entspricht der Verwendung der SEARCH()-Tabellenfunktion, um zu bestimmen, ob die Zelle den Text enthält oder nicht.

### TIME_PERIOD {#TIME-PERIOD}
```
public static final int TIME_PERIOD
```


Diese bedingte Formatierungsregel hebt Zellen hervor, die Daten im angegebenen Zeitraum enthalten. Der zugrunde liegende Wert der Zelle wird ausgewertet, daher muss die Zelle nicht als Datum formatiert sein, um ausgewertet zu werden. Zum Beispiel wird bei einer Zelle mit dem Wert 38913 das bedingte Format angewendet, wenn die Regel einen Wert von 14.07.2006 erfordert.

### TOP_10 {#TOP-10}
```
public static final int TOP_10
```


Diese bedingte Formatierungsregel hebt Zellen hervor, deren Werte in das obere N‑ oder untere N‑Intervall fallen, wie angegeben.

### UNIQUE_VALUES {#UNIQUE-VALUES}
```
public static final int UNIQUE_VALUES
```


Diese bedingte Formatierungsregel hebt eindeutige Werte im Bereich hervor.

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

