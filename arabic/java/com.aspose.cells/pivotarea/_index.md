---
title: "PivotArea"
second_title: "Aspose.Cells for Java API Reference"
description: "يعرض المنطقة المحددة من جدول المحور."
type: docs
url: /ar/java/com.aspose.cells/pivotarea/
---

**Inheritance:**
java.lang.Object
```
public class PivotArea
```

يعرض المنطقة المحددة من جدول المحور.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [PivotArea(PivotTable table)](#PivotArea-com.aspose.cells.PivotTable-) | يعرض المنطقة المحددة من PivotTable. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAxisType()](#getAxisType--) | يحصل على نطاق PivotTable الذي تنطبق عليه هذه القاعدة. |
| [getCellAreas()](#getCellAreas--) | يحصل على مناطق الخلايا لهذه PivotArea. |
| [getClass()](#getClass--) |  |
| [getFilters()](#getFilters--) | يحصل على جميع المرشحات لهذه PivotArea. |
| [getOnlyData()](#getOnlyData--) | يشير إلى ما إذا كان يتم اختيار قيم البيانات فقط (في منطقة البيانات للعرض) لتحديد عنصر ولا تشمل تسميات العنصر. |
| [getOnlyLabel()](#getOnlyLabel--) | يشير إلى ما إذا كانت تسميات البيانات فقط لتحديد عنصر مختارة. |
| [getRuleType()](#getRuleType--) | يحصل على نوع قاعدة الاختيار. |
| [hashCode()](#hashCode--) |  |
| [isColumnGrandIncluded()](#isColumnGrandIncluded--) | يشير إلى ما إذا كان إجمالي العمود شاملًا. |
| [isOutline()](#isOutline--) | يشير إلى ما إذا كانت القاعدة تشير إلى منطقة في وضع المخطط. |
| [isRowGrandIncluded()](#isRowGrandIncluded--) | يشير إلى ما إذا كان إجمالي الصف شاملًا. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [select(int axisType, int fieldPosition, int selectionType)](#select-int-int-int-) | حدد المنطقة مع المرشحات. |
| [selectField(int axisType, PivotField field)](#selectField-int-com.aspose.cells.PivotField-) | حدد حقلًا في النطاق كمنطقة. |
| [selectField(int axisType, String fieldName)](#selectField-int-java.lang.String-) | حدد حقلًا في النطاق كمنطقة. |
| [setAxisType(int value)](#setAxisType-int-) | يضبط نطاق PivotTable الذي تنطبق عليه هذه القاعدة. |
| [setColumnGrandIncluded(boolean value)](#setColumnGrandIncluded-boolean-) | يشير إلى ما إذا كان إجمالي العمود شاملًا. |
| [setOnlyData(boolean value)](#setOnlyData-boolean-) | يشير إلى ما إذا كان يتم اختيار قيم البيانات فقط (في منطقة البيانات للعرض) لتحديد عنصر ولا تشمل تسميات العنصر. |
| [setOnlyLabel(boolean value)](#setOnlyLabel-boolean-) | يشير إلى ما إذا كانت تسميات البيانات فقط لتحديد عنصر مختارة. |
| [setOutline(boolean value)](#setOutline-boolean-) | يشير إلى ما إذا كانت القاعدة تشير إلى منطقة في وضع المخطط. |
| [setRowGrandIncluded(boolean value)](#setRowGrandIncluded-boolean-) | يشير إلى ما إذا كان إجمالي الصف شاملًا. |
| [setRuleType(int value)](#setRuleType-int-) | يضبط نوع قاعدة الاختيار. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotArea(PivotTable table) {#PivotArea-com.aspose.cells.PivotTable-}
```
public PivotArea(PivotTable table)
```


يعرض المنطقة المحددة من PivotTable.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| table | [PivotTable](../../com.aspose.cells/pivottable) |  |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAxisType() {#getAxisType--}
```
public int getAxisType()
```


يحصل على نطاق PivotTable الذي تنطبق عليه هذه القاعدة.

انظر [PivotFieldType](../../com.aspose.cells/pivotfieldtype).

**Returns:**
int
### getCellAreas() {#getCellAreas--}
```
public CellArea[] getCellAreas()
```


يحصل على مناطق الخلايا لهذه PivotArea.

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


يحصل على جميع المرشحات لهذه PivotArea.

**Returns:**
[PivotAreaFilterCollection](../../com.aspose.cells/pivotareafiltercollection)
### getOnlyData() {#getOnlyData--}
```
public boolean getOnlyData()
```


يشير إلى ما إذا كان يتم اختيار قيم البيانات فقط (في منطقة البيانات للعرض) لتحديد عنصر ولا تشمل تسميات العنصر.

**Returns:**
boolean
### getOnlyLabel() {#getOnlyLabel--}
```
public boolean getOnlyLabel()
```


يشير إلى ما إذا كانت تسميات البيانات فقط لتحديد عنصر مختارة.

**Returns:**
boolean
### getRuleType() {#getRuleType--}
```
public int getRuleType()
```


يحصل على نوع قاعدة الاختيار.

انظر [PivotAreaType](../../com.aspose.cells/pivotareatype).

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


يشير إلى ما إذا كان إجمالي العمود شاملًا.

**Returns:**
boolean
### isOutline() {#isOutline--}
```
public boolean isOutline()
```


يشير إلى ما إذا كانت القاعدة تشير إلى منطقة في وضع المخطط.

**Returns:**
boolean
### isRowGrandIncluded() {#isRowGrandIncluded--}
```
public boolean isRowGrandIncluded()
```


يشير إلى ما إذا كان إجمالي الصف شاملًا.

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


حدد المنطقة مع المرشحات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). المنطقة في PivotTable التي ينطبق عليها هذه القاعدة. |
| fieldPosition | int | موضع الحقل داخل المحور الذي تنطبق عليه هذه القاعدة. |
| selectionType | int | [PivotTableSelectionType](../../com.aspose.cells/pivottableselectiontype). يحدد ما يمكن تحديده في PivotTable أثناء اختيار منظم. |

### selectField(int axisType, PivotField field) {#selectField-int-com.aspose.cells.PivotField-}
```
public void selectField(int axisType, PivotField field)
```


حدد حقلًا في النطاق كمنطقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). نوع المنطقة. |
| field | [PivotField](../../com.aspose.cells/pivotfield) | حقل Pivot. |

### selectField(int axisType, String fieldName) {#selectField-int-java.lang.String-}
```
public void selectField(int axisType, String fieldName)
```


حدد حقلًا في النطاق كمنطقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). نوع المنطقة. |
| fieldName | java.lang.String | اسم حقل Pivot. |

### setAxisType(int value) {#setAxisType-int-}
```
public void setAxisType(int value)
```


يضبط نطاق PivotTable الذي تنطبق عليه هذه القاعدة.

انظر [PivotFieldType](../../com.aspose.cells/pivotfieldtype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setColumnGrandIncluded(boolean value) {#setColumnGrandIncluded-boolean-}
```
public void setColumnGrandIncluded(boolean value)
```


يشير إلى ما إذا كان إجمالي العمود شاملًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setOnlyData(boolean value) {#setOnlyData-boolean-}
```
public void setOnlyData(boolean value)
```


يشير إلى ما إذا كان يتم اختيار قيم البيانات فقط (في منطقة البيانات للعرض) لتحديد عنصر ولا تشمل تسميات العنصر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setOnlyLabel(boolean value) {#setOnlyLabel-boolean-}
```
public void setOnlyLabel(boolean value)
```


يشير إلى ما إذا كانت تسميات البيانات فقط لتحديد عنصر مختارة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setOutline(boolean value) {#setOutline-boolean-}
```
public void setOutline(boolean value)
```


يشير إلى ما إذا كانت القاعدة تشير إلى منطقة في وضع المخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setRowGrandIncluded(boolean value) {#setRowGrandIncluded-boolean-}
```
public void setRowGrandIncluded(boolean value)
```


يشير إلى ما إذا كان إجمالي الصف شاملًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setRuleType(int value) {#setRuleType-int-}
```
public void setRuleType(int value)
```


يضبط نوع قاعدة الاختيار.

انظر [PivotAreaType](../../com.aspose.cells/pivotareatype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

