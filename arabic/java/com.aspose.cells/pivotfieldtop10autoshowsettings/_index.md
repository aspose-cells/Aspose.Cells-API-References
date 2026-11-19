---
title: "PivotFieldTop10AutoShowSettings"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل إعدادات Top 10 AutoShow لحقل pivot."
type: docs
url: /ar/java/com.aspose.cells/pivotfieldtop10autoshowsettings/
---

**Inheritance:**
java.lang.Object
```
public class PivotFieldTop10AutoShowSettings
```

يمثل إعدادات Top 10 AutoShow لحقل pivot.

**Remarks**

في xls : تنفيذ مرشحات أعلى 10 في Xls عبر Top 10 AutoShow. في ملفات ooxml : يدعم تنسيق ملف ooxml الأساسي Top10 AutoShow، لكن واجهة المستخدم في Excel 2007 وما بعدها توفر الوصول فقط عبر مرشح Top10. إذا لم تكن توافقية XLS مطلوبة، يُنصح باستخدام مرشح Top10 بدلاً من ذلك.

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("fruit");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("blueberry");
         cells.get(3, 0).setValue("kiwi");
         cells.get(4, 0).setValue("cherry");
         cells.get(5, 0).setValue("grape");
         cells.get(6, 0).setValue("blueberry");
         cells.get(7, 0).setValue("kiwi");
         cells.get(8, 0).setValue("cherry");
 
         cells.get(0, 1).setValue("year");
         cells.get(1, 1).setValue(2020);
         cells.get(2, 1).setValue(2020);
         cells.get(3, 1).setValue(2020);
         cells.get(4, 1).setValue(2020);
         cells.get(5, 1).setValue(2021);
         cells.get(6, 1).setValue(2021);
         cells.get(7, 1).setValue(2021);
         cells.get(8, 1).setValue(2021);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
         cells.get(5, 2).setValue(90);
         cells.get(6, 2).setValue(100);
         cells.get(7, 2).setValue(110);
         cells.get(8, 2).setValue(120);
 
         PivotTableCollection pivots = sheet.getPivotTables();
 
         PivotTable pivot = pivots.add("=Sheet1!A1:C9", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
          //Change PivotField's attributes
         PivotField rowField = pivot.getRowFields().get(0);
         rowField.setDisplayName("custom display name");
 
         //Show top 2 items by row field label.
         rowField.top10AutoShow(true, true, 2, -1);
 
         PivotFieldTop10AutoShowSettings sortSetting = rowField.getTop10AutoShowSettings();
         System.out.println(sortSetting.isAutoShow());
 
          pivot.calculateData();
 
         book.save("out.xlsx");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoShowCount()](#getAutoShowCount--) | يمثل عدد العناصر العليا أو السفلى التي تُظهر تلقائيًا في حقل PivotTable المحدد. |
| [getClass()](#getClass--) |  |
| [getRankBy()](#getRankBy--) | يحدد فهرس حقل البيانات لتصنيف AutoShow. |
| [hashCode()](#hashCode--) |  |
| [isAutoShow()](#isAutoShow--) | يشير إلى ما إذا كان تم تطبيق مرشح "Top 10 AutoShow" على هذا الحقل. |
| [isTop()](#isTop--) | يشير إلى ما إذا كان حقل PivotTable المحدد يُعرض تلقائيًا تصاعديًا. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoShow(boolean value)](#setAutoShow-boolean-) | يشير إلى ما إذا كان تم تطبيق مرشح "Top 10 AutoShow" على هذا الحقل. |
| [setAutoShowCount(int value)](#setAutoShowCount-int-) | يمثل عدد العناصر العليا أو السفلى التي تُظهر تلقائيًا في حقل PivotTable المحدد. |
| [setRankBy(int value)](#setRankBy-int-) | يحدد فهرس حقل البيانات لتصنيف AutoShow. |
| [setTop(boolean value)](#setTop-boolean-) | يشير إلى ما إذا كان حقل PivotTable المحدد يُعرض تلقائيًا تصاعديًا. |
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
### getAutoShowCount() {#getAutoShowCount--}
```
public int getAutoShowCount()
```


يمثل عدد العناصر العليا أو السفلى التي تُظهر تلقائيًا في حقل PivotTable المحدد.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getRankBy() {#getRankBy--}
```
public int getRankBy()
```


يحدد فهرس حقل البيانات لتصنيف AutoShow. يمثل فهرس حقل العرض التلقائي. -1 يعني حقل PivotField نفسه. يجب أن يكون فهرس حقول البيانات.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoShow() {#isAutoShow--}
```
public boolean isAutoShow()
```


يشير إلى ما إذا كان تم تطبيق مرشح "Top 10 AutoShow" على هذا الحقل.

**Returns:**
boolean
### isTop() {#isTop--}
```
public boolean isTop()
```


يشير إلى ما إذا كان حقل PivotTable المحدد يُعرض تلقائيًا تصاعديًا.

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




### setAutoShow(boolean value) {#setAutoShow-boolean-}
```
public void setAutoShow(boolean value)
```


يشير إلى ما إذا كان تم تطبيق مرشح "Top 10 AutoShow" على هذا الحقل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAutoShowCount(int value) {#setAutoShowCount-int-}
```
public void setAutoShowCount(int value)
```


يمثل عدد العناصر العليا أو السفلى التي تُظهر تلقائيًا في حقل PivotTable المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setRankBy(int value) {#setRankBy-int-}
```
public void setRankBy(int value)
```


يحدد فهرس حقل البيانات لتصنيف AutoShow. يمثل فهرس حقل العرض التلقائي. -1 يعني حقل PivotField نفسه. يجب أن يكون فهرس حقول البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTop(boolean value) {#setTop-boolean-}
```
public void setTop(boolean value)
```


يشير إلى ما إذا كان حقل PivotTable المحدد يُعرض تلقائيًا تصاعديًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

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

