---
title: "CalculationPrecisionStrategy"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Enumeriert Strategien zum Umgang mit Berechnungsgenauigkeit."
type: docs
url: /de/java/com.aspose.cells/calculationprecisionstrategy/
---

**Inheritance:**
java.lang.Object
```
public final class CalculationPrecisionStrategy
```

Enumeriert Strategien zur Handhabung der Berechnungsgenauigkeit. Aufgrund des Präzisionsproblems der IEEE‑754‑Gleitkommaarithmetik können einige "scheinbar einfache" Formeln nicht das erwartete Ergebnis liefern. Zum Beispiel die Formel "=-0.45+0.43+0.02"; wenn die Operanden direkt mit dem '+'‑Operator berechnet werden, ist das Ergebnis nicht null. Für solche Präzisionsprobleme können spezielle Strategien das erwartete Ergebnis liefern.
## Felder

| Feld | Beschreibung |
| --- | --- |
| [DECIMAL](#DECIMAL) | Verwendet Dezimalzahlen als Operanden, wenn möglich. |
| [NONE](#NONE) | Keine Strategie bei der Berechnung angewendet. |
| [ROUND](#ROUND) | Rundet das Berechnungsergebnis gemäß signifikanten Stellen. |
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
### DECIMAL {#DECIMAL}
```
public static final int DECIMAL
```


Verwendet Dezimalzahlen als Operanden, wenn möglich. Am ineffizientesten für die Leistung.

### NONE {#NONE}
```
public static final int NONE
```


Keine Strategie bei der Berechnung angewendet. Beim Berechnen wird einfach der ursprüngliche double‑Wert als Operand verwendet und das Ergebnis direkt zurückgegeben. Am effizientesten für die Leistung und in den meisten Fällen anwendbar.

### ROUND {#ROUND}
```
public static final int ROUND
```


Rundet das Berechnungsergebnis gemäß signifikanten Stellen.

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

