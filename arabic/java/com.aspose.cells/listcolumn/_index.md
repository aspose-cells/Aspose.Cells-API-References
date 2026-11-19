---
title: "ListColumn"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل عمودًا في جدول."
type: docs
url: /ar/java/com.aspose.cells/listcolumn/
---

**Inheritance:**
java.lang.Object
```
public class ListColumn
```

يمثل عمودًا في جدول.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         for (int i = 0; i  ? i++)
         {
         cells.get(0,i).putValue(CellsHelper.columnIndexToName(i));
          }
         for (int row = 1; row  ? row++)
         {
          for (int column = 0; column  ? column++)
         {
         cells.get(row, column).putValue(row * column);
          }
          }
         ListObjectCollection tables = workbook.getWorksheets().get(0).getListObjects();
         int index = tables.add(0, 0, 9, 4, true);
         ListObject table = tables.get(0);
         table.setShowTotals(true);
         ListColumn listColumn = table.getListColumns().get(4);
         listColumn.setTotalsCalculation(com.aspose.cells.TotalsCalculation.SUM);
         listColumn.setFormula("=[A]");
         workbook.save("Book1.xlsx");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCustomCalculatedFormula(boolean isR1C1, boolean isLocal)](#getCustomCalculatedFormula-boolean-boolean-) | يحصل على صيغة هذا العمود القائم. |
| [getCustomTotalsRowFormula(boolean isR1C1, boolean isLocal)](#getCustomTotalsRowFormula-boolean-boolean-) | يحصل على صيغة صف الإجماليات لهذا العمود القائم. |
| [getDataStyle()](#getDataStyle--) | يحصل على نمط البيانات في هذا العمود من الجدول. |
| [getFormula()](#getFormula--) | يحصل على صيغة العمود القائم. |
| [getName()](#getName--) | يحصل على اسم العمود. |
| [getRange()](#getRange--) | يحصل على نطاق هذا العمود في القائمة. |
| [getTotalsCalculation()](#getTotalsCalculation--) | يحصل على نوع الحساب في صف الإجماليات للعمود في القائمة. |
| [getTotalsRowLabel()](#getTotalsRowLabel--) | يحصل على تسميات العرض لصف الإجماليات. |
| [hashCode()](#hashCode--) |  |
| [isArrayFormula()](#isArrayFormula--) | يشير إلى ما إذا كانت الـ fomula مصفوفة. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCustomCalculatedFormula(String formula, boolean isR1C1, boolean isLocal)](#setCustomCalculatedFormula-java.lang.String-boolean-boolean-) | يضبط الصيغة لهذا العمود في القائمة. |
| [setCustomTotalsRowFormula(String formula, boolean isR1C1, boolean isLocal)](#setCustomTotalsRowFormula-java.lang.String-boolean-boolean-) | يحصل على صيغة صف الإجماليات لهذا العمود القائم. |
| [setDataStyle(Style style)](#setDataStyle-com.aspose.cells.Style-) | يضبط نمط البيانات في هذا العمود من الجدول. |
| [setFormula(String value)](#setFormula-java.lang.String-) | يضبط صيغة العمود في القائمة. |
| [setName(String value)](#setName-java.lang.String-) | يضبط اسم العمود. |
| [setTotalsCalculation(int value)](#setTotalsCalculation-int-) | يضبط نوع الحساب في صف الإجماليات للعمود في القائمة. |
| [setTotalsRowLabel(String value)](#setTotalsRowLabel-java.lang.String-) | يضبط تسميات العرض لصف الإجماليات. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomCalculatedFormula(boolean isR1C1, boolean isLocal) {#getCustomCalculatedFormula-boolean-boolean-}
```
public String getCustomCalculatedFormula(boolean isR1C1, boolean isLocal)
```


يحصل على صيغة هذا العمود القائم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| isR1C1 | boolean | ما إذا كانت الصيغة تحتاج إلى تنسيق كـ R1C1. |
| isLocal | boolean | ما إذا كانت الصيغة تحتاج إلى تنسيق حسب الإعدادات الإقليمية. |

**Returns:**
java.lang.String - صيغة هذا العمود في القائمة.
### getCustomTotalsRowFormula(boolean isR1C1, boolean isLocal) {#getCustomTotalsRowFormula-boolean-boolean-}
```
public String getCustomTotalsRowFormula(boolean isR1C1, boolean isLocal)
```


يحصل على صيغة صف الإجماليات لهذا العمود القائم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| isR1C1 | boolean | ما إذا كانت الصيغة تحتاج إلى تنسيق كـ R1C1. |
| isLocal | boolean | ما إذا كانت الصيغة تحتاج إلى تنسيق حسب الإعدادات الإقليمية. |

**Returns:**
java.lang.String - صيغة هذا العمود في القائمة.
### getDataStyle() {#getDataStyle--}
```
public Style getDataStyle()
```


يحصل على نمط البيانات في هذا العمود من الجدول.

**Returns:**
[Style](../../com.aspose.cells/style)
### getFormula() {#getFormula--}
```
public String getFormula()
```


يحصل على صيغة العمود القائم.

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


يحصل على اسم العمود.

**Remarks**

إذا تم ضبط اسم العمود، سيتغير قيمة الخلية المقابلة أيضًا.

**Returns:**
java.lang.String
### getRange() {#getRange--}
```
public Range getRange()
```


يحصل على نطاق هذا العمود في القائمة.

**Returns:**
[Range](../../com.aspose.cells/range)
### getTotalsCalculation() {#getTotalsCalculation--}
```
public int getTotalsCalculation()
```


يحصل على نوع الحساب في صف الإجماليات للعمود في القائمة.

انظر [TotalsCalculation](../../com.aspose.cells/totalscalculation).

**Returns:**
int
### getTotalsRowLabel() {#getTotalsRowLabel--}
```
public String getTotalsRowLabel()
```


يحصل على تسميات العرض لصف الإجماليات.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isArrayFormula() {#isArrayFormula--}
```
public boolean isArrayFormula()
```


يشير إلى ما إذا كانت الـ fomula مصفوفة.

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




### setCustomCalculatedFormula(String formula, boolean isR1C1, boolean isLocal) {#setCustomCalculatedFormula-java.lang.String-boolean-boolean-}
```
public void setCustomCalculatedFormula(String formula, boolean isR1C1, boolean isLocal)
```


يضبط الصيغة لهذا العمود في القائمة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| formula | java.lang.String | الصيغة لهذا العمود في القائمة. |
| isR1C1 | boolean | ما إذا كانت الصيغة تحتاج إلى تنسيق كـ R1C1. |
| isLocal | boolean | ما إذا كانت الصيغة تحتاج إلى تنسيق حسب الإعدادات الإقليمية. |

### setCustomTotalsRowFormula(String formula, boolean isR1C1, boolean isLocal) {#setCustomTotalsRowFormula-java.lang.String-boolean-boolean-}
```
public void setCustomTotalsRowFormula(String formula, boolean isR1C1, boolean isLocal)
```


يحصل على صيغة صف الإجماليات لهذا العمود القائم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| formula | java.lang.String | الصيغة لهذا العمود في القائمة. |
| isR1C1 | boolean | ما إذا كانت الصيغة تحتاج إلى تنسيق كـ R1C1. |
| isLocal | boolean | ما إذا كانت الصيغة تحتاج إلى تنسيق حسب الإعدادات الإقليمية. |

### setDataStyle(Style style) {#setDataStyle-com.aspose.cells.Style-}
```
public void setDataStyle(Style style)
```


يضبط نمط البيانات في هذا العمود من الجدول.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) |  |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public void setFormula(String value)
```


يضبط صيغة العمود في القائمة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


يضبط اسم العمود.

**Remarks**

إذا تم ضبط اسم العمود، سيتغير قيمة الخلية المقابلة أيضًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setTotalsCalculation(int value) {#setTotalsCalculation-int-}
```
public void setTotalsCalculation(int value)
```


يضبط نوع الحساب في صف الإجماليات للعمود في القائمة.

انظر [TotalsCalculation](../../com.aspose.cells/totalscalculation).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTotalsRowLabel(String value) {#setTotalsRowLabel-java.lang.String-}
```
public void setTotalsRowLabel(String value)
```


يضبط تسميات العرض لصف الإجماليات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

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

