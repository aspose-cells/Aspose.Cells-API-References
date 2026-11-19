---
title: "ImageConverter"
second_title: "Aspose.Cells for Java API Reference"
description: "محول لتحويل ملف القالب إلى صور."
type: docs
url: /ar/java/com.aspose.cells/imageconverter/
---

**Inheritance:**
java.lang.Object
```
public class ImageConverter
```

محول لتحويل ملف القالب إلى صور.

**Example**

```
         ImageConverter.process("template.xlsx", "res.png");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)](#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-) | يحوّل ملف القالب إلى صور |
| [process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeSaveOptionsProvider provider)](#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-com.aspose.cells.AbstractLowCodeSaveOptionsProvider-) | يحوّل ملف القالب إلى صور |
| [process(String templateFile, String resultFile)](#process-java.lang.String-java.lang.String-) | يحوّل ملف القالب إلى صور. |
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


يحوّل ملف القالب إلى صور

**Remarks**

عند التحويل إلى صورة بصيغة تدعم صفحات متعددة (مثل tiff)، سيتم استخدام [LowCodeSaveOptions.getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) أو [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--) المحددين مباشرةً للصورة الناتجة.

بالنسبة لأنواع الصور الأخرى، إذا حددت خيارات الحفظ Stream كمخرج، فسيتم حفظ جميع الصور الناتجة إلى نفس الـ Stream. وإلا، سيتم إنشاء ملفات الإخراج من ملف الإخراج المحدد في خيارات الحفظ عن طريق إلحاق رقم تسلسلي للورقة والجزء المقسّم. على سبيل المثال، إذا كان ملف الإخراج المحدد هو Image.png، فستكون ملفات الصور المولدة Image\_0\_0.png، Image\_0\_1.png، …، Image\_1\_0.png، …

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| loadOptions | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | خيارات الإدخال والتحميل |
| saveOptions | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | خيارات الإخراج والحفظ |

### process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeSaveOptionsProvider provider) {#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-com.aspose.cells.AbstractLowCodeSaveOptionsProvider-}
```
public static void process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeSaveOptionsProvider provider)
```


يحوّل ملف القالب إلى صور

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| loadOptions | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | خيارات الإدخال والتحميل |
| saveOptions | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | خيارات الحفظ. مخرجاته ([LowCodeSaveOptions.getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) أو [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--)) لا تأثير لها لأن جميع المخرجات سيتم تحديدها بواسطة معامل \"provider\". |
| provider | [AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider) | مزوّد خيارات الحفظ لحفظ الصور المولدة |

### process(String templateFile, String resultFile) {#process-java.lang.String-java.lang.String-}
```
public static void process(String templateFile, String resultFile)
```


يحوّل ملف القالب إلى صور.

**Remarks**

ستُبنى ملفات الإخراج من ملف النتيجة المحدد عن طريق إلحاق رقم تسلسلي للورقة والجزء المقسّم. على سبيل المثال، إذا كان ملف الإخراج المحدد هو Image.png، فستكون ملفات الصور المولدة Image\_0\_0.png، Image\_0\_1.png، …، Image\_1\_0.png، …

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| templateFile | java.lang.String | ملف القالب الذي سيتم تحويله إلى صور. |
| resultFile | java.lang.String | ملف النتيجة (نمط الاسم) للصور المولدة. |

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

