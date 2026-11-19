---
title: "ActiveXControlBase"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل عنصر التحكم ActiveX."
type: docs
url: /ar/java/com.aspose.cells/activexcontrolbase/
---

**Inheritance:**
java.lang.Object
```
public abstract class ActiveXControlBase
```

يمثل عنصر التحكم ActiveX.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackOleColor()](#getBackOleColor--) | يحصل على لون ole للخلفية. |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | يحصل على البيانات الثنائية للتحكم. |
| [getForeOleColor()](#getForeOleColor--) | يحصل على لون OLE للمقدمة. |
| [getHeight()](#getHeight--) | يحصل على ارتفاع التحكم بوحدة النقاط. |
| [getLinkedCell()](#getLinkedCell--) | يحصل على الخلية المرتبطة. |
| [getListFillRange()](#getListFillRange--) | يحصل على نطاق تعبئة القائمة. |
| [getMouseIcon()](#getMouseIcon--) | يحصل على أيقونة مخصصة لعرضها كمؤشر الفأرة للتحكم. |
| [getMousePointer()](#getMousePointer--) | يحصل على نوع الأيقونة المعروضة كمؤشر الفأرة للتحكم. |
| [getShadow()](#getShadow--) | يشير إلى ما إذا كان يجب إظهار الظل. |
| [getType()](#getType--) | يحصل على نوع عنصر التحكم ActiveX. |
| [getWidth()](#getWidth--) | يحصل على عرض التحكم بوحدة النقاط. |
| [getWorkbook()](#getWorkbook--) | يحصل على كائن [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--). |
| [hashCode()](#hashCode--) |  |
| [isVisible()](#isVisible--) | يشير إلى ما إذا كان هذا التحكم مرئيًا. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackOleColor(int value)](#setBackOleColor-int-) | يضبط لون OLE للخلفية. |
| [setForeOleColor(int value)](#setForeOleColor-int-) | يضبط لون OLE للمقدمة. |
| [setHeight(double value)](#setHeight-double-) | يضبط ارتفاع التحكم بوحدة النقاط. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | يضبط الخلية المرتبطة. |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | يضبط نطاق تعبئة القائمة. |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | يضبط أيقونة مخصصة لتظهر كمؤشر الفأرة للتحكم. |
| [setMousePointer(int value)](#setMousePointer-int-) | يضبط نوع الأيقونة المعروضة كمؤشر الفأرة للتحكم. |
| [setShadow(boolean value)](#setShadow-boolean-) | يشير إلى ما إذا كان يجب إظهار الظل. |
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
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


يشير إلى ما إذا كان يجب إظهار الظل.

**Returns:**
boolean
### getType() {#getType--}
```
public abstract int getType()
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




### setBackOleColor(int value) {#setBackOleColor-int-}
```
public void setBackOleColor(int value)
```


يضبط لون OLE للخلفية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

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

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


يشير إلى ما إذا كان يجب إظهار الظل.

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

