---
title: "TextConverter"
second_title: "Aspose.Cells for Java API Reference"
description: "محول للتحويل بين صيغ النص مثل csv و tsv و dif... وغيرها من صيغ ملفات الجداول."
type: docs
url: /ar/java/com.aspose.cells/textconverter/
---

**Inheritance:**
java.lang.Object
```
public class TextConverter
```

محول للتحويل بين الصيغ المعتمدة على النص (csv، tsv، dif ...) وصيغ ملفات جداول البيانات الأخرى.

**Example**

```
         TextConverter.process("template.csv", "res.xlsx");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)](#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-) | يقوم بتحويل صيغ الملفات بين صيغ النص وغيرها من صيغ ملفات الجداول. |
| [process(String templateFile, String resultFile)](#process-java.lang.String-java.lang.String-) | يقوم بتحويل ملف القالب المحدد بين ملفات النص وغيرها من الصيغ. |
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




### process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions) {#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-}
```
public static void process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```


يقوم بتحويل صيغ الملفات بين صيغ النص وغيرها من صيغ ملفات الجداول.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| loadOptions | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | خيارات الإدخال والتحميل |
| saveOptions | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | خيارات الإخراج والحفظ |

### process(String templateFile, String resultFile) {#process-java.lang.String-java.lang.String-}
```
public static void process(String templateFile, String resultFile)
```


يقوم بتحويل ملف القالب المحدد بين ملفات النص وغيرها من الصيغ.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| templateFile | java.lang.String | ملف القالب المراد تحويله |
| resultFile | java.lang.String | الملف الناتج |

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

