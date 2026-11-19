---
title: "ListBoxActiveXControl"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل عنصر التحكم ActiveX لمربع القائمة."
type: docs
url: /ar/java/com.aspose.cells/listboxactivexcontrol/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ActiveXControlBase](../../com.aspose.cells/activexcontrolbase), [com.aspose.cells.ActiveXControl](../../com.aspose.cells/activexcontrol)
```
public class ListBoxActiveXControl extends ActiveXControl
```

يمثل عنصر التحكم ActiveX لمربع القائمة.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackOleColor()](#getBackOleColor--) | يحصل على لون ole للخلفية. |
| [getBorderOleColor()](#getBorderOleColor--) | يحصل على لون ole للخلفية. |
| [getBorderStyle()](#getBorderStyle--) | يحصل على نوع الحد المستخدم من قبل التحكم. |
| [getBoundColumn()](#getBoundColumn--) | يمثل كيفية تحديد خاصية Value لصندوق ComboBox أو ListBox عندما تكون قيمة خاصية MultiSelect هي (fmMultiSelectSingle). |
| [getClass()](#getClass--) |  |
| [getColumnCount()](#getColumnCount--) | يمثل عدد الأعمدة التي سيتم عرضها في صندوق ComboBox أو ListBox. |
| [getColumnWidths()](#getColumnWidths--) | يحصل على عرض العمود. |
| [getData()](#getData--) | يحصل على البيانات الثنائية للتحكم. |
| [getFont()](#getFont--) | يمثل خط التحكم. |
| [getForeOleColor()](#getForeOleColor--) | يحصل على لون OLE للمقدمة. |
| [getHeight()](#getHeight--) | يحصل على ارتفاع التحكم بوحدة النقاط. |
| [getIMEMode()](#getIMEMode--) | يحصل على وضع التشغيل الافتراضي لمحرر طريقة الإدخال للتحكم عند استلامه للتركيز. |
| [getIntegralHeight()](#getIntegralHeight--) | يشير إلى ما إذا كان التحكم سيظهر فقط أسطر النص الكاملة دون إظهار أي أسطر جزئية. |
| [getLinkedCell()](#getLinkedCell--) | يحصل على الخلية المرتبطة. |
| [getListFillRange()](#getListFillRange--) | يحصل على نطاق تعبئة القائمة. |
| [getListStyle()](#getListStyle--) | يحصل على المظهر البصري. |
| [getListWidth()](#getListWidth--) | يحصل على العرض بوحدة النقاط. |
| [getMatchEntry()](#getMatchEntry--) | يشير إلى كيفية بحث ListBox أو ComboBox في قائمته عندما يكتب المستخدم. |
| [getMouseIcon()](#getMouseIcon--) | يحصل على أيقونة مخصصة لعرضها كمؤشر الفأرة للتحكم. |
| [getMousePointer()](#getMousePointer--) | يحصل على نوع الأيقونة المعروضة كمؤشر الفأرة للتحكم. |
| [getScrollBars()](#getScrollBars--) | يشير إلى ما إذا كان التحكم يحتوي على أشرطة تمرير عمودية، أشرطة تمرير أفقية، كلاهما، أو لا شيء. |
| [getSelectionType()](#getSelectionType--) | يشير إلى ما إذا كان التحكم يسمح بتحديدات متعددة. |
| [getShadow()](#getShadow--) | يشير إلى ما إذا كان يجب إظهار الظل. |
| [getShowColumnHeads()](#getShowColumnHeads--) | يشير إلى ما إذا كانت عناوين الأعمدة معروضة. |
| [getSpecialEffect()](#getSpecialEffect--) | يحصل على التأثير الخاص للتحكم. |
| [getTextAlign()](#getTextAlign--) | يمثل طريقة محاذاة النص المستخدم في التحكم. |
| [getTextColumn()](#getTextColumn--) | يمثل العمود في ComboBox أو ListBox لعرضه للمستخدم. |
| [getType()](#getType--) | يحصل على نوع عنصر التحكم ActiveX. |
| [getValue()](#getValue--) | يحصل على قيمة التحكم. |
| [getWidth()](#getWidth--) | يحصل على عرض التحكم بوحدة النقاط. |
| [getWorkbook()](#getWorkbook--) | يحصل على كائن [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--). |
| [hashCode()](#hashCode--) |  |
| [isAutoSize()](#isAutoSize--) | يشير إلى ما إذا كان التحكم سيعيد تحجيمه تلقائيًا لعرض محتوياته بالكامل. |
| [isEnabled()](#isEnabled--) | يشير إلى ما إذا كان التحكم يمكنه استلام التركيز والاستجابة للأحداث التي يولدها المستخدم. |
| [isLocked()](#isLocked--) | يشير إلى ما إذا كانت البيانات في التحكم مقفلة للتحرير. |
| [isTransparent()](#isTransparent--) | يشير إلى ما إذا كان التحكم شفافًا. |
| [isVisible()](#isVisible--) | يشير إلى ما إذا كان هذا التحكم مرئيًا. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | يشير إلى ما إذا كان التحكم سيعيد تحجيمه تلقائيًا لعرض محتوياته بالكامل. |
| [setBackOleColor(int value)](#setBackOleColor-int-) | يضبط لون OLE للخلفية. |
| [setBorderOleColor(int value)](#setBorderOleColor-int-) | يضبط لون OLE للخلفية. |
| [setBorderStyle(int value)](#setBorderStyle-int-) | يضبط نوع الحد المستخدم من قبل التحكم. |
| [setBoundColumn(int value)](#setBoundColumn-int-) | يمثل كيفية تحديد خاصية Value لصندوق ComboBox أو ListBox عندما تكون قيمة خاصية MultiSelect هي (fmMultiSelectSingle). |
| [setColumnCount(int value)](#setColumnCount-int-) | يمثل عدد الأعمدة التي سيتم عرضها في صندوق ComboBox أو ListBox. |
| [setColumnWidths(double value)](#setColumnWidths-double-) | يضبط عرض العمود. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | يشير إلى ما إذا كان التحكم يمكنه استلام التركيز والاستجابة للأحداث التي يولدها المستخدم. |
| [setForeOleColor(int value)](#setForeOleColor-int-) | يضبط لون OLE للمقدمة. |
| [setHeight(double value)](#setHeight-double-) | يضبط ارتفاع التحكم بوحدة النقاط. |
| [setIMEMode(int value)](#setIMEMode-int-) | يضبط وضع التشغيل الافتراضي لمحرر طريقة الإدخال للتحكم عند استلامه للتركيز. |
| [setIntegralHeight(boolean value)](#setIntegralHeight-boolean-) | يشير إلى ما إذا كان التحكم سيظهر فقط أسطر النص الكاملة دون إظهار أي أسطر جزئية. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | يضبط الخلية المرتبطة. |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | يضبط نطاق تعبئة القائمة. |
| [setListStyle(int value)](#setListStyle-int-) | يضبط المظهر البصري. |
| [setListWidth(double value)](#setListWidth-double-) | يضبط العرض بوحدة النقاط. |
| [setLocked(boolean value)](#setLocked-boolean-) | يشير إلى ما إذا كانت البيانات في التحكم مقفلة للتحرير. |
| [setMatchEntry(int value)](#setMatchEntry-int-) | يشير إلى كيفية بحث ListBox أو ComboBox في قائمته عندما يكتب المستخدم. |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | يضبط أيقونة مخصصة لتظهر كمؤشر الفأرة للتحكم. |
| [setMousePointer(int value)](#setMousePointer-int-) | يضبط نوع الأيقونة المعروضة كمؤشر الفأرة للتحكم. |
| [setScrollBars(int value)](#setScrollBars-int-) | يشير إلى ما إذا كان التحكم يحتوي على أشرطة تمرير عمودية، أشرطة تمرير أفقية، كلاهما، أو لا شيء. |
| [setSelectionType(int value)](#setSelectionType-int-) | يشير إلى ما إذا كان التحكم يسمح بتحديدات متعددة. |
| [setShadow(boolean value)](#setShadow-boolean-) | يشير إلى ما إذا كان يجب إظهار الظل. |
| [setShowColumnHeads(boolean value)](#setShowColumnHeads-boolean-) | يشير إلى ما إذا كانت عناوين الأعمدة معروضة. |
| [setSpecialEffect(int value)](#setSpecialEffect-int-) | يضبط التأثير الخاص للتحكم. |
| [setTextAlign(int value)](#setTextAlign-int-) | يمثل طريقة محاذاة النص المستخدم في التحكم. |
| [setTextColumn(int value)](#setTextColumn-int-) | يمثل العمود في ComboBox أو ListBox لعرضه للمستخدم. |
| [setTransparent(boolean value)](#setTransparent-boolean-) | يشير إلى ما إذا كان التحكم شفافًا. |
| [setValue(String value)](#setValue-java.lang.String-) | يضبط قيمة التحكم. |
| [setVisible(boolean value)](#setVisible-boolean-) | يشير إلى ما إذا كان هذا التحكم مرئيًا. |
| [setWidth(double value)](#setWidth-double-) | يضبط عرض التحكم بوحدة النقاط. |
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
### getBackOleColor() {#getBackOleColor--}
```
public int getBackOleColor()
```


يحصل على لون ole للخلفية.

**Returns:**
int
### getBorderOleColor() {#getBorderOleColor--}
```
public int getBorderOleColor()
```


يحصل على لون ole للخلفية.

**Returns:**
int
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


يحصل على نوع الحد المستخدم من قبل التحكم.

انظر [ControlBorderType](../../com.aspose.cells/controlbordertype).

**Returns:**
int
### getBoundColumn() {#getBoundColumn--}
```
public int getBoundColumn()
```


يمثل كيفية تحديد خاصية Value لصندوق ComboBox أو ListBox عندما تكون قيمة خاصية MultiSelect هي (fmMultiSelectSingle).

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


يمثل عدد الأعمدة التي سيتم عرضها في صندوق ComboBox أو ListBox.

**Returns:**
int
### getColumnWidths() {#getColumnWidths--}
```
public double getColumnWidths()
```


يحصل على عرض العمود.

**Returns:**
double
### getData() {#getData--}
```
public byte[] getData()
```


يحصل على البيانات الثنائية للتحكم.

**Returns:**
byte[]
### getFont() {#getFont--}
```
public Font getFont()
```


يمثل خط التحكم.

**Returns:**
[Font](../../com.aspose.cells/font)
### getForeOleColor() {#getForeOleColor--}
```
public int getForeOleColor()
```


يحصل على لون OLE للمقدمة.

**Remarks**

لا ينطبق على التحكم بالصورة.

**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```


يحصل على ارتفاع التحكم بوحدة النقاط.

**Returns:**
double
### getIMEMode() {#getIMEMode--}
```
public int getIMEMode()
```


يحصل على وضع التشغيل الافتراضي لمحرر طريقة الإدخال للتحكم عند استلامه للتركيز.

انظر [InputMethodEditorMode](../../com.aspose.cells/inputmethodeditormode).

**Returns:**
int
### getIntegralHeight() {#getIntegralHeight--}
```
public boolean getIntegralHeight()
```


يشير إلى ما إذا كان التحكم سيظهر فقط أسطر النص الكاملة دون إظهار أي أسطر جزئية.

**Returns:**
boolean
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```


يحصل على الخلية المرتبطة.

**Returns:**
java.lang.String
### getListFillRange() {#getListFillRange--}
```
public String getListFillRange()
```


يحصل على نطاق تعبئة القائمة.

**Returns:**
java.lang.String
### getListStyle() {#getListStyle--}
```
public int getListStyle()
```


يحصل على المظهر البصري.

انظر [ControlListStyle](../../com.aspose.cells/controlliststyle).

**Returns:**
int
### getListWidth() {#getListWidth--}
```
public double getListWidth()
```


يحصل على العرض بوحدة النقاط.

**Returns:**
double
### getMatchEntry() {#getMatchEntry--}
```
public int getMatchEntry()
```


يشير إلى كيفية بحث ListBox أو ComboBox في قائمته عندما يكتب المستخدم.

انظر [ControlMatchEntryType](../../com.aspose.cells/controlmatchentrytype).

**Returns:**
int
### getMouseIcon() {#getMouseIcon--}
```
public byte[] getMouseIcon()
```


يحصل على أيقونة مخصصة لعرضها كمؤشر الفأرة للتحكم.

**Returns:**
byte[]
### getMousePointer() {#getMousePointer--}
```
public int getMousePointer()
```


يحصل على نوع الأيقونة المعروضة كمؤشر الفأرة للتحكم.

انظر [ControlMousePointerType](../../com.aspose.cells/controlmousepointertype).

**Returns:**
int
### getScrollBars() {#getScrollBars--}
```
public int getScrollBars()
```


يشير إلى ما إذا كان التحكم يحتوي على أشرطة تمرير عمودية، أشرطة تمرير أفقية، كلاهما، أو لا شيء.

انظر [ControlScrollBarType](../../com.aspose.cells/controlscrollbartype).

**Returns:**
int
### getSelectionType() {#getSelectionType--}
```
public int getSelectionType()
```


يشير إلى ما إذا كان التحكم يسمح بتحديدات متعددة.

انظر [SelectionType](../../com.aspose.cells/selectiontype).

**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


يشير إلى ما إذا كان يجب إظهار الظل.

**Returns:**
boolean
### getShowColumnHeads() {#getShowColumnHeads--}
```
public boolean getShowColumnHeads()
```


يشير إلى ما إذا كانت عناوين الأعمدة معروضة.

**Returns:**
boolean
### getSpecialEffect() {#getSpecialEffect--}
```
public int getSpecialEffect()
```


يحصل على التأثير الخاص للتحكم.

انظر [ControlSpecialEffectType](../../com.aspose.cells/controlspecialeffecttype).

**Returns:**
int
### getTextAlign() {#getTextAlign--}
```
public int getTextAlign()
```


يمثل طريقة محاذاة النص المستخدم في التحكم.

انظر [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getTextColumn() {#getTextColumn--}
```
public int getTextColumn()
```


يمثل العمود في ComboBox أو ListBox لعرضه للمستخدم.

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


يحصل على نوع عنصر التحكم ActiveX.

انظر [ControlType](../../com.aspose.cells/controltype).

**Returns:**
int
### getValue() {#getValue--}
```
public String getValue()
```


يحصل على قيمة التحكم.

**Remarks**

يؤثر فقط عندما [getSelectionType()](../../com.aspose.cells/listboxactivexcontrol\#getSelectionType--) هو SelectionType.Single;

**Returns:**
java.lang.String
### getWidth() {#getWidth--}
```
public double getWidth()
```


يحصل على عرض التحكم بوحدة النقاط.

**Returns:**
double
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


يحصل على كائن [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--).

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoSize() {#isAutoSize--}
```
public boolean isAutoSize()
```


يشير إلى ما إذا كان التحكم سيعيد تحجيمه تلقائيًا لعرض محتوياته بالكامل.

**Returns:**
boolean
### isEnabled() {#isEnabled--}
```
public boolean isEnabled()
```


يشير إلى ما إذا كان التحكم يمكنه استلام التركيز والاستجابة للأحداث التي يولدها المستخدم.

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


يشير إلى ما إذا كانت البيانات في التحكم مقفلة للتحرير.

**Returns:**
boolean
### isTransparent() {#isTransparent--}
```
public boolean isTransparent()
```


يشير إلى ما إذا كان التحكم شفافًا.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


يشير إلى ما إذا كان هذا التحكم مرئيًا.

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




### setAutoSize(boolean value) {#setAutoSize-boolean-}
```
public void setAutoSize(boolean value)
```


يشير إلى ما إذا كان التحكم سيعيد تحجيمه تلقائيًا لعرض محتوياته بالكامل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setBackOleColor(int value) {#setBackOleColor-int-}
```
public void setBackOleColor(int value)
```


يضبط لون OLE للخلفية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setBorderOleColor(int value) {#setBorderOleColor-int-}
```
public void setBorderOleColor(int value)
```


يضبط لون OLE للخلفية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setBorderStyle(int value) {#setBorderStyle-int-}
```
public void setBorderStyle(int value)
```


يضبط نوع الحد المستخدم من قبل التحكم.

انظر [ControlBorderType](../../com.aspose.cells/controlbordertype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setBoundColumn(int value) {#setBoundColumn-int-}
```
public void setBoundColumn(int value)
```


يمثل كيفية تحديد خاصية Value لصندوق ComboBox أو ListBox عندما تكون قيمة خاصية MultiSelect هي (fmMultiSelectSingle).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setColumnCount(int value) {#setColumnCount-int-}
```
public void setColumnCount(int value)
```


يمثل عدد الأعمدة التي سيتم عرضها في صندوق ComboBox أو ListBox.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setColumnWidths(double value) {#setColumnWidths-double-}
```
public void setColumnWidths(double value)
```


يضبط عرض العمود.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public void setEnabled(boolean value)
```


يشير إلى ما إذا كان التحكم يمكنه استلام التركيز والاستجابة للأحداث التي يولدها المستخدم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setForeOleColor(int value) {#setForeOleColor-int-}
```
public void setForeOleColor(int value)
```


يضبط لون OLE للمقدمة.

**Remarks**

لا ينطبق على التحكم بالصورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


يضبط ارتفاع التحكم بوحدة النقاط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setIMEMode(int value) {#setIMEMode-int-}
```
public void setIMEMode(int value)
```


يضبط وضع التشغيل الافتراضي لمحرر طريقة الإدخال للتحكم عند استلامه للتركيز.

انظر [InputMethodEditorMode](../../com.aspose.cells/inputmethodeditormode).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setIntegralHeight(boolean value) {#setIntegralHeight-boolean-}
```
public void setIntegralHeight(boolean value)
```


يشير إلى ما إذا كان التحكم سيظهر فقط أسطر النص الكاملة دون إظهار أي أسطر جزئية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setLinkedCell(String value) {#setLinkedCell-java.lang.String-}
```
public void setLinkedCell(String value)
```


يضبط الخلية المرتبطة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setListFillRange(String value) {#setListFillRange-java.lang.String-}
```
public void setListFillRange(String value)
```


يضبط نطاق تعبئة القائمة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setListStyle(int value) {#setListStyle-int-}
```
public void setListStyle(int value)
```


يضبط المظهر البصري.

انظر [ControlListStyle](../../com.aspose.cells/controlliststyle).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setListWidth(double value) {#setListWidth-double-}
```
public void setListWidth(double value)
```


يضبط العرض بوحدة النقاط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


يشير إلى ما إذا كانت البيانات في التحكم مقفلة للتحرير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setMatchEntry(int value) {#setMatchEntry-int-}
```
public void setMatchEntry(int value)
```


يشير إلى كيفية بحث ListBox أو ComboBox في قائمته عندما يكتب المستخدم.

انظر [ControlMatchEntryType](../../com.aspose.cells/controlmatchentrytype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setMouseIcon(byte[] value) {#setMouseIcon-byte---}
```
public void setMouseIcon(byte[] value)
```


يضبط أيقونة مخصصة لتظهر كمؤشر الفأرة للتحكم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | byte[] |  |

### setMousePointer(int value) {#setMousePointer-int-}
```
public void setMousePointer(int value)
```


يضبط نوع الأيقونة المعروضة كمؤشر الفأرة للتحكم.

انظر [ControlMousePointerType](../../com.aspose.cells/controlmousepointertype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setScrollBars(int value) {#setScrollBars-int-}
```
public void setScrollBars(int value)
```


يشير إلى ما إذا كان التحكم يحتوي على أشرطة تمرير عمودية، أشرطة تمرير أفقية، كلاهما، أو لا شيء.

انظر [ControlScrollBarType](../../com.aspose.cells/controlscrollbartype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setSelectionType(int value) {#setSelectionType-int-}
```
public void setSelectionType(int value)
```


يشير إلى ما إذا كان التحكم يسمح بتحديدات متعددة.

انظر [SelectionType](../../com.aspose.cells/selectiontype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


يشير إلى ما إذا كان يجب إظهار الظل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowColumnHeads(boolean value) {#setShowColumnHeads-boolean-}
```
public void setShowColumnHeads(boolean value)
```


يشير إلى ما إذا كانت عناوين الأعمدة معروضة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSpecialEffect(int value) {#setSpecialEffect-int-}
```
public void setSpecialEffect(int value)
```


يضبط التأثير الخاص للتحكم.

انظر [ControlSpecialEffectType](../../com.aspose.cells/controlspecialeffecttype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTextAlign(int value) {#setTextAlign-int-}
```
public void setTextAlign(int value)
```


يمثل طريقة محاذاة النص المستخدم في التحكم.

انظر [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTextColumn(int value) {#setTextColumn-int-}
```
public void setTextColumn(int value)
```


يمثل العمود في ComboBox أو ListBox لعرضه للمستخدم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTransparent(boolean value) {#setTransparent-boolean-}
```
public void setTransparent(boolean value)
```


يشير إلى ما إذا كان التحكم شفافًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setValue(String value) {#setValue-java.lang.String-}
```
public void setValue(String value)
```


يضبط قيمة التحكم.

**Remarks**

يؤثر فقط عندما [getSelectionType()](../../com.aspose.cells/listboxactivexcontrol\#getSelectionType--) هو SelectionType.Single;

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


يشير إلى ما إذا كان هذا التحكم مرئيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```


يضبط عرض التحكم بوحدة النقاط.

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

