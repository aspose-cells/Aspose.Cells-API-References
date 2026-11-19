---
title: "GridShape"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل كائن شكل."
type: docs
url: /ar/java/com.aspose.gridweb/gridshape/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.gridweb.IGridSave
```
public class GridShape implements IGridSave
```

يمثل كائن شكل.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBuffer()](#getBuffer--) | يحصل على المخزن المؤقت للكائن. |
| [getClass()](#getClass--) |  |
| [getID()](#getID--) | يحصل على معرف المجموعات للشكل. |
| [getLeft()](#getLeft--) | يمثل الإزاحة الأفقية للشكل من عموده الأيسر، بوحدة البكسل. |
| [getLeftToCorner()](#getLeftToCorner--) | يمثل الإزاحة الأفقية للشكل من الحافة اليسرى لورقة العمل، بوحدة البكسل. |
| [getMsoDrawingType()](#getMsoDrawingType--) | يحصل على نوع رسم mso. |
| [getName()](#getName--) | يحصل على اسم الشكل. |
| [getText()](#getText--) | يمثل السلسلة في كائن TextBox هذا. |
| [getTop()](#getTop--) | يمثل الإزاحة العمودية للشكل من صفه العلوي، بوحدة البكسل. |
| [getTopToCorner()](#getTopToCorner--) | يمثل الإزاحة العمودية للشكل من الحافة العلوية لورقة العمل، بوحدة البكسل. |
| [getUpperLeftColumn()](#getUpperLeftColumn--) | يمثل فهرس عمود الزاوية العلوية اليسرى. |
| [getUpperLeftRow()](#getUpperLeftRow--) | يمثل فهرس الصف للزاوية العلوية اليسرى. |
| [getZOrderPosition()](#getZOrderPosition--) | يعيد موضع الشكل في ترتيب z. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [saveToImage(InputStream s)](#saveToImage-java.io.InputStream-) | ينشئ الصورة ويحفظها إلى تدفق بالتنسيق png المحدد. |
| [setID(String value)](#setID-java.lang.String-) | يحصل على معرف المجموعات للشكل. |
| [setLeftToCorner(int value)](#setLeftToCorner-int-) | يمثل الإزاحة الأفقية للشكل من الحافة اليسرى لورقة العمل، بوحدة البكسل. |
| [setText(String value)](#setText-java.lang.String-) | يمثل السلسلة في كائن TextBox هذا. |
| [setTopToCorner(int value)](#setTopToCorner-int-) | يمثل الإزاحة العمودية للشكل من الحافة العلوية لورقة العمل، بوحدة البكسل. |
| [setZOrderPosition(int value)](#setZOrderPosition-int-) | يعيد موضع الشكل في ترتيب z. |
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
### getBuffer() {#getBuffer--}
```
public byte[] getBuffer()
```


يحصل على المخزن المؤقت للكائن.

**Returns:**
byte[]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getID() {#getID--}
```
public String getID()
```


يحصل على معرف المجموعات للشكل.

**Returns:**
java.lang.String
### getLeft() {#getLeft--}
```
public int getLeft()
```


يمثل الإزاحة الأفقية للشكل من عموده الأيسر، بوحدة البكسل.

**Returns:**
int
### getLeftToCorner() {#getLeftToCorner--}
```
public int getLeftToCorner()
```


يمثل الإزاحة الأفقية للشكل من الحافة اليسرى لورقة العمل، بوحدة البكسل.

**Returns:**
int
### getMsoDrawingType() {#getMsoDrawingType--}
```
public int getMsoDrawingType()
```


يحصل على نوع رسم mso.

انظر [GridMsoDrawingType](../../com.aspose.gridweb/gridmsodrawingtype).

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


يحصل على اسم الشكل.

**Returns:**
java.lang.String
### getText() {#getText--}
```
public String getText()
```


يمثل السلسلة في كائن TextBox هذا.

**Returns:**
java.lang.String
### getTop() {#getTop--}
```
public int getTop()
```


يمثل الإزاحة العمودية للشكل من صفه العلوي، بوحدة البكسل.

**Remarks**

إذا كان الشكل داخل المخطط، يمثل الإزاحة العمودية للشكل من حدّه العلوي.

**Returns:**
int
### getTopToCorner() {#getTopToCorner--}
```
public int getTopToCorner()
```


يمثل الإزاحة العمودية للشكل من الحافة العلوية لورقة العمل، بوحدة البكسل.

**Returns:**
int
### getUpperLeftColumn() {#getUpperLeftColumn--}
```
public int getUpperLeftColumn()
```


يمثل فهرس عمود الزاوية العلوية اليسرى.

**Returns:**
int
### getUpperLeftRow() {#getUpperLeftRow--}
```
public int getUpperLeftRow()
```


يمثل فهرس الصف للزاوية العلوية اليسرى.

**Remarks**

إذا كان الشكل داخل شكل آخر أو داخل مجموعة، سيتم تجاهل UpperLeftRow.

**Returns:**
int
### getZOrderPosition() {#getZOrderPosition--}
```
public int getZOrderPosition()
```


يعيد موضع الشكل في ترتيب z.

**Returns:**
int
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




### saveToImage(InputStream s) {#saveToImage-java.io.InputStream-}
```
public void saveToImage(InputStream s)
```


ينشئ الصورة ويحفظها إلى تدفق بالتنسيق png المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| s | java.io.InputStream |  |

### setID(String value) {#setID-java.lang.String-}
```
public void setID(String value)
```


يحصل على معرف المجموعات للشكل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setLeftToCorner(int value) {#setLeftToCorner-int-}
```
public void setLeftToCorner(int value)
```


يمثل الإزاحة الأفقية للشكل من الحافة اليسرى لورقة العمل، بوحدة البكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


يمثل السلسلة في كائن TextBox هذا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setTopToCorner(int value) {#setTopToCorner-int-}
```
public void setTopToCorner(int value)
```


يمثل الإزاحة العمودية للشكل من الحافة العلوية لورقة العمل، بوحدة البكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setZOrderPosition(int value) {#setZOrderPosition-int-}
```
public void setZOrderPosition(int value)
```


يعيد موضع الشكل في ترتيب z.

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

