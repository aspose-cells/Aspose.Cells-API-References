---
title: "PivotTableCalculateOption"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Optionen zur Berechnung von Daten der PivotTable dar."
type: docs
url: /de/java/com.aspose.cells/pivottablecalculateoption/
---

**Inheritance:**
java.lang.Object
```
public class PivotTableCalculateOption
```

Stellt die Optionen zur Berechnung von Daten der PivotTable dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [PivotTableCalculateOption()](#PivotTableCalculateOption--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getRefreshCharts()](#getRefreshCharts--) | Gibt an, ob das Aktualisieren von Diagrammen auf dieser Pivot‑Tabelle basiert. |
| [getRefreshData()](#getRefreshData--) | Gibt an, ob die Datenquelle der Pivot‑Tabelle aktualisiert wird. |
| [getRefreshOption()](#getRefreshOption--) | Ruft Optionen zum Aktualisieren der Datenquelle in den Pivot‑Cache ab. |
| [getReserveMissingPivotItemType()](#getReserveMissingPivotItemType--) | Stellt dar, wie fehlende Pivot-Elemente reserviert werden. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setRefreshCharts(boolean value)](#setRefreshCharts-boolean-) | Gibt an, ob das Aktualisieren von Diagrammen auf dieser Pivot‑Tabelle basiert. |
| [setRefreshData(boolean value)](#setRefreshData-boolean-) | Gibt an, ob die Datenquelle der Pivot‑Tabelle aktualisiert wird. |
| [setRefreshOption(PivotTableRefreshOption value)](#setRefreshOption-com.aspose.cells.PivotTableRefreshOption-) | Legt Optionen zum Aktualisieren der Datenquelle in den Pivot‑Cache fest. |
| [setReserveMissingPivotItemType(int value)](#setReserveMissingPivotItemType-int-) | Stellt dar, wie fehlende Pivot-Elemente reserviert werden. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotTableCalculateOption() {#PivotTableCalculateOption--}
```
public PivotTableCalculateOption()
```


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
### getRefreshCharts() {#getRefreshCharts--}
```
public boolean getRefreshCharts()
```


Gibt an, ob das Aktualisieren von Diagrammen auf dieser Pivot‑Tabelle basiert.

**Returns:**
boolean
### getRefreshData() {#getRefreshData--}
```
public boolean getRefreshData()
```


Gibt an, ob die Datenquelle der Pivot‑Tabelle aktualisiert wird.

**Remarks**

Wenn wahr, wird der Pivot‑Cache aus der Datenquelle aktualisiert und anschließend alle Pivot‑Tabellen basierend auf demselben Pivot‑Cache berechnet.

**Returns:**
boolean
### getRefreshOption() {#getRefreshOption--}
```
public PivotTableRefreshOption getRefreshOption()
```


Ruft Optionen zum Aktualisieren der Datenquelle in den Pivot‑Cache ab.

**Returns:**
[PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption)
### getReserveMissingPivotItemType() {#getReserveMissingPivotItemType--}
```
public int getReserveMissingPivotItemType()
```


Stellt dar, wie fehlende Pivot-Elemente reserviert werden.

Siehe [ReserveMissingPivotItemType](../../com.aspose.cells/reservemissingpivotitemtype).

**Remarks**

Funktioniert nur, wenn [getRefreshData()](../../com.aspose.cells/pivottablecalculateoption\#getRefreshData--) wahr ist.

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




### setRefreshCharts(boolean value) {#setRefreshCharts-boolean-}
```
public void setRefreshCharts(boolean value)
```


Gibt an, ob das Aktualisieren von Diagrammen auf dieser Pivot‑Tabelle basiert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setRefreshData(boolean value) {#setRefreshData-boolean-}
```
public void setRefreshData(boolean value)
```


Gibt an, ob die Datenquelle der Pivot‑Tabelle aktualisiert wird.

**Remarks**

Wenn wahr, wird der Pivot‑Cache aus der Datenquelle aktualisiert und anschließend alle Pivot‑Tabellen basierend auf demselben Pivot‑Cache berechnet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setRefreshOption(PivotTableRefreshOption value) {#setRefreshOption-com.aspose.cells.PivotTableRefreshOption-}
```
public void setRefreshOption(PivotTableRefreshOption value)
```


Legt Optionen zum Aktualisieren der Datenquelle in den Pivot‑Cache fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) |  |

### setReserveMissingPivotItemType(int value) {#setReserveMissingPivotItemType-int-}
```
public void setReserveMissingPivotItemType(int value)
```


Stellt dar, wie fehlende Pivot-Elemente reserviert werden.

Siehe [ReserveMissingPivotItemType](../../com.aspose.cells/reservemissingpivotitemtype).

**Remarks**

Funktioniert nur, wenn [getRefreshData()](../../com.aspose.cells/pivottablecalculateoption\#getRefreshData--) wahr ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

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

