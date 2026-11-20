---
title: "PivotTableRefreshOption"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Optionen zum Aktualisieren der Datenquelle der PivotTable dar."
type: docs
url: /de/java/com.aspose.cells/pivottablerefreshoption/
---

**Inheritance:**
java.lang.Object
```
public class PivotTableRefreshOption
```

Stellt die Optionen zum Aktualisieren der Datenquelle der PivotTable dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [PivotTableRefreshOption()](#PivotTableRefreshOption--) | Stellt die Optionen zum Aktualisieren der Datenquelle der PivotTable dar. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getKeepCachedLocalGroupData()](#getKeepCachedLocalGroupData--) | Gibt an, ob zwischengespeicherte lokale Gruppendaten beibehalten werden sollen, wenn die maximalen und minimalen Werte unverändert bleiben. |
| [getReserveMissingPivotItemType()](#getReserveMissingPivotItemType--) | Stellt dar, wie fehlende Pivot-Elemente reserviert werden. |
| [hashCode()](#hashCode--) |  |
| [isKeepOriginalOrder()](#isKeepOriginalOrder--) | Gibt an, ob die ursprüngliche Reihenfolge der Pivot-Elemente wie bei der alten Datenquelle beibehalten wird. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setKeepCachedLocalGroupData(boolean value)](#setKeepCachedLocalGroupData-boolean-) | Gibt an, ob zwischengespeicherte lokale Gruppendaten beibehalten werden sollen, wenn die maximalen und minimalen Werte unverändert bleiben. |
| [setKeepOriginalOrder(boolean value)](#setKeepOriginalOrder-boolean-) | Gibt an, ob die ursprüngliche Reihenfolge der Pivot-Elemente wie bei der alten Datenquelle beibehalten wird. |
| [setReserveMissingPivotItemType(int value)](#setReserveMissingPivotItemType-int-) | Stellt dar, wie fehlende Pivot-Elemente reserviert werden. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotTableRefreshOption() {#PivotTableRefreshOption--}
```
public PivotTableRefreshOption()
```


Stellt die Optionen zum Aktualisieren der Datenquelle der PivotTable dar.

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
### getKeepCachedLocalGroupData() {#getKeepCachedLocalGroupData--}
```
public boolean getKeepCachedLocalGroupData()
```


Gibt an, ob zwischengespeicherte lokale Gruppendaten beibehalten werden sollen, wenn die maximalen und minimalen Werte unverändert bleiben. Der Standardwert ist false, was bedeutet, dass die Gruppe mit lokaler Einstellung aktualisiert wird.

**Remarks**

Dies ist eine vorübergehende Lösung, bitte lokalisieren Sie Pivot-Tabellen, indem Sie [PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings) implementieren.

**Returns:**
boolean
### getReserveMissingPivotItemType() {#getReserveMissingPivotItemType--}
```
public int getReserveMissingPivotItemType()
```


Stellt dar, wie fehlende Pivot-Elemente reserviert werden.

Siehe [ReserveMissingPivotItemType](../../com.aspose.cells/reservemissingpivotitemtype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isKeepOriginalOrder() {#isKeepOriginalOrder--}
```
public boolean isKeepOriginalOrder()
```


Gibt an, ob die ursprüngliche Reihenfolge der Pivot-Elemente wie bei der alten Datenquelle beibehalten wird.

**Remarks**

Nur anwendbar für das Pivot-Feld, das nicht sortiert ist. Beim Aktualisieren eines solchen Pivot-Feldes behält Ms Excel die ursprüngliche Reihenfolge der alten Datenquelle bei. Der Standardwert dieser Eigenschaft ist true, was das gleiche Verhalten wie bei Ms Excel darstellt. Wenn der Benutzer das Pivot-Feld vollständig wie die Daten in der neuen Datenquelle aktualisieren möchte, sollte diese Eigenschaft auf false gesetzt werden.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setKeepCachedLocalGroupData(boolean value) {#setKeepCachedLocalGroupData-boolean-}
```
public void setKeepCachedLocalGroupData(boolean value)
```


Gibt an, ob zwischengespeicherte lokale Gruppendaten beibehalten werden sollen, wenn die maximalen und minimalen Werte unverändert bleiben. Der Standardwert ist false, was bedeutet, dass die Gruppe mit lokaler Einstellung aktualisiert wird.

**Remarks**

Dies ist eine vorübergehende Lösung, bitte lokalisieren Sie Pivot-Tabellen, indem Sie [PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings) implementieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setKeepOriginalOrder(boolean value) {#setKeepOriginalOrder-boolean-}
```
public void setKeepOriginalOrder(boolean value)
```


Gibt an, ob die ursprüngliche Reihenfolge der Pivot-Elemente wie bei der alten Datenquelle beibehalten wird.

**Remarks**

Nur anwendbar für das Pivot-Feld, das nicht sortiert ist. Beim Aktualisieren eines solchen Pivot-Feldes behält Ms Excel die ursprüngliche Reihenfolge der alten Datenquelle bei. Der Standardwert dieser Eigenschaft ist true, was das gleiche Verhalten wie bei Ms Excel darstellt. Wenn der Benutzer das Pivot-Feld vollständig wie die Daten in der neuen Datenquelle aktualisieren möchte, sollte diese Eigenschaft auf false gesetzt werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setReserveMissingPivotItemType(int value) {#setReserveMissingPivotItemType-int-}
```
public void setReserveMissingPivotItemType(int value)
```


Stellt dar, wie fehlende Pivot-Elemente reserviert werden.

Siehe [ReserveMissingPivotItemType](../../com.aspose.cells/reservemissingpivotitemtype).

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

