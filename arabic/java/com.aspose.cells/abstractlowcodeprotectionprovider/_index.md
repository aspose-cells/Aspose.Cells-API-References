---
title: "AbstractLowCodeProtectionProvider"
second_title: "Aspose.Cells for Java API Reference"
description: "تنفيذ لتوفير إعدادات الحماية"
type: docs
url: /ar/java/com.aspose.cells/abstractlowcodeprotectionprovider/
---

**Inheritance:**
java.lang.Object
```
public class AbstractLowCodeProtectionProvider
```

تنفيذ لتوفير إعدادات الحماية
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [AbstractLowCodeProtectionProvider()](#AbstractLowCodeProtectionProvider--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getOpenPassword()](#getOpenPassword--) | يحصل على كلمة المرور لفتح ملف جدول البيانات. |
| [getWorkbookPassword()](#getWorkbookPassword--) | يحصل على كلمة المرور لحماية المصنف بنوع الحماية المحدد. |
| [getWorkbookProtectionType()](#getWorkbookProtectionType--) | يحصل على نوع الحماية لحماية المصنف. |
| [getWorksheetPassword(String sheetName)](#getWorksheetPassword-java.lang.String-) | يحصل على كلمة المرور لحماية ورقة العمل المحددة. |
| [getWorksheetProtectionType(String sheetName)](#getWorksheetProtectionType-java.lang.String-) | يحصل على نوع الحماية لحماية ورقة العمل المحددة. |
| [getWritePassword()](#getWritePassword--) | يحصل على كلمة المرور لتعديل ملف جدول البيانات. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractLowCodeProtectionProvider() {#AbstractLowCodeProtectionProvider--}
```
public AbstractLowCodeProtectionProvider()
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
### getOpenPassword() {#getOpenPassword--}
```
public String getOpenPassword()
```


يحصل على كلمة المرور لفتح ملف جدول البيانات.

**Returns:**
java.lang.String - كلمة المرور لفتح ملف جدول البيانات. فارغ يعني عدم وجود حماية لفتح الملف.
### getWorkbookPassword() {#getWorkbookPassword--}
```
public String getWorkbookPassword()
```


يحصل على كلمة المرور لحماية المصنف بنوع الحماية المحدد.

**Returns:**
java.lang.String - كلمة المرور لحماية المصنف.
### getWorkbookProtectionType() {#getWorkbookProtectionType--}
```
public int getWorkbookProtectionType()
```


يحصل على نوع الحماية لحماية المصنف.

**Returns:**
int - [ProtectionType](../../com.aspose.cells/protectiontype). نوع الحماية لحماية المصنف. [ProtectionType.NONE](../../com.aspose.cells/protectiontype\#NONE) يعني عدم وجود حماية للمصنف.
### getWorksheetPassword(String sheetName) {#getWorksheetPassword-java.lang.String-}
```
public String getWorksheetPassword(String sheetName)
```


يحصل على كلمة المرور لحماية ورقة العمل المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetName | java.lang.String |  |

**Returns:**
java.lang.String - كلمة المرور لحماية ورقة العمل المحددة.
### getWorksheetProtectionType(String sheetName) {#getWorksheetProtectionType-java.lang.String-}
```
public int getWorksheetProtectionType(String sheetName)
```


يحصل على نوع الحماية لحماية ورقة العمل المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetName | java.lang.String |  |

**Returns:**
int - [ProtectionType](../../com.aspose.cells/protectiontype). نوع الحماية لحماية ورقة العمل المحددة. [ProtectionType.NONE](../../com.aspose.cells/protectiontype\#NONE) يعني عدم وجود حماية لورقة العمل.
### getWritePassword() {#getWritePassword--}
```
public String getWritePassword()
```


يحصل على كلمة المرور لتعديل ملف جدول البيانات.

**Returns:**
java.lang.String - كلمة المرور لتعديل ملف جدول البيانات. فارغ يعني عدم وجود حماية لتعديل الملف.
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

