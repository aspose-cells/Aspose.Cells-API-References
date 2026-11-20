---
title: "PivotArea"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt den ausgewählten Bereich der Pivot-Tabelle dar."
type: docs
url: /de/java/com.aspose.cells/pivotarea/
---

**Inheritance:**
java.lang.Object
```
public class PivotArea
```

Stellt den ausgewählten Bereich der Pivot-Tabelle dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [PivotArea(PivotTable table)](#PivotArea-com.aspose.cells.PivotTable-) | Stellt den ausgewählten Bereich der PivotTable dar. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAxisType()](#getAxisType--) | Ruft den Bereich der PivotTable ab, auf den diese Regel zutrifft. |
| [getCellAreas()](#getCellAreas--) | Ruft die Zellbereiche dieses Pivot-Bereichs ab. |
| [getClass()](#getClass--) |  |
| [getFilters()](#getFilters--) | Ruft alle Filter für diesen PivotArea ab. |
| [getOnlyData()](#getOnlyData--) | Gibt an, ob nur die Datenwerte (im Datenbereich der Ansicht) für eine Elementauswahl ausgewählt sind und die Elementbeschriftungen nicht enthalten. |
| [getOnlyLabel()](#getOnlyLabel--) | Gibt an, ob nur die Datenbeschriftungen für eine Elementauswahl ausgewählt sind. |
| [getRuleType()](#getRuleType--) | Ruft den Typ der Auswahlregel ab. |
| [hashCode()](#hashCode--) |  |
| [isColumnGrandIncluded()](#isColumnGrandIncluded--) | Gibt an, ob die Gesamtsumme der Spalte enthalten ist. |
| [isOutline()](#isOutline--) | Gibt an, ob die Regel sich auf einen Bereich bezieht, der im Gliederungsmodus ist. |
| [isRowGrandIncluded()](#isRowGrandIncluded--) | Gibt an, ob die Gesamtsumme der Zeile enthalten ist. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [select(int axisType, int fieldPosition, int selectionType)](#select-int-int-int-) | Wählen Sie den Bereich mit Filtern aus. |
| [selectField(int axisType, PivotField field)](#selectField-int-com.aspose.cells.PivotField-) | Wählen Sie ein Feld im Bereich als Bereich aus. |
| [selectField(int axisType, String fieldName)](#selectField-int-java.lang.String-) | Wählen Sie ein Feld im Bereich als Bereich aus. |
| [setAxisType(int value)](#setAxisType-int-) | Setzt den Bereich der PivotTable, auf den diese Regel zutrifft. |
| [setColumnGrandIncluded(boolean value)](#setColumnGrandIncluded-boolean-) | Gibt an, ob die Gesamtsumme der Spalte enthalten ist. |
| [setOnlyData(boolean value)](#setOnlyData-boolean-) | Gibt an, ob nur die Datenwerte (im Datenbereich der Ansicht) für eine Elementauswahl ausgewählt sind und die Elementbeschriftungen nicht enthalten. |
| [setOnlyLabel(boolean value)](#setOnlyLabel-boolean-) | Gibt an, ob nur die Datenbeschriftungen für eine Elementauswahl ausgewählt sind. |
| [setOutline(boolean value)](#setOutline-boolean-) | Gibt an, ob die Regel sich auf einen Bereich bezieht, der im Gliederungsmodus ist. |
| [setRowGrandIncluded(boolean value)](#setRowGrandIncluded-boolean-) | Gibt an, ob die Gesamtsumme der Zeile enthalten ist. |
| [setRuleType(int value)](#setRuleType-int-) | Setzt den Typ der Auswahlregel. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotArea(PivotTable table) {#PivotArea-com.aspose.cells.PivotTable-}
```
public PivotArea(PivotTable table)
```


Stellt den ausgewählten Bereich der PivotTable dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| table | [PivotTable](../../com.aspose.cells/pivottable) |  |

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
### getAxisType() {#getAxisType--}
```
public int getAxisType()
```


Ruft den Bereich der PivotTable ab, auf den diese Regel zutrifft.

Siehe [PivotFieldType](../../com.aspose.cells/pivotfieldtype).

**Returns:**
int
### getCellAreas() {#getCellAreas--}
```
public CellArea[] getCellAreas()
```


Ruft die Zellbereiche dieses Pivot-Bereichs ab.

**Returns:**
com.aspose.cells.CellArea[] -
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFilters() {#getFilters--}
```
public PivotAreaFilterCollection getFilters()
```


Ruft alle Filter für diesen PivotArea ab.

**Returns:**
[PivotAreaFilterCollection](../../com.aspose.cells/pivotareafiltercollection)
### getOnlyData() {#getOnlyData--}
```
public boolean getOnlyData()
```


Gibt an, ob nur die Datenwerte (im Datenbereich der Ansicht) für eine Elementauswahl ausgewählt sind und die Elementbeschriftungen nicht enthalten.

**Returns:**
boolean
### getOnlyLabel() {#getOnlyLabel--}
```
public boolean getOnlyLabel()
```


Gibt an, ob nur die Datenbeschriftungen für eine Elementauswahl ausgewählt sind.

**Returns:**
boolean
### getRuleType() {#getRuleType--}
```
public int getRuleType()
```


Ruft den Typ der Auswahlregel ab.

Siehe [PivotAreaType](../../com.aspose.cells/pivotareatype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isColumnGrandIncluded() {#isColumnGrandIncluded--}
```
public boolean isColumnGrandIncluded()
```


Gibt an, ob die Gesamtsumme der Spalte enthalten ist.

**Returns:**
boolean
### isOutline() {#isOutline--}
```
public boolean isOutline()
```


Gibt an, ob die Regel sich auf einen Bereich bezieht, der im Gliederungsmodus ist.

**Returns:**
boolean
### isRowGrandIncluded() {#isRowGrandIncluded--}
```
public boolean isRowGrandIncluded()
```


Gibt an, ob die Gesamtsumme der Zeile enthalten ist.

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




### select(int axisType, int fieldPosition, int selectionType) {#select-int-int-int-}
```
public void select(int axisType, int fieldPosition, int selectionType)
```


Wählen Sie den Bereich mit Filtern aus.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Der Bereich der PivotTable, für den diese Regel gilt. |
| fieldPosition | int | Position des Feldes innerhalb der Achse, für die diese Regel gilt. |
| selectionType | int | [PivotTableSelectionType](../../com.aspose.cells/pivottableselectiontype). Gibt an, was in einer PivotTable während einer strukturierten Auswahl ausgewählt werden kann. |

### selectField(int axisType, PivotField field) {#selectField-int-com.aspose.cells.PivotField-}
```
public void selectField(int axisType, PivotField field)
```


Wählen Sie ein Feld im Bereich als Bereich aus.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Der Regionstyp. |
| field | [PivotField](../../com.aspose.cells/pivotfield) | Das Pivot-Feld. |

### selectField(int axisType, String fieldName) {#selectField-int-java.lang.String-}
```
public void selectField(int axisType, String fieldName)
```


Wählen Sie ein Feld im Bereich als Bereich aus.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Der Regionstyp. |
| fieldName | java.lang.String | Der Name des Pivot-Feldes. |

### setAxisType(int value) {#setAxisType-int-}
```
public void setAxisType(int value)
```


Setzt den Bereich der PivotTable, auf den diese Regel zutrifft.

Siehe [PivotFieldType](../../com.aspose.cells/pivotfieldtype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setColumnGrandIncluded(boolean value) {#setColumnGrandIncluded-boolean-}
```
public void setColumnGrandIncluded(boolean value)
```


Gibt an, ob die Gesamtsumme der Spalte enthalten ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setOnlyData(boolean value) {#setOnlyData-boolean-}
```
public void setOnlyData(boolean value)
```


Gibt an, ob nur die Datenwerte (im Datenbereich der Ansicht) für eine Elementauswahl ausgewählt sind und die Elementbeschriftungen nicht enthalten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setOnlyLabel(boolean value) {#setOnlyLabel-boolean-}
```
public void setOnlyLabel(boolean value)
```


Gibt an, ob nur die Datenbeschriftungen für eine Elementauswahl ausgewählt sind.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setOutline(boolean value) {#setOutline-boolean-}
```
public void setOutline(boolean value)
```


Gibt an, ob die Regel sich auf einen Bereich bezieht, der im Gliederungsmodus ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setRowGrandIncluded(boolean value) {#setRowGrandIncluded-boolean-}
```
public void setRowGrandIncluded(boolean value)
```


Gibt an, ob die Gesamtsumme der Zeile enthalten ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setRuleType(int value) {#setRuleType-int-}
```
public void setRuleType(int value)
```


Setzt den Typ der Auswahlregel.

Siehe [PivotAreaType](../../com.aspose.cells/pivotareatype).

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

