---
title: "CalculationCell"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die für die Berechnung relevanten Daten einer Zelle dar, die gerade berechnet wird."
type: docs
url: /de/java/com.aspose.cells/calculationcell/
---

**Inheritance:**
java.lang.Object
```
public class CalculationCell
```

Stellt die für die Berechnung relevanten Daten einer Zelle dar, die gerade berechnet wird.

**Remarks**

Der Benutzer sollte während des Formelbeurteilungsprozesses keine Daten in der Arbeitsmappe ändern, da sonst unerwartete Ergebnisse oder Ausnahmen auftreten können. Daher dienen alle von dieser Klasse bereitgestellten Objekte (wie das Zellobjekt von [getCell()](../../com.aspose.cells/calculationcell\#getCell--)) ausschließlich dem "Lese"‑Zweck.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCell()](#getCell--) | Liest das Zellobjekt, das berechnet wird. |
| [getCellColumn()](#getCellColumn--) | Ermittelt den Spaltenindex der Zelle. |
| [getCellRow()](#getCellRow--) | Ermittelt den Zeilenindex der Zelle. |
| [getClass()](#getClass--) |  |
| [getWorkbook()](#getWorkbook--) | Liest das Arbeitsmappen‑Objekt. |
| [getWorksheet()](#getWorksheet--) | Liest das Arbeitsblatt‑Objekt, in dem sich die Zelle befindet. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalculatedValue(Object v)](#setCalculatedValue-java.lang.Object-) | Setzt den berechneten Wert für die Zelle. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getCell() {#getCell--}
```
public Cell getCell()
```


Liest das Zellobjekt, das berechnet wird.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getCellColumn() {#getCellColumn--}
```
public int getCellColumn()
```


Ermittelt den Spaltenindex der Zelle.

**Returns:**
int
### getCellRow() {#getCellRow--}
```
public int getCellRow()
```


Ermittelt den Zeilenindex der Zelle.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Liest das Arbeitsmappen‑Objekt.

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Liest das Arbeitsblatt‑Objekt, in dem sich die Zelle befindet.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
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




### setCalculatedValue(Object v) {#setCalculatedValue-java.lang.Object-}
```
public void setCalculatedValue(Object v)
```


Setzt den berechneten Wert für die Zelle.

**Remarks**

Der Benutzer kann das berechnete Ergebnis mit dieser Methode festlegen, um die automatische Berechnung für die Zelle zu ignorieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| v | java.lang.Object |  |

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

