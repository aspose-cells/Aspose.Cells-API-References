---
title: "FormatConditionCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل التنسيق الشرطي."
type: docs
url: /ar/java/com.aspose.cells/formatconditioncollection/
---

**Inheritance:**
java.lang.Object
```
public class FormatConditionCollection
```

يمثل التنسيق الشرطي. يمكن أن تحتوي FormatConditions على ما يصل إلى ثلاثة تنسيقات شرطية.

**Example**

```
         //Create a new Workbook.
         Workbook workbook = new Workbook();
 
         //Get the first worksheet.
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Adds an empty conditional formatting
         int index = sheet.getConditionalFormattings().add();
         FormatConditionCollection fcs = sheet.getConditionalFormattings().get(index);
         //Sets the conditional format range.
         CellArea ca = new CellArea();
         ca.StartRow = 0;
         ca.EndRow = 0;
         ca.StartColumn = 0;
         ca.EndColumn = 0;
         fcs.addArea(ca);
         ca = new CellArea();
         ca.StartRow = 1;
         ca.EndRow = 1;
         ca.StartColumn = 1;
         ca.EndColumn = 1;
         fcs.addArea(ca);
         //Adds condition.
         int conditionIndex = fcs.addCondition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "=A2", "100");
         //Adds condition.
         int conditionIndex2 = fcs.addCondition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "50", "100");
         //Sets the background color.
         FormatCondition fc = fcs.get(conditionIndex);
         fc.getStyle().setBackgroundColor(Color.getRed());
         //Saving the Excel file
         workbook.save("output.xls");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(CellArea cellArea, int type, int operatorType, String formula1, String formula2)](#add-com.aspose.cells.CellArea-int-int-java.lang.String-java.lang.String-) | يضيف شرط تنسيق ونطاق الخلايا المتأثر إلى FormatConditions. يمكن أن تحتوي FormatConditions على ما يصل إلى ثلاثة تنسيقات شرطية. |
| [addArea(CellArea cellArea)](#addArea-com.aspose.cells.CellArea-) | يضيف نطاق خلايا منسق بشكل شرطي. |
| [addCondition(int type)](#addCondition-int-) | أضف شرط تنسيق. |
| [addCondition(int type, int operatorType, String formula1, String formula2)](#addCondition-int-int-java.lang.String-java.lang.String-) | يضيف شرط تنسيق. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | يحصل على شرط التنسيق حسب الفهرس. |
| [getCellArea(int index)](#getCellArea-int-) | يحصل على نطاق الخلايا المنسق بشكل شرطي حسب الفهرس. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | يحصل على عدد الشروط. |
| [getRangeCount()](#getRangeCount--) | يحصل على عدد النطاقات المنسقة بشكل شرطي. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeArea(int index)](#removeArea-int-) | يزيل نطاق الخلايا المنسق بشكل شرطي حسب الفهرس. |
| [removeArea(int startRow, int startColumn, int totalRows, int totalColumns)](#removeArea-int-int-int-int-) | إزالة التنسيق الشرطي في النطاق. |
| [removeCondition(int index)](#removeCondition-int-) | يزيل شرط التنسيق حسب الفهرس. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(CellArea cellArea, int type, int operatorType, String formula1, String formula2) {#add-com.aspose.cells.CellArea-int-int-java.lang.String-java.lang.String-}
```
public int[] add(CellArea cellArea, int type, int operatorType, String formula1, String formula2)
```


يضيف شرط تنسيق ونطاق الخلايا المتأثر إلى FormatConditions. يمكن أن يحتوي FormatConditions على ما يصل إلى ثلاثة تنسيقات شرطية. لا يُسمح بالإشارات إلى الأوراق الأخرى في صيغ التنسيق الشرطي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | نطاق خلايا منسق بشكل شرطي. |
| type | int | [FormatConditionType](../../com.aspose.cells/formatconditiontype). نوع التنسيق الشرطي. يمكن أن يكون أحد أعضاء FormatConditionType. |
| operatorType | int | [OperatorType](../../com.aspose.cells/operatortype). عامل المقارنة. يمكن أن يكون أحد أعضاء OperatorType. |
| formula1 | java.lang.String | القيمة أو التعبير المرتبط بالتنسيق الشرطي. |
| formula2 | java.lang.String | القيمة أو التعبير المرتبط بالتنسيق الشرطي |

**Returns:**
int[] - [0]:فهرس كائن شرط التنسيق؛[1] فهرس نطاق الخلية المتأثرة.
### addArea(CellArea cellArea) {#addArea-com.aspose.cells.CellArea-}
```
public int addArea(CellArea cellArea)
```


يضيف نطاق خلايا منسق بشكل شرطي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | نطاق خلايا منسق بشكل شرطي. |

**Returns:**
int - فهرس نطاق الخلية المنسقة بشكل شرطي.
### addCondition(int type) {#addCondition-int-}
```
public int addCondition(int type)
```


أضف شرط تنسيق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [FormatConditionType](../../com.aspose.cells/formatconditiontype). نوع شرط التنسيق. |

**Returns:**
int - فهرس كائن شرط التنسيق؛
### addCondition(int type, int operatorType, String formula1, String formula2) {#addCondition-int-int-java.lang.String-java.lang.String-}
```
public int addCondition(int type, int operatorType, String formula1, String formula2)
```


يضيف شرط تنسيق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [FormatConditionType](../../com.aspose.cells/formatconditiontype). نوع شرط التنسيق. |
| operatorType | int | [OperatorType](../../com.aspose.cells/operatortype). نوع العامل |
| formula1 | java.lang.String | القيمة أو التعبير المرتبط بالتنسيق الشرطي. إذا بدأت القيمة المدخلة بـ '=', فسيتم اعتبارها صيغة. وإلا فسيتم اعتبارها قيمة عادية (نص، رقم، منطق). بالنسبة للقيمة النصية التي تبدأ بـ '=', يمكن للمستخدم إدخالها كصيغة بالتنسيق: "=\\"=...\\"". |
| formula2 | java.lang.String | القيمة أو التعبير المرتبط بالتنسيق الشرطي. تنسيق الإدخال هو نفسه مع formula1 |

**Returns:**
int - فهرس كائن شرط التنسيق؛
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
### get(int index) {#get-int-}
```
public FormatCondition get(int index)
```


يحصل على شرط التنسيق حسب الفهرس.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | فهرس شرط التنسيق للإرجاع. |

**Returns:**
[FormatCondition](../../com.aspose.cells/formatcondition) - the formatting condition
### getCellArea(int index) {#getCellArea-int-}
```
public CellArea getCellArea(int index)
```


يحصل على نطاق الخلايا المنسق بشكل شرطي حسب الفهرس.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | فهرس نطاق الخلايا المُنسَّق شرطيًا. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the conditional formatted cell range
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


يحصل على عدد الشروط.

**Returns:**
int
### getRangeCount() {#getRangeCount--}
```
public int getRangeCount()
```


يحصل على عدد النطاقات المنسقة بشكل شرطي.

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




### removeArea(int index) {#removeArea-int-}
```
public void removeArea(int index)
```


يزيل نطاق الخلايا المنسق بشكل شرطي حسب الفهرس.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | فهرس نطاق الخلايا المُنسَّق شرطيًا الذي سيتم إزالته. |

### removeArea(int startRow, int startColumn, int totalRows, int totalColumns) {#removeArea-int-int-int-int-}
```
public boolean removeArea(int startRow, int startColumn, int totalRows, int totalColumns)
```


إزالة التنسيق الشرطي في النطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | int | صف البداية للنطاق. |
| startColumn | int | عمود البداية للنطاق. |
| totalRows | int | عدد الصفوف في النطاق. |
| totalColumns | int | عدد الأعمدة في النطاق. |

**Returns:**
منطقي - يُرجع TRUE، يجب إزالة هذا FormatCondtionCollection.
### removeCondition(int index) {#removeCondition-int-}
```
public void removeCondition(int index)
```


يزيل شرط التنسيق حسب الفهرس.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | فهرس شرط التنسيق الذي سيتم إزالته. |

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

