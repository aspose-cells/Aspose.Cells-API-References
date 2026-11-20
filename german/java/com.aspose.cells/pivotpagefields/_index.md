---
title: "PivotPageFields"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Pivot‑Seiten‑Elemente dar, wenn die Datenquelle der Pivot‑Tabelle Konsolidierungsbereiche ist."
type: docs
url: /de/java/com.aspose.cells/pivotpagefields/
---

**Inheritance:**
java.lang.Object
```
public class PivotPageFields
```

Stellt die Pivot‑Seiten‑Elemente dar, wenn die Datenquelle der Pivot‑Tabelle Konsolidierungsbereiche ist. Sie kann höchstens 4 Elemente enthalten.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [PivotPageFields()](#PivotPageFields--) | Stellt die Pivot‑Seiten‑Feld‑Elemente dar. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [addIdentify(int rangeIndex, int[] pageItemIndex)](#addIdentify-int-int---) | Legt fest, welche Elementbezeichnung in jedem Seitenfeld verwendet wird, um den Datenbereich zu identifizieren. |
| [addPageField(String[] pageItems)](#addPageField-java.lang.String---) | Fügt ein Seitenfeld hinzu. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPageFieldCount()](#getPageFieldCount--) | Ermittelt die Anzahl der Seitenfelder. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotPageFields() {#PivotPageFields--}
```
public PivotPageFields()
```


Stellt die Pivot‑Seiten‑Feld‑Elemente dar.

### addIdentify(int rangeIndex, int[] pageItemIndex) {#addIdentify-int-int---}
```
public void addIdentify(int rangeIndex, int[] pageItemIndex)
```


Legt fest, welche Elementbezeichnung in jedem Seitenfeld verwendet wird, um den Datenbereich zu identifizieren. pageItemIndex.Length muss gleich PageFieldCount sein, bitte fügen Sie zuerst das Seitenfeld hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rangeIndex | int | Der Index des Konsolidierungsdatenbereichs. |
| pageItemIndex | int[] | Der Index des Seitenelements in jedem Seitenfeld. pageItemIndex[2] = 1 bedeutet, dass das zweite Element im dritten Feld verwendet wird, um diesen Bereich zu identifizieren. pageItemIndex[1] = -1 bedeutet, dass kein Element im zweiten Feld verwendet wird, um diesen Bereich zu identifizieren, und MS wird automatisch ein "blank" Element im zweiten Feld erstellen, um diesen Bereich zu identifizieren. |

### addPageField(String[] pageItems) {#addPageField-java.lang.String---}
```
public void addPageField(String[] pageItems)
```


Fügt ein Seitenfeld hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pageItems | java.lang.String[] | Bezeichnung des Seitenfeld‑Elements |

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
### getPageFieldCount() {#getPageFieldCount--}
```
public int getPageFieldCount()
```


Ermittelt die Anzahl der Seitenfelder.

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

