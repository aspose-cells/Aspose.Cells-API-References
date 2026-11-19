---
title: "LabelActiveXControl"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل عنصر التحكم ActiveX للتسمية."
type: docs
url: /ar/java/com.aspose.cells/labelactivexcontrol/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ActiveXControlBase](../../com.aspose.cells/activexcontrolbase), [com.aspose.cells.ActiveXControl](../../com.aspose.cells/activexcontrol)
```
public class LabelActiveXControl extends ActiveXControl
```

يمثل عنصر التحكم ActiveX للتسمية.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAccelerator()](#getAccelerator--) | يحصل على مفتاح الاختصار للعنصر. |
| [getBackOleColor()](#getBackOleColor--) | يحصل على لون ole للخلفية. |
| [getBorderOleColor()](#getBorderOleColor--) | يحصل على لون ole للخلفية. |
| [getBorderStyle()](#getBorderStyle--) | يحصل على نوع الحد المستخدم من قبل التحكم. |
| [getCaption()](#getCaption--) | يحصل على النص الوصفي الذي يظهر على العنصر. |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | يحصل على البيانات الثنائية للتحكم. |
| [getFont()](#getFont--) | يمثل خط التحكم. |
| [getForeOleColor()](#getForeOleColor--) | يحصل على لون OLE للمقدمة. |
| [getHeight()](#getHeight--) | يحصل على ارتفاع التحكم بوحدة النقاط. |
| [getIMEMode()](#getIMEMode--) | يحصل على وضع التشغيل الافتراضي لمحرر طريقة الإدخال للتحكم عند استلامه للتركيز. |
| [getLinkedCell()](#getLinkedCell--) | يحصل على الخلية المرتبطة. |
| [getListFillRange()](#getListFillRange--) | يحصل على نطاق تعبئة القائمة. |
| [getMouseIcon()](#getMouseIcon--) | يحصل على أيقونة مخصصة لعرضها كمؤشر الفأرة للتحكم. |
| [getMousePointer()](#getMousePointer--) | يحصل على نوع الأيقونة المعروضة كمؤشر الفأرة للتحكم. |
| [getPicture()](#getPicture--) | يحصل على بيانات الصورة. |
| [getPicturePosition()](#getPicturePosition--) | يحصل على موقع صورة العنصر بالنسبة لتسميته. |
| [getShadow()](#getShadow--) | يشير إلى ما إذا كان يجب إظهار الظل. |
| [getSpecialEffect()](#getSpecialEffect--) | يحصل على التأثير الخاص للتحكم. |
| [getTextAlign()](#getTextAlign--) | يمثل طريقة محاذاة النص المستخدم في التحكم. |
| [getType()](#getType--) | يحصل على نوع عنصر التحكم ActiveX. |
| [getWidth()](#getWidth--) | يحصل على عرض التحكم بوحدة النقاط. |
| [getWorkbook()](#getWorkbook--) | يحصل على كائن [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--). |
| [hashCode()](#hashCode--) |  |
| [isAutoSize()](#isAutoSize--) | يشير إلى ما إذا كان التحكم سيعيد تحجيمه تلقائيًا لعرض محتوياته بالكامل. |
| [isEnabled()](#isEnabled--) | يشير إلى ما إذا كان التحكم يمكنه استلام التركيز والاستجابة للأحداث التي يولدها المستخدم. |
| [isLocked()](#isLocked--) | يشير إلى ما إذا كانت البيانات في التحكم مقفلة للتحرير. |
| [isTransparent()](#isTransparent--) | يشير إلى ما إذا كان التحكم شفافًا. |
| [isVisible()](#isVisible--) | يشير إلى ما إذا كان هذا التحكم مرئيًا. |
| [isWordWrapped()](#isWordWrapped--) | يشير إلى ما إذا كانت محتويات العنصر تُلتف تلقائيًا في نهاية السطر. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAccelerator(char value)](#setAccelerator-char-) | يضبط مفتاح الاختصار للعنصر. |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | يشير إلى ما إذا كان التحكم سيعيد تحجيمه تلقائيًا لعرض محتوياته بالكامل. |
| [setBackOleColor(int value)](#setBackOleColor-int-) | يضبط لون OLE للخلفية. |
| [setBorderOleColor(int value)](#setBorderOleColor-int-) | يضبط لون OLE للخلفية. |
| [setBorderStyle(int value)](#setBorderStyle-int-) | يضبط نوع الحد المستخدم من قبل التحكم. |
| [setCaption(String value)](#setCaption-java.lang.String-) | يضبط النص الوصفي الذي يظهر على العنصر. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | يشير إلى ما إذا كان التحكم يمكنه استلام التركيز والاستجابة للأحداث التي يولدها المستخدم. |
| [setForeOleColor(int value)](#setForeOleColor-int-) | يضبط لون OLE للمقدمة. |
| [setHeight(double value)](#setHeight-double-) | يضبط ارتفاع التحكم بوحدة النقاط. |
| [setIMEMode(int value)](#setIMEMode-int-) | يضبط وضع التشغيل الافتراضي لمحرر طريقة الإدخال للتحكم عند استلامه للتركيز. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | يضبط الخلية المرتبطة. |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | يضبط نطاق تعبئة القائمة. |
| [setLocked(boolean value)](#setLocked-boolean-) | يشير إلى ما إذا كانت البيانات في التحكم مقفلة للتحرير. |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | يضبط أيقونة مخصصة لتظهر كمؤشر الفأرة للتحكم. |
| [setMousePointer(int value)](#setMousePointer-int-) | يضبط نوع الأيقونة المعروضة كمؤشر الفأرة للتحكم. |
| [setPicture(byte[] value)](#setPicture-byte---) | يضبط بيانات الصورة. |
| [setPicturePosition(int value)](#setPicturePosition-int-) | يضبط موقع صورة العنصر بالنسبة لتسميته. |
| [setShadow(boolean value)](#setShadow-boolean-) | يشير إلى ما إذا كان يجب إظهار الظل. |
| [setSpecialEffect(int value)](#setSpecialEffect-int-) | يضبط التأثير الخاص للتحكم. |
| [setTextAlign(int value)](#setTextAlign-int-) | يمثل طريقة محاذاة النص المستخدم في التحكم. |
| [setTransparent(boolean value)](#setTransparent-boolean-) | يشير إلى ما إذا كان التحكم شفافًا. |
| [setVisible(boolean value)](#setVisible-boolean-) | يشير إلى ما إذا كان هذا التحكم مرئيًا. |
| [setWidth(double value)](#setWidth-double-) | يضبط عرض التحكم بوحدة النقاط. |
| [setWordWrapped(boolean value)](#setWordWrapped-boolean-) | يشير إلى ما إذا كانت محتويات العنصر تُلتف تلقائيًا في نهاية السطر. |
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
### getAccelerator() {#getAccelerator--}
```
public char getAccelerator()
```


يحصل على مفتاح الاختصار للعنصر.

**Returns:**
char
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
### getCaption() {#getCaption--}
```
public String getCaption()
```


يحصل على النص الوصفي الذي يظهر على العنصر.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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
### getPicture() {#getPicture--}
```
public byte[] getPicture()
```


يحصل على بيانات الصورة.

**Returns:**
byte[]
### getPicturePosition() {#getPicturePosition--}
```
public int getPicturePosition()
```


يحصل على موقع صورة العنصر بالنسبة لتسميته.

انظر [ControlPicturePositionType](../../com.aspose.cells/controlpicturepositiontype).

**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


يشير إلى ما إذا كان يجب إظهار الظل.

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
### getType() {#getType--}
```
public int getType()
```


يحصل على نوع عنصر التحكم ActiveX.

انظر [ControlType](../../com.aspose.cells/controltype).

**Returns:**
int
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
### isWordWrapped() {#isWordWrapped--}
```
public boolean isWordWrapped()
```


يشير إلى ما إذا كانت محتويات العنصر تُلتف تلقائيًا في نهاية السطر.

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




### setAccelerator(char value) {#setAccelerator-char-}
```
public void setAccelerator(char value)
```


يضبط مفتاح الاختصار للعنصر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | char |  |

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

### setCaption(String value) {#setCaption-java.lang.String-}
```
public void setCaption(String value)
```


يضبط النص الوصفي الذي يظهر على العنصر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

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

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


يشير إلى ما إذا كانت البيانات في التحكم مقفلة للتحرير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

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

### setPicture(byte[] value) {#setPicture-byte---}
```
public void setPicture(byte[] value)
```


يضبط بيانات الصورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | byte[] |  |

### setPicturePosition(int value) {#setPicturePosition-int-}
```
public void setPicturePosition(int value)
```


يضبط موقع صورة العنصر بالنسبة لتسميته.

انظر [ControlPicturePositionType](../../com.aspose.cells/controlpicturepositiontype).

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

### setTransparent(boolean value) {#setTransparent-boolean-}
```
public void setTransparent(boolean value)
```


يشير إلى ما إذا كان التحكم شفافًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

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

### setWordWrapped(boolean value) {#setWordWrapped-boolean-}
```
public void setWordWrapped(boolean value)
```


يشير إلى ما إذا كانت محتويات العنصر تُلتف تلقائيًا في نهاية السطر.

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

