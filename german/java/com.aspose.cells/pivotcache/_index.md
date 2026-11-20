---
title: "PivotCache"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt den Speicher-Cache für einige PivotTable-Berichte dar."
type: docs
url: /de/java/com.aspose.cells/pivotcache/
---

**Inheritance:**
java.lang.Object
```
public abstract class PivotCache
```

Stellt den Speicher-Cache für einige PivotTable-Berichte dar.

**Remarks**

Alle Daten werden in diesen Cache gesammelt, und die Pivot‑Tabelle ruft Daten nur aus diesem Cache ab, nicht direkt aus der Datenquelle. Wenn die Datenquelle einiger [PivotTable](../../com.aspose.cells/pivottable)s identisch ist, verwenden sie denselben Pivot‑Cache.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [PivotCache()](#PivotCache--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [dispose()](#dispose--) | Alle Ressourcen freigeben. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getMissingItemsLimit()](#getMissingItemsLimit--) | Ermittelt die Anzahl nicht verwendeter Elemente, die zulässig sind, bevor nicht verwendete Elemente verworfen werden. |
| [getPivotTables()](#getPivotTables--) | Ermittelt alle Pivot‑Tabellen mit diesem Pivot‑Cache. |
| [getSourceType()](#getSourceType--) | Ermittelt den [PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype). |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | Aktualisiert Daten aus der Datenquelle und berechnet Daten für die Ansicht aller Pivot‑Tabellen, deren Datenquelle dieser Pivot‑Cache ist. |
| [refresh(PivotTableRefreshOption option)](#refresh-com.aspose.cells.PivotTableRefreshOption-) | Aktualisiert Daten aus der Datenquelle und berechnet Daten für die Ansicht aller Pivot‑Tabellen, deren Datenquelle dieser Pivot‑Cache ist. |
| [setMissingItemsLimit(int value)](#setMissingItemsLimit-int-) | Legt die Anzahl nicht verwendeter Elemente fest, die zulässig sind, bevor nicht verwendete Elemente verworfen werden. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotCache() {#PivotCache--}
```
public PivotCache()
```


### dispose() {#dispose--}
```
public abstract void dispose()
```


Alle Ressourcen freigeben.

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
### getMissingItemsLimit() {#getMissingItemsLimit--}
```
public int getMissingItemsLimit()
```


Ermittelt die Anzahl nicht verwendeter Elemente, die zulässig sind, bevor nicht verwendete Elemente verworfen werden. Dieser Wert MUSS größer als -2 und kleiner als 1048577 sein. [PivotCacheMissingItemsLimitConst](../../com.aspose.cells/pivotcachemissingitemslimitconst);

**Returns:**
int
### getPivotTables() {#getPivotTables--}
```
public PivotTable[] getPivotTables()
```


Ermittelt alle Pivot‑Tabellen mit diesem Pivot‑Cache.

**Returns:**
com.aspose.cells.PivotTable[] -
### getSourceType() {#getSourceType--}
```
public abstract byte getSourceType()
```


Ermittelt den [PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype).

Siehe [PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype).

**Returns:**
byte
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




### refresh() {#refresh--}
```
public int refresh()
```


Aktualisiert Daten aus der Datenquelle und berechnet Daten für die Ansicht aller Pivot‑Tabellen, deren Datenquelle dieser Pivot‑Cache ist.

**Remarks**

Wenn sowohl table1 als auch table2 diesen Cache verwenden, werden beide Tabellen berechnet. Es ist besser, wenn Sie einfach [Workbook.refreshAll()](../../com.aspose.cells/workbook\#refreshAll--) aufrufen, um alle Pivot‑Tabellen und Diagramme in der Datei zu aktualisieren.

**Returns:**
int
### refresh(PivotTableRefreshOption option) {#refresh-com.aspose.cells.PivotTableRefreshOption-}
```
public int refresh(PivotTableRefreshOption option)
```


Aktualisiert Daten aus der Datenquelle und berechnet Daten für die Ansicht aller Pivot‑Tabellen, deren Datenquelle dieser Pivot‑Cache ist.

**Remarks**

Es ist besser, wenn Sie einfach [Workbook.refreshAll()](../../com.aspose.cells/workbook\#refreshAll--) aufrufen, um alle Pivot‑Tabellen und Diagramme in der Datei zu aktualisieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | Die Optionen zum Aktualisieren der Datenquelle der Pivot‑Tabelle. |

**Returns:**
int
### setMissingItemsLimit(int value) {#setMissingItemsLimit-int-}
```
public void setMissingItemsLimit(int value)
```


Legt die Anzahl nicht verwendeter Elemente fest, die zulässig sind, bevor nicht verwendete Elemente verworfen werden. Dieser Wert MUSS größer als -2 und kleiner als 1048577 sein. [PivotCacheMissingItemsLimitConst](../../com.aspose.cells/pivotcachemissingitemslimitconst);

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

