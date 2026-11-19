---
title: "CalculationCell"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل البيانات المتعلقة بالحساب لخلية واحدة يتم حسابها."
type: docs
url: /ar/java/com.aspose.cells/calculationcell/
---

**Inheritance:**
java.lang.Object
```
public class CalculationCell
```

يمثل البيانات المتعلقة بالحساب لخلية واحدة يتم حسابها.

**Remarks**

يجب على المستخدم عدم تغيير أي بيانات في الـ Workbook أثناء عملية حساب الصيغ، وإلا قد يحدث نتيجة غير متوقعة أو استثناء. لذلك، جميع الكائنات التي توفرها هذه الفئة (مثل كائن Cell في [getCell()](../../com.aspose.cells/calculationcell\#getCell--)) مخصصة للغرض "القراءة" فقط.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCell()](#getCell--) | يحصل على كائن Cell الذي يتم حسابه. |
| [getCellColumn()](#getCellColumn--) | يحصل على فهرس العمود للخلية. |
| [getCellRow()](#getCellRow--) | يحصل على فهرس الصف للخلية. |
| [getClass()](#getClass--) |  |
| [getWorkbook()](#getWorkbook--) | يحصل على كائن Workbook. |
| [getWorksheet()](#getWorksheet--) | يحصل على كائن Worksheet الذي توجد فيه الخلية. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalculatedValue(Object v)](#setCalculatedValue-java.lang.Object-) | يضبط القيمة المحسوبة للخلية. |
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
### getCell() {#getCell--}
```
public Cell getCell()
```


يحصل على كائن Cell الذي يتم حسابه.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getCellColumn() {#getCellColumn--}
```
public int getCellColumn()
```


يحصل على فهرس العمود للخلية.

**Returns:**
int
### getCellRow() {#getCellRow--}
```
public int getCellRow()
```


يحصل على فهرس الصف للخلية.

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


يحصل على كائن Workbook.

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


يحصل على كائن Worksheet الذي توجد فيه الخلية.

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


يضبط القيمة المحسوبة للخلية.

**Remarks**

يمكن للمستخدم تعيين النتيجة المحسوبة بهذه الطريقة لتجاهل الحساب التلقائي للخلية.

**Parameters:**
| معامل | نوع | الوصف |
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

