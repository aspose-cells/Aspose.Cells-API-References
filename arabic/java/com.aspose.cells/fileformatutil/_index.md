---
title: "FileFormatUtil"
second_title: "Aspose.Cells for Java API Reference"
description: "يوفر طرقًا مساعدة لتحويل تعداد تنسيق الملف إلى سلاسل أو امتدادات ملفات والعكس."
type: docs
url: /ar/java/com.aspose.cells/fileformatutil/
---

**Inheritance:**
java.lang.Object
```
public class FileFormatUtil
```

يوفر طرقًا مساعدة لتحويل تعداد تنسيق الملف إلى سلاسل أو امتدادات ملفات والعكس.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [detectFileFormat(InputStream stream)](#detectFileFormat-java.io.InputStream-) | يكشف ويعيد المعلومات حول تنسيق ملف إكسل المخزن في تدفق. |
| [detectFileFormat(InputStream stream, String password)](#detectFileFormat-java.io.InputStream-java.lang.String-) | يكشف ويعيد المعلومات حول تنسيق ملف إكسل المخزن في تدفق. |
| [detectFileFormat(String filePath)](#detectFileFormat-java.lang.String-) | يكشف ويعيد المعلومات حول تنسيق ملف إكسل المخزن في ملف. |
| [detectFileFormat(String filePath, String password)](#detectFileFormat-java.lang.String-java.lang.String-) | يكشف ويعيد المعلومات حول تنسيق ملف إكسل المخزن في ملف. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [extensionToSaveFormat(String extension)](#extensionToSaveFormat-java.lang.String-) | يحوّل امتداد اسم الملف إلى قيمة SaveFormat. |
| [fileFormatToSaveFormat(int format)](#fileFormatToSaveFormat-int-) | تحويل تنسيق الملف إلى تنسيق حفظ. |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [isTemplateFormat(String extension)](#isTemplateFormat-java.lang.String-) | يرجع true إذا كان الامتداد .xlt أو .xltX أو .xltm أو .ots. |
| [loadFormatToExtension(int loadFormat)](#loadFormatToExtension-int-) | يحوّل قيمة تعداد تنسيق التحميل إلى امتداد ملف. |
| [loadFormatToSaveFormat(int loadFormat)](#loadFormatToSaveFormat-int-) | يحوّل قيمة LoadFormat إلى قيمة SaveFormat إذا كان ذلك ممكنًا. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [saveFormatToExtension(int format)](#saveFormatToExtension-int-) | يحوّل قيمة تعداد تنسيق الحفظ إلى امتداد ملف. |
| [saveFormatToLoadFormat(int saveFormat)](#saveFormatToLoadFormat-int-) | يحوّل قيمة SaveFormat إلى قيمة LoadFormat إذا كان ذلك ممكنًا. |
| [toString()](#toString--) |  |
| [verifyPassword(InputStream stream, String password)](#verifyPassword-java.io.InputStream-java.lang.String-) | يكشف ويعيد المعلومات حول تنسيق ملف إكسل المخزن في تدفق. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### detectFileFormat(InputStream stream) {#detectFileFormat-java.io.InputStream-}
```
public static FileFormatInfo detectFileFormat(InputStream stream)
```


يكشف ويعيد المعلومات حول تنسيق ملف إكسل المخزن في تدفق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.InputStream | التدفق |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
### detectFileFormat(InputStream stream, String password) {#detectFileFormat-java.io.InputStream-java.lang.String-}
```
public static FileFormatInfo detectFileFormat(InputStream stream, String password)
```


يكشف ويعيد المعلومات حول تنسيق ملف إكسل المخزن في تدفق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.InputStream |  |
| password | java.lang.String | كلمة المرور للملفات ooxml المشفرة. |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
### detectFileFormat(String filePath) {#detectFileFormat-java.lang.String-}
```
public static FileFormatInfo detectFileFormat(String filePath)
```


يكشف ويعيد المعلومات حول تنسيق ملف إكسل المخزن في ملف.

**Remarks**

يدعم فقط فحص بعض الملفات ذات التوقيع السحري. إذا لم يكن هناك توقيع سحري، لا يمكننا اكتشاف تنسيق الملف بدقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| filePath | java.lang.String | مسار الملف. |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
### detectFileFormat(String filePath, String password) {#detectFileFormat-java.lang.String-java.lang.String-}
```
public static FileFormatInfo detectFileFormat(String filePath, String password)
```


يكشف ويعيد المعلومات حول تنسيق ملف إكسل المخزن في ملف.

**Remarks**

يدعم فقط فحص بعض الملفات ذات التوقيع السحري. إذا لم يكن هناك توقيع سحري، لا يمكننا اكتشاف تنسيق الملف بدقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| filePath | java.lang.String | مسار الملف. |
| password | java.lang.String | كلمة المرور للملفات ooxml المشفرة. |

**Returns:**
[FileFormatInfo](../../com.aspose.cells/fileformatinfo) - A [FileFormatInfo](../../com.aspose.cells/fileformatinfo) object that contains the detected information.
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
### extensionToSaveFormat(String extension) {#extensionToSaveFormat-java.lang.String-}
```
public static int extensionToSaveFormat(String extension)
```


يحوّل امتداد اسم الملف إلى قيمة SaveFormat.

**Remarks**

إذا لم يتم التعرف على الامتداد، تُرجع [SaveFormat.UNKNOWN](../../com.aspose.cells/saveformat\#UNKNOWN).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| extension | java.lang.String | امتداد الملف. يمكن أن يكون مع أو بدون نقطة بادئة. غير حساس لحالة الأحرف. |

**Returns:**
int - [SaveFormat](../../com.aspose.cells/saveformat).
### fileFormatToSaveFormat(int format) {#fileFormatToSaveFormat-int-}
```
public static int fileFormatToSaveFormat(int format)
```


تحويل تنسيق الملف إلى تنسيق حفظ.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| format | int | [FileFormatType](../../com.aspose.cells/fileformattype). نوع تنسيق الملف. |

**Returns:**
int - [SaveFormat](../../com.aspose.cells/saveformat).
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
### isTemplateFormat(String extension) {#isTemplateFormat-java.lang.String-}
```
public static boolean isTemplateFormat(String extension)
```


يرجع true إذا كان الامتداد .xlt أو .xltX أو .xltm أو .ots.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| extension | java.lang.String |  |

**Returns:**
boolean -
### loadFormatToExtension(int loadFormat) {#loadFormatToExtension-int-}
```
public static String loadFormatToExtension(int loadFormat)
```


يحوّل قيمة تعداد تنسيق التحميل إلى امتداد ملف.

**Remarks**

إذا تعذر تحويله، تُرجع null.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| loadFormat | int | [LoadFormat](../../com.aspose.cells/loadformat). تنسيق الملف المحمّل. |

**Returns:**
java.lang.String - الامتداد المُرجع هو سلسلة بأحرف صغيرة مع نقطة بادئة.
### loadFormatToSaveFormat(int loadFormat) {#loadFormatToSaveFormat-int-}
```
public static int loadFormatToSaveFormat(int loadFormat)
```


يحوّل قيمة LoadFormat إلى قيمة SaveFormat إذا كان ذلك ممكنًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| loadFormat | int | [LoadFormat](../../com.aspose.cells/loadformat). تنسيق التحميل. |

**Returns:**
int - [SaveFormat](../../com.aspose.cells/saveformat). تنسيق الحفظ.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### saveFormatToExtension(int format) {#saveFormatToExtension-int-}
```
public static String saveFormatToExtension(int format)
```


يحوّل قيمة تعداد تنسيق الحفظ إلى امتداد ملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| format | int | [SaveFormat](../../com.aspose.cells/saveformat). تنسيق الحفظ. |

**Returns:**
java.lang.String - الامتداد المُرجع هو سلسلة بأحرف صغيرة مع نقطة بادئة.
### saveFormatToLoadFormat(int saveFormat) {#saveFormatToLoadFormat-int-}
```
public static int saveFormatToLoadFormat(int saveFormat)
```


يحوّل قيمة SaveFormat إلى قيمة LoadFormat إذا كان ذلك ممكنًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). تنسيق الحفظ. |

**Returns:**
int - [LoadFormat](../../com.aspose.cells/loadformat). تنسيق التحميل
### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### verifyPassword(InputStream stream, String password) {#verifyPassword-java.io.InputStream-java.lang.String-}
```
public static boolean verifyPassword(InputStream stream, String password)
```


يكشف ويعيد المعلومات حول تنسيق ملف إكسل المخزن في تدفق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.InputStream |  |
| password | java.lang.String | كلمة المرور للملفات ooxml المشفرة. |

**Returns:**
boolean - يُرجع ما إذا كانت كلمة المرور مصححة.
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

