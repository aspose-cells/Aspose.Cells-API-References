---
title: "PivotArea"
second_title: "Aspose.Cells för Java API-referens"
description: "Visar det valda området i pivottabellen."
type: docs
url: /sv/java/com.aspose.cells/pivotarea/
---

**Inheritance:**
java.lang.Object
```
public class PivotArea
```

Visar det valda området i pivottabellen.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [PivotArea(PivotTable table)](#PivotArea-com.aspose.cells.PivotTable-) | Visar det valda området i pivottabellen. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAxisType()](#getAxisType--) | Hämtar regionen i pivottabellen som denna regel gäller för. |
| [getCellAreas()](#getCellAreas--) | Hämtar cellområden för detta pivotområde. |
| [getClass()](#getClass--) |  |
| [getFilters()](#getFilters--) | Hämtar alla filter för detta PivotArea. |
| [getOnlyData()](#getOnlyData--) | Anger om endast datavärdena (i dataområdet i vyn) för ett objektval är markerade och inte inkluderar objektetiketterna. |
| [getOnlyLabel()](#getOnlyLabel--) | Anger om endast datalabelerna för ett objektval är markerade. |
| [getRuleType()](#getRuleType--) | Hämtar typen av urvalsregel. |
| [hashCode()](#hashCode--) |  |
| [isColumnGrandIncluded()](#isColumnGrandIncluded--) | Anger om kolumnens totalsumma inkluderas. |
| [isOutline()](#isOutline--) | Anger om regeln hänvisar till ett område som är i konturläge. |
| [isRowGrandIncluded()](#isRowGrandIncluded--) | Anger om radens totalsumma inkluderas. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [select(int axisType, int fieldPosition, int selectionType)](#select-int-int-int-) | Välj området med filter. |
| [selectField(int axisType, PivotField field)](#selectField-int-com.aspose.cells.PivotField-) | Välj ett fält i regionen som ett område. |
| [selectField(int axisType, String fieldName)](#selectField-int-java.lang.String-) | Välj ett fält i regionen som ett område. |
| [setAxisType(int value)](#setAxisType-int-) | Ställer in regionen i pivottabellen som denna regel gäller för. |
| [setColumnGrandIncluded(boolean value)](#setColumnGrandIncluded-boolean-) | Anger om kolumnens totalsumma inkluderas. |
| [setOnlyData(boolean value)](#setOnlyData-boolean-) | Anger om endast datavärdena (i dataområdet i vyn) för ett objektval är markerade och inte inkluderar objektetiketterna. |
| [setOnlyLabel(boolean value)](#setOnlyLabel-boolean-) | Anger om endast datalabelerna för ett objektval är markerade. |
| [setOutline(boolean value)](#setOutline-boolean-) | Anger om regeln hänvisar till ett område som är i konturläge. |
| [setRowGrandIncluded(boolean value)](#setRowGrandIncluded-boolean-) | Anger om radens totalsumma inkluderas. |
| [setRuleType(int value)](#setRuleType-int-) | Ställer in typen av urvalsregel. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotArea(PivotTable table) {#PivotArea-com.aspose.cells.PivotTable-}
```
public PivotArea(PivotTable table)
```


Visar det valda området i pivottabellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| table | [PivotTable](../../com.aspose.cells/pivottable) |  |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAxisType() {#getAxisType--}
```
public int getAxisType()
```


Hämtar regionen i pivottabellen som denna regel gäller för.

Se [PivotFieldType](../../com.aspose.cells/pivotfieldtype).

**Returns:**
int
### getCellAreas() {#getCellAreas--}
```
public CellArea[] getCellAreas()
```


Hämtar cellområden för detta pivotområde.

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


Hämtar alla filter för detta PivotArea.

**Returns:**
[PivotAreaFilterCollection](../../com.aspose.cells/pivotareafiltercollection)
### getOnlyData() {#getOnlyData--}
```
public boolean getOnlyData()
```


Anger om endast datavärdena (i dataområdet i vyn) för ett objektval är markerade och inte inkluderar objektetiketterna.

**Returns:**
boolean
### getOnlyLabel() {#getOnlyLabel--}
```
public boolean getOnlyLabel()
```


Anger om endast datalabelerna för ett objektval är markerade.

**Returns:**
boolean
### getRuleType() {#getRuleType--}
```
public int getRuleType()
```


Hämtar typen av urvalsregel.

Se [PivotAreaType](../../com.aspose.cells/pivotareatype).

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


Anger om kolumnens totalsumma inkluderas.

**Returns:**
boolean
### isOutline() {#isOutline--}
```
public boolean isOutline()
```


Anger om regeln hänvisar till ett område som är i konturläge.

**Returns:**
boolean
### isRowGrandIncluded() {#isRowGrandIncluded--}
```
public boolean isRowGrandIncluded()
```


Anger om radens totalsumma inkluderas.

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


Välj området med filter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Regionen i pivottabellen som denna regel gäller för. |
| fieldPosition | int | Fältets position inom axeln som denna regel gäller för. |
| selectionType | int | [PivotTableSelectionType](../../com.aspose.cells/pivottableselectiontype). Anger vad som kan väljas i en pivottabell under en strukturerad markering. |

### selectField(int axisType, PivotField field) {#selectField-int-com.aspose.cells.PivotField-}
```
public void selectField(int axisType, PivotField field)
```


Välj ett fält i regionen som ett område.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Regionstypen. |
| field | [PivotField](../../com.aspose.cells/pivotfield) | Pivottfältet. |

### selectField(int axisType, String fieldName) {#selectField-int-java.lang.String-}
```
public void selectField(int axisType, String fieldName)
```


Välj ett fält i regionen som ett område.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). Regionstypen. |
| fieldName | java.lang.String | Namnet på pivottfältet. |

### setAxisType(int value) {#setAxisType-int-}
```
public void setAxisType(int value)
```


Ställer in regionen i pivottabellen som denna regel gäller för.

Se [PivotFieldType](../../com.aspose.cells/pivotfieldtype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setColumnGrandIncluded(boolean value) {#setColumnGrandIncluded-boolean-}
```
public void setColumnGrandIncluded(boolean value)
```


Anger om kolumnens totalsumma inkluderas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setOnlyData(boolean value) {#setOnlyData-boolean-}
```
public void setOnlyData(boolean value)
```


Anger om endast datavärdena (i dataområdet i vyn) för ett objektval är markerade och inte inkluderar objektetiketterna.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setOnlyLabel(boolean value) {#setOnlyLabel-boolean-}
```
public void setOnlyLabel(boolean value)
```


Anger om endast datalabelerna för ett objektval är markerade.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setOutline(boolean value) {#setOutline-boolean-}
```
public void setOutline(boolean value)
```


Anger om regeln hänvisar till ett område som är i konturläge.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setRowGrandIncluded(boolean value) {#setRowGrandIncluded-boolean-}
```
public void setRowGrandIncluded(boolean value)
```


Anger om radens totalsumma inkluderas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setRuleType(int value) {#setRuleType-int-}
```
public void setRuleType(int value)
```


Ställer in typen av urvalsregel.

Se [PivotAreaType](../../com.aspose.cells/pivotareatype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

