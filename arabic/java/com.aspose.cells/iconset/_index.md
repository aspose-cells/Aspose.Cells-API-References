---
title: "IconSet"
second_title: "Aspose.Cells for Java API Reference"
description: "يصف قاعدة التنسيق الشرطي لمجموعة الأيقونات."
type: docs
url: /ar/java/com.aspose.cells/iconset/
---

**Inheritance:**
java.lang.Object
```
public class IconSet
```

وصف قاعدة تنسيق الشرطية لـ IconSet. تقوم هذه القاعدة بتطبيق الأيقونات على الخلايا وفقًا لقيمها.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Adds an empty conditional formatting
         int index = sheet.getConditionalFormattings().add();
 
         FormatConditionCollection fcs = sheet.getConditionalFormattings().get(index);
 
         //Sets the conditional format range.
         CellArea ca = new CellArea();
 
         ca.StartRow = 0;
 
         ca.EndRow = 2;
 
         ca.StartColumn = 0;
 
         ca.EndColumn = 0;
 
         fcs.addArea(ca);
 
         //Adds condition.
         int idx = fcs.addCondition(FormatConditionType.ICON_SET);
 
         fcs.addArea(ca);
 
         FormatCondition cond = fcs.get(idx);
 
         //Get Icon Set
         IconSet iconSet = cond.getIconSet();
 
         //Set Icon Type
         iconSet.setType(IconSetType.ARROWS_3);
 
         //Put Cell Values
         Cell cell1 = sheet.getCells().get("A1");
 
         cell1.putValue(10);
 
         Cell cell2 = sheet.getCells().get("A2");
 
         cell2.putValue(120);
 
         Cell cell3 = sheet.getCells().get("A3");
 
         cell3.putValue(260);
 
         //Saving the Excel file
         workbook.save("book1.xlsx");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCfIcons()](#getCfIcons--) | احصل على[ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) من المجموعة |
| [getCfvos()](#getCfvos--) | احصل على مثيل CFValueObjects. |
| [getClass()](#getClass--) |  |
| [getReverse()](#getReverse--) | يحصل على العلامة التي تشير إلى ما إذا كان سيتم عكس الترتيب الافتراضي للأيقونات في مجموعة الأيقونات هذه. |
| [getShowValue()](#getShowValue--) | يحصل على العلامة التي تشير إلى ما إذا كان سيتم إظهار قيم الخلايا التي تم تطبيق مجموعة الأيقونات عليها. |
| [getType()](#getType--) | يحصل على نوع مجموعة الأيقونات للعرض. |
| [hashCode()](#hashCode--) |  |
| [isCustom()](#isCustom--) | يشير إلى ما إذا كانت مجموعة الأيقونات مخصصة. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setReverse(boolean value)](#setReverse-boolean-) | يضبط العلامة التي تشير إلى ما إذا كان سيتم عكس الترتيب الافتراضي للأيقونات في مجموعة الأيقونات هذه. |
| [setShowValue(boolean value)](#setShowValue-boolean-) | يضبط العلامة التي تشير إلى ما إذا كان سيتم إظهار قيم الخلايا التي تم تطبيق مجموعة الأيقونات عليها. |
| [setType(int value)](#setType-int-) | يضبط نوع مجموعة الأيقونات للعرض. |
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
### getCfIcons() {#getCfIcons--}
```
public ConditionalFormattingIconCollection getCfIcons()
```


احصل على[ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) من المجموعة

**Returns:**
[ConditionalFormattingIconCollection](../../com.aspose.cells/conditionalformattingiconcollection)
### getCfvos() {#getCfvos--}
```
public ConditionalFormattingValueCollection getCfvos()
```


احصل على مثيل CFValueObjects.

**Returns:**
[ConditionalFormattingValueCollection](../../com.aspose.cells/conditionalformattingvaluecollection)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getReverse() {#getReverse--}
```
public boolean getReverse()
```


يحصل على العلامة التي تشير إلى ما إذا كان سيتم عكس الترتيب الافتراضي للأيقونات في مجموعة الأيقونات هذه. القيمة الافتراضية هي false.

**Returns:**
boolean
### getShowValue() {#getShowValue--}
```
public boolean getShowValue()
```


يحصل على العلامة التي تشير إلى ما إذا كان سيتم إظهار قيم الخلايا التي تم تطبيق مجموعة الأيقونات عليها. القيمة الافتراضية هي true.

**Returns:**
boolean
### getType() {#getType--}
```
public int getType()
```


يحصل على نوع مجموعة الأيقونات للعرض. سيؤدي ضبط النوع إلى فحص تلقائي إذا كان عدد Cfvos الحالي يتوافق مع النوع الجديد. إذا لم يتوافق، سيتم مسح Cfvos القديمة وإضافة Cfvos الافتراضية.

انظر [IconSetType](../../com.aspose.cells/iconsettype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCustom() {#isCustom--}
```
public boolean isCustom()
```


يشير إلى ما إذا كانت مجموعة الأيقونات مخصصة. القيمة الافتراضية هي false.

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




### setReverse(boolean value) {#setReverse-boolean-}
```
public void setReverse(boolean value)
```


يضبط العلامة التي تشير إلى ما إذا كان سيتم عكس الترتيب الافتراضي للأيقونات في مجموعة الأيقونات هذه. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowValue(boolean value) {#setShowValue-boolean-}
```
public void setShowValue(boolean value)
```


يضبط العلامة التي تشير إلى ما إذا كان سيتم إظهار قيم الخلايا التي تم تطبيق مجموعة الأيقونات عليها. القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


يضبط نوع مجموعة الأيقونات للعرض. ضبط النوع سيتحقق تلقائيًا إذا كان عدد Cfvos الحالي متوافقًا مع النوع الجديد. إذا لم يكن متوافقًا، سيتم تنظيف Cfvos القديمة وإضافة Cfvos الافتراضية.

انظر [IconSetType](../../com.aspose.cells/iconsettype).

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

