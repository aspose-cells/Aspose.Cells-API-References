---
title: "عمود"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل عمودًا واحدًا في ورقة عمل."
type: docs
url: /ar/java/com.aspose.cells/column/
---

**Inheritance:**
java.lang.Object
```
public class Column
```

يمثل عمودًا واحدًا في ورقة عمل.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
         Style style = workbook.createStyle();
 
         //Setting the background color to Blue
         style.setBackgroundColor(Color.getBlue());
 
         //Setting the foreground color to Red
         style.setForegroundColor(Color.getRed());
 
         //setting Background Pattern
         style.setPattern(BackgroundType.DIAGONAL_STRIPE);
 
         //New Style Flag
         StyleFlag styleFlag = new StyleFlag();
 
         //Set All Styles
         styleFlag.setAll(true);
 
         //Get first Column
         Column column = worksheet.getCells().getColumns().get(0);
 
         //Apply Style to first Column
         column.applyStyle(style, styleFlag);
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | يطبق التنسيقات على عمود كامل. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getGroupLevel()](#getGroupLevel--) | يحصل على مستوى المجموعة للعمود. |
| [getIndex()](#getIndex--) | يحصل على فهرس هذا العمود. |
| [getStyle()](#getStyle--) | يحصل على نمط هذا العمود. |
| [getWidth()](#getWidth--) | يحصل على عرض العمود بوحدة الأحرف. |
| [hasCustomStyle()](#hasCustomStyle--) | يشير إلى ما إذا كان لهذا العمود إعدادات نمط مخصصة(مختلفة عن الإعداد الافتراضي الموروث من المصنف). |
| [hashCode()](#hashCode--) |  |
| [isCollapsed()](#isCollapsed--) | ما إذا كان العمود مطويًا |
| [isHidden()](#isHidden--) | يشير إلى ما إذا كان العمود مخفيًا. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCollapsed(boolean value)](#setCollapsed-boolean-) | ما إذا كان العمود مطويًا |
| [setGroupLevel(byte value)](#setGroupLevel-byte-) | يحصل على مستوى المجموعة للعمود. |
| [setHidden(boolean value)](#setHidden-boolean-) | يشير إلى ما إذا كان العمود مخفيًا. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | يضبط نمط هذا العمود. |
| [setWidth(double value)](#setWidth-double-) | يضبط عرض العمود بوحدة الأحرف. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


يطبق التنسيقات على عمود كامل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | كائن النمط الذي سيتم تطبيقه. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | علامات تشير إلى خصائص التنسيق المطبقة. |

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
### getGroupLevel() {#getGroupLevel--}
```
public byte getGroupLevel()
```


يحصل على مستوى المجموعة للعمود.

**Returns:**
byte
### getIndex() {#getIndex--}
```
public int getIndex()
```


يحصل على فهرس هذا العمود.

**Returns:**
int
### getStyle() {#getStyle--}
```
public Style getStyle()
```


يحصل على نمط هذا العمود.

**Remarks**

تعديل كائن النمط المرتجع مباشرة لا يؤثر على هذا العمود أو أي خلايا في هذا العمود. عليك استدعاء طريقة [applyStyle(Style,StyleFlag)](../../com.aspose.cells/column\#applyStyle-Style-StyleFlag-) أو [setStyle(Style)](../../com.aspose.cells/column\#setStyle-Style-) لتطبيق التغيير على هذا العمود.

نمط العمود هو النمط الذي سيُورث إلى الخلايا في هذا العمود(تلك الخلايا التي لا تملك إعدادات نمط مخصصة، مثل الخلايا الموجودة التي لم يتم تعيين نمط لها صراحةً، أو تلك التي لم يتم إنشاءها).

**Returns:**
[Style](../../com.aspose.cells/style)
### getWidth() {#getWidth--}
```
public double getWidth()
```


يحصل على عرض العمود بوحدة الأحرف.

**Remarks**

في جداول البيانات، يتم قياس عرض العمود كعدد الأحرف لعرض الرقم الأقصى للأرقام 0~9 كما يتم عرضها في خط النمط العادي.

**Returns:**
double
### hasCustomStyle() {#hasCustomStyle--}
```
public boolean hasCustomStyle()
```


يشير إلى ما إذا كان لهذا العمود إعدادات نمط مخصصة(مختلفة عن الإعداد الافتراضي الموروث من المصنف).

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCollapsed() {#isCollapsed--}
```
public boolean isCollapsed()
```


ما إذا كان العمود مطويًا

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


يشير إلى ما إذا كان العمود مخفيًا.

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




### setCollapsed(boolean value) {#setCollapsed-boolean-}
```
public void setCollapsed(boolean value)
```


ما إذا كان العمود مطويًا

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setGroupLevel(byte value) {#setGroupLevel-byte-}
```
public void setGroupLevel(byte value)
```


يحصل على مستوى المجموعة للعمود.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | byte |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


يشير إلى ما إذا كان العمود مخفيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


يضبط نمط هذا العمود.

**Remarks**

هذه الطريقة تقوم فقط بتعيين النمط المحدد كنمط افتراضي لهذا العمود، دون تغيير إعدادات النمط للخلايا الموجودة في هذا العمود. لتحديث إعدادات النمط للخلايا الموجودة إلى النمط المحدد في نفس الوقت، يرجى استخدام [applyStyle(Style,StyleFlag)](../../com.aspose.cells/column\#applyStyle-Style-StyleFlag-)

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | النمط الذي سيُستخدم كنمط افتراضي للخلايا في هذا العمود. |

### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```


يضبط عرض العمود بوحدة الأحرف.

**Remarks**

في جداول البيانات، يتم قياس عرض العمود كعدد الأحرف لعرض الرقم الأقصى للأرقام 0~9 كما يتم عرضها في خط النمط العادي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

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

