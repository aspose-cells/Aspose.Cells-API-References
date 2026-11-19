---
title: "SpreadsheetSplitter"
second_title: "Aspose.Cells for Java API Reference"
description: "يقسم ملف جدول البيانات إلى عدة أجزاء."
type: docs
url: /ar/java/com.aspose.cells/spreadsheetsplitter/
---

**Inheritance:**
java.lang.Object
```
public class SpreadsheetSplitter
```

يقسم ملف جدول البيانات إلى عدة أجزاء.

**Example**

```
         SpreadsheetSplitter.process("template.xlsx", "split.xlsx");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [process(LowCodeSplitOptions options)](#process-com.aspose.cells.LowCodeSplitOptions-) | يقسم ملف جدول البيانات إلى عدة أجزاء. |
| [process(String templateFile, String resultFile)](#process-java.lang.String-java.lang.String-) | يقسم ملف القالب المحدد إلى عدة أجزاء. |
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
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### process(LowCodeSplitOptions options) {#process-com.aspose.cells.LowCodeSplitOptions-}
```
public static void process(LowCodeSplitOptions options)
```


يقسم ملف جدول البيانات إلى عدة أجزاء.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| options | [LowCodeSplitOptions](../../com.aspose.cells/lowcodesplitoptions) | خيارات تقسيم جدول البيانات |

### process(String templateFile, String resultFile) {#process-java.lang.String-java.lang.String-}
```
public static void process(String templateFile, String resultFile)
```


يقسم ملف القالب المحدد إلى عدة أجزاء.

**Remarks**

سيتم إنشاء ملفات الإخراج من الملف الناتج المحدد عن طريق إلحاق رقم تسلسلي للورقة والجزء المقسّم. على سبيل المثال، إذا كان ملف الإخراج المحدد هو Split.xlsx، فستكون الملفات المُنشأة Split\_0\_0.xlsx، Split\_0\_1.xlsx، ...، Split\_1\_0.xlsx، ...

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| templateFile | java.lang.String | ملف القالب الذي سيتم تقسيمه |
| resultFile | java.lang.String | الملف الناتج (نمط الاسم) |

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

