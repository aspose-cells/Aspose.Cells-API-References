---
title: "PivotItem"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل عنصرًا في تقرير PivotField."
type: docs
url: /ar/java/com.aspose.cells/pivotitem/
---

**Inheritance:**
java.lang.Object
```
public class PivotItem
```

يمثل عنصرًا في تقرير PivotField.

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
 
         //Hide the first item
         PivotItem item = rowField.getPivotItems().get(0);          
         item.setHidden(true);
 
          pivot.calculateData();
 
         book.save("out.xlsx");
```
## حقول

| حقل | الوصف |
| --- | --- |
| [ALL_PAGE_ITEMS_INDEX](#ALL-PAGE-ITEMS-INDEX) | فهرس الحارس لتحديد الكل لعناصر الصفحة (0x7FFD، ليس فهرسًا صالحًا) |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDateTimeValue()](#getDateTimeValue--) | يحصل على قيمة التاريخ والوقت لعنصر المحور. إذا كانت القيمة null، سيُرجع DateTime.MinValue. |
| [getDoubleValue()](#getDoubleValue--) | يحصل على القيمة المزدوجة لعنصر المحور. إذا كانت القيمة null أو ليست رقمًا، سيُرجع 0. |
| [getFormula()](#getFormula--) | يحصل على الصيغة لهذا العنصر المحسوب. |
| [getIndex()](#getIndex--) | يحصل على فهرس عنصر المحور في حقل الذاكرة المؤقتة. |
| [getName()](#getName--) | يحصل على اسم عنصر المحور. |
| [getPosition()](#getPosition--) | تحديد فهرس هذا العنصر في جميع عناصر PivotItems الخاصة بالحقل. |
| [getPositionInSameParentNode()](#getPositionInSameParentNode--) | تحديد فهرس الموضع في عناصر PivotItems تحت نفس العقدة الأصلية. |
| [getStringValue()](#getStringValue--) | يحصل على القيمة النصية لعنصر الـ pivot. إذا كانت القيمة فارغة (null)، سيعيد "" |
| [getValue()](#getValue--) | يحصل على قيمة عنصر الـ pivot |
| [hashCode()](#hashCode--) |  |
| [hide(boolean value)](#hide-boolean-) | يضبط ما إذا كان عنصر الـ pivot مخفيًا. |
| [isCalculatedItem()](#isCalculatedItem--) | يشير إلى ما إذا كان عنصر الـ pivot هذا عنصر صيغة محسوبة. |
| [isDetailHidden()](#isDetailHidden--) | يحصل على ما إذا كان تفصيل هذا العنصر الـ pivot مخفيًا. |
| [isFormula()](#isFormula--) | يشير إلى ما إذا كان عنصر الـ pivot هذا عنصر صيغة محسوبة. |
| [isHidden()](#isHidden--) | يحصل على ما إذا كان عنصر الـ pivot مخفيًا. |
| [isHideDetail()](#isHideDetail--) | يحصل على ما إذا كان عنصر الـ pivot يخفي التفاصيل. |
| [isMissing()](#isMissing--) | يشير إلى ما إذا تم إزالة العنصر من مصدر البيانات. |
| [move(int offset)](#move-int-) | ينقل العنصر للأعلى أو للأسفل في حقل الـ pivot |
| [move(int offset, boolean isSameParent)](#move-int-boolean-) | ينقل العنصر للأعلى أو للأسفل |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDetailHidden(boolean value)](#setDetailHidden-boolean-) | يضبط ما إذا كان تفصيل هذا العنصر الـ pivot مخفيًا. |
| [setFormula(boolean value)](#setFormula-boolean-) | يشير إلى ما إذا كان عنصر الـ pivot هذا عنصر صيغة محسوبة. |
| [setHidden(boolean value)](#setHidden-boolean-) | يضبط ما إذا كان عنصر الـ pivot مخفيًا. |
| [setHideDetail(boolean value)](#setHideDetail-boolean-) | يضبط ما إذا كان عنصر الـ pivot يخفي التفاصيل. |
| [setIndex(int value)](#setIndex-int-) | يحصل على فهرس عنصر المحور في حقل الذاكرة المؤقتة. |
| [setName(String value)](#setName-java.lang.String-) | يحصل على اسم عنصر المحور. |
| [setPosition(int value)](#setPosition-int-) | تحديد فهرس هذا العنصر في جميع عناصر PivotItems الخاصة بالحقل. |
| [setPositionInSameParentNode(int value)](#setPositionInSameParentNode-int-) | تحديد فهرس الموضع في عناصر PivotItems تحت نفس العقدة الأصلية. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ALL_PAGE_ITEMS_INDEX {#ALL-PAGE-ITEMS-INDEX}
```
public static final short ALL_PAGE_ITEMS_INDEX
```


فهرس الحارس لتحديد الكل لعناصر الصفحة (0x7FFD، ليس فهرسًا صالحًا)

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
### getDateTimeValue() {#getDateTimeValue--}
```
public DateTime getDateTimeValue()
```


يحصل على قيمة التاريخ والوقت لعنصر المحور. إذا كانت القيمة null، سيُرجع DateTime.MinValue.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getDoubleValue() {#getDoubleValue--}
```
public double getDoubleValue()
```


يحصل على القيمة المزدوجة لعنصر المحور. إذا كانت القيمة null أو ليست رقمًا، سيُرجع 0.

**Returns:**
double
### getFormula() {#getFormula--}
```
public String getFormula()
```


يحصل على صيغة هذا العنصر المحسوب. يعمل فقط عندما يكون هذا العنصر عنصرًا محسوبًا.

**Returns:**
java.lang.String -
### getIndex() {#getIndex--}
```
public int getIndex()
```


يحصل على فهرس عنصر المحور في حقل الذاكرة المؤقتة.

**Remarks**

ملاحظة: هذه الخاصية الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية **PivotItem.Position**. سيتم إزالة هذه الطريقة بعد 6 أشهر اعتبارًا من أغسطس 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


يحصل على اسم عنصر المحور.

**Returns:**
java.lang.String
### getPosition() {#getPosition--}
```
public int getPosition()
```


تحديد فهرس هذا العنصر في جميع عناصر PivotItems الخاصة بالحقل.

**Returns:**
int
### getPositionInSameParentNode() {#getPositionInSameParentNode--}
```
public int getPositionInSameParentNode()
```


تحديد فهرس الموضع في عناصر PivotItems تحت نفس العقدة الأصلية.

**Remarks**

ملاحظة: هذه الطريقة الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة **PivotTable.MoveItem(PivotFieldType, string[],bool,int)**. سيتم إزالة هذه الطريقة بعد 12 شهرًا اعتبارًا من نوفمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
int
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```


يحصل على القيمة النصية لعنصر الـ pivot. إذا كانت القيمة فارغة (null)، سيعيد ""

**Returns:**
java.lang.String
### getValue() {#getValue--}
```
public Object getValue()
```


يحصل على قيمة عنصر الـ pivot

**Returns:**
java.lang.Object
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### hide(boolean value) {#hide-boolean-}
```
public void hide(boolean value)
```


يضبط ما إذا كان عنصر الـ pivot مخفيًا.

**Remarks**

ملاحظة: هذا العضو الآن مهجور. بدلاً من ذلك، يرجى استخدام خاصية **Aspose.Cells.Pivot.PivotItem.IsHidden**. سيتم إزالة هذه الخاصية بعد 12 شهرًا اعتبارًا من يناير 2012. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### isCalculatedItem() {#isCalculatedItem--}
```
public boolean isCalculatedItem()
```


يشير إلى ما إذا كان عنصر الـ pivot هذا عنصر صيغة محسوبة.

**Returns:**
boolean
### isDetailHidden() {#isDetailHidden--}
```
public boolean isDetailHidden()
```


يحصل على ما إذا كان تفصيل هذا العنصر الـ pivot مخفيًا.

**Returns:**
boolean
### isFormula() {#isFormula--}
```
public boolean isFormula()
```


يشير إلى ما إذا كان عنصر الـ pivot هذا عنصر صيغة محسوبة.

**Remarks**

ملاحظة: هذه الخاصية الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية **PivotItem.IsCalculatedItem**. سيتم إزالة هذه الخاصية بعد 12 شهرًا اعتبارًا من نوفمبر 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


يحصل على ما إذا كان عنصر الـ pivot مخفيًا.

**Returns:**
boolean
### isHideDetail() {#isHideDetail--}
```
public boolean isHideDetail()
```


يحصل على ما إذا كان عنصر الـ pivot يخفي التفاصيل.

**Remarks**

ملاحظة: هذه الخاصية الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية **PivotItem.IsDetailHidden**. سيتم إزالة هذه الخاصية بعد 12 شهرًا اعتبارًا من نوفمبر 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
boolean
### isMissing() {#isMissing--}
```
public boolean isMissing()
```


يشير إلى ما إذا تم إزالة العنصر من مصدر البيانات.

**Remarks**

يعني True أن هذه القيمة قد أُزيلت من مصدر البيانات.

**Returns:**
boolean
### move(int offset) {#move-int-}
```
public void move(int offset)
```


ينقل العنصر للأعلى أو للأسفل في حقل الـ pivot

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الإزاحة | int | عدد مرات التحريك للأعلى أو للأسفل. حرّك العنصر للأعلى إذا كانت القيمة أقل من الصفر؛ حرّك العنصر للأسفل إذا كانت القيمة أكبر من الصفر. |

### move(int offset, boolean isSameParent) {#move-int-boolean-}
```
public void move(int offset, boolean isSameParent)
```


ينقل العنصر للأعلى أو للأسفل

**Remarks**

ملاحظة: هذه الطريقة الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة **PivotTable.MoveItem(PivotFieldType, string[],bool,int)** أو طريقة **PivotItem.Move(int)**. سيتم إزالة هذه الطريقة بعد 12 شهرًا اعتبارًا من نوفمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الإزاحة | int | عدد مرات التحريك للأعلى أو للأسفل. حرّك العنصر للأعلى إذا كانت القيمة أقل من الصفر؛ حرّك العنصر للأسفل إذا كانت القيمة أكبر من الصفر. |
| isSameParent | boolean | تحديد ما إذا كانت عملية النقل في نفس العقدة الأصلية أم لا |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setDetailHidden(boolean value) {#setDetailHidden-boolean-}
```
public void setDetailHidden(boolean value)
```


يضبط ما إذا كان تفصيل هذا العنصر الـ pivot مخفيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setFormula(boolean value) {#setFormula-boolean-}
```
public void setFormula(boolean value)
```


يشير إلى ما إذا كان عنصر الـ pivot هذا عنصر صيغة محسوبة.

**Remarks**

ملاحظة: هذه الخاصية الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية **PivotItem.IsCalculatedItem**. سيتم إزالة هذه الخاصية بعد 12 شهرًا اعتبارًا من نوفمبر 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


يضبط ما إذا كان عنصر الـ pivot مخفيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHideDetail(boolean value) {#setHideDetail-boolean-}
```
public void setHideDetail(boolean value)
```


يضبط ما إذا كان عنصر الـ pivot يخفي التفاصيل.

**Remarks**

ملاحظة: هذه الخاصية الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية **PivotItem.IsDetailHidden**. سيتم إزالة هذه الخاصية بعد 12 شهرًا اعتبارًا من نوفمبر 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setIndex(int value) {#setIndex-int-}
```
public void setIndex(int value)
```


يحصل على فهرس عنصر المحور في حقل الذاكرة المؤقتة.

**Remarks**

ملاحظة: هذه الخاصية الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية **PivotItem.Position**. سيتم إزالة هذه الطريقة بعد 6 أشهر اعتبارًا من أغسطس 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


يحصل على اسم عنصر المحور.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setPosition(int value) {#setPosition-int-}
```
public void setPosition(int value)
```


تحديد فهرس هذا العنصر في جميع عناصر PivotItems الخاصة بالحقل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPositionInSameParentNode(int value) {#setPositionInSameParentNode-int-}
```
public void setPositionInSameParentNode(int value)
```


تحديد فهرس الموضع في عناصر PivotItems تحت نفس العقدة الأصلية.

**Remarks**

ملاحظة: هذه الطريقة الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة **PivotTable.MoveItem(PivotFieldType, string[],bool,int)**. سيتم إزالة هذه الطريقة بعد 12 شهرًا اعتبارًا من نوفمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

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

