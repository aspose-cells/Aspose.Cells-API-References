---
title: "AbstractFormulaChangeMonitor"
second_title: "Aspose.Cells for Java API Reference"
description: "مراقبة للمستخدم لتتبع تغيير الصيغ أثناء عمليات معينة."
type: docs
url: /ar/java/com.aspose.cells/abstractformulachangemonitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractFormulaChangeMonitor
```

مراقبة للمستخدم لتتبع تغيير الصيغ أثناء عمليات معينة.

**Remarks**

على سبيل المثال، أثناء حذف/إدراج نطاق من الخلايا، قد تتغير صيغ الخلايا الأخرى بسبب إزاحة المراجع. يرجى ملاحظة أن طرق المراقب قد تُستدعى عدة مرات لكائن واحد يحتوي على الصيغة.

**Example**

```
         class MyFormulaChangeMonitor extends AbstractFormulaChangeMonitor
         {
             private final WorksheetCollection mWorksheets;
             public MyFormulaChangeMonitor(WorksheetCollection worksheets)
             {
                 mWorksheets = worksheets;
             }
             public /*override*/ void onCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
             {
                 System.out.println("Cell " + mWorksheets.get(sheetIndex).getName() + "!"
                     + CellsHelper.cellIndexToName(rowIndex, columnIndex)
                     + "'s formula was changed while inserting rows.");
             }
         }
         Workbook wb = new Workbook("template.xlsx");
         InsertOptions options = new InsertOptions();
         options.setFormulaChangeMonitor(new MyFormulaChangeMonitor(wb.getWorksheets()));
         wb.getWorksheets().get(0).getCells().insertRows(0, 2, options);
```
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [AbstractFormulaChangeMonitor()](#AbstractFormulaChangeMonitor--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [onCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)](#onCellFormulaChanged-int-int-int-) | الحدث الذي سيتم تشغيله عندما تتغير الصيغة في خلية. |
| [onFormatConditionFormulaChanged(FormatCondition fc)](#onFormatConditionFormulaChanged-com.aspose.cells.FormatCondition-) | الحدث الذي سيتم تشغيله عندما تتغير صيغة FormatCondition. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractFormulaChangeMonitor() {#AbstractFormulaChangeMonitor--}
```
public AbstractFormulaChangeMonitor()
```


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




### onCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex) {#onCellFormulaChanged-int-int-int-}
```
public void onCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
```


الحدث الذي سيتم تشغيله عندما تتغير الصيغة في خلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetIndex | int | فهرس الورقة للخلية المتغيّرة. |
| rowIndex | int | فهرس الصف للخلية المتغيّرة. |
| columnIndex | int | فهرس العمود للخلية المتغيّرة. |

### onFormatConditionFormulaChanged(FormatCondition fc) {#onFormatConditionFormulaChanged-com.aspose.cells.FormatCondition-}
```
public void onFormatConditionFormulaChanged(FormatCondition fc)
```


الحدث الذي سيتم تشغيله عندما تتغير صيغة FormatCondition.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fc | [FormatCondition](../../com.aspose.cells/formatcondition) | كائن FormatCondition الذي تغيرت صيغته. |

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

