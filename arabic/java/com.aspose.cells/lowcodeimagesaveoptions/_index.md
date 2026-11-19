---
title: "LowCodeImageSaveOptions"
second_title: "Aspose.Cells for Java API Reference"
description: "خيارات حفظ الصورة بطريقة منخفضة الكود."
type: docs
url: /ar/java/com.aspose.cells/lowcodeimagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
```
public class LowCodeImageSaveOptions extends LowCodeSaveOptions
```

خيارات حفظ الصورة بطريقة منخفضة الكود.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [LowCodeImageSaveOptions()](#LowCodeImageSaveOptions--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getImageOptions()](#getImageOptions--) | الخيارات لتصيير الصور. |
| [getOutputFile()](#getOutputFile--) | يحصل على الملف (مع المسار إذا لزم) لحفظ البيانات المولدة. |
| [getOutputStream()](#getOutputStream--) | يحصل على الدفق لكتابة البيانات المولدة إليه. |
| [getSaveFormat()](#getSaveFormat--) | يحصل على تنسيق الحفظ. |
| [getSaveOptionsProvider()](#getSaveOptionsProvider--) | مزود خيارات الحفظ لحفظ الصور المُولدة. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setImageOptions(ImageOrPrintOptions value)](#setImageOptions-com.aspose.cells.ImageOrPrintOptions-) | الخيارات لتصيير الصور. |
| [setOutputFile(String value)](#setOutputFile-java.lang.String-) | يضبط الملف (مع المسار إذا لزم) لحفظ البيانات المولدة. |
| [setOutputStream(InputStream value)](#setOutputStream-java.io.InputStream-) | يضبط الدفق لكتابة البيانات المولدة إليه. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | يضبط تنسيق الحفظ. |
| [setSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider value)](#setSaveOptionsProvider-com.aspose.cells.AbstractLowCodeSaveOptionsProvider-) | مزود خيارات الحفظ لحفظ الصور المُولدة. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeImageSaveOptions() {#LowCodeImageSaveOptions--}
```
public LowCodeImageSaveOptions()
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
### getImageOptions() {#getImageOptions--}
```
public ImageOrPrintOptions getImageOptions()
```


الخيارات لتصيير الصور.

**Remarks**

عند تحديد مثيل واحد من [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)، سيتم استبدال [getSaveFormat()](../../com.aspose.cells/lowcodeimagesaveoptions\#getSaveFormat--) (إذا كان قد تم تحديده مسبقًا).

**Returns:**
[ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)
### getOutputFile() {#getOutputFile--}
```
public String getOutputFile()
```


يحصل على الملف (مع المسار إذا لزم) لحفظ البيانات المولدة. عند ضبط هذه الخاصية بقيمة غير null أو سلسلة فارغة، سيتم تجاهل [getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--).

**Returns:**
java.lang.String
### getOutputStream() {#getOutputStream--}
```
public InputStream getOutputStream()
```


يحصل على الدفق لكتابة البيانات المولدة إليه. عند ضبط هذه الخاصية بقيمة غير null، سيتم تجاهل [getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--).

**Returns:**
java.io.InputStream
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


يحصل على تنسيق الحفظ.

انظر [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

إذا تم تحديد [getImageOptions()](../../com.aspose.cells/lowcodeimagesaveoptions\#getImageOptions--)، فإن ضبط هذه الخاصية سيغير أيضًا قيمة [ImageOrPrintOptions.getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--) الخاصة به.

**Returns:**
int
### getSaveOptionsProvider() {#getSaveOptionsProvider--}
```
public AbstractLowCodeSaveOptionsProvider getSaveOptionsProvider()
```


مزود خيارات الحفظ لحفظ الصور المُولدة.

**Remarks**

الإخراج ([LowCodeSaveOptions.getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) أو [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--)) المحدد بواسطة هذه المثيلة لن يكون له أي تأثير عند تحديد هذه الخاصية. بدلاً من ذلك، سيتم تحديد إخراج كل صورة مُولدة بواسطة الموفر.

**Returns:**
[AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider)
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




### setImageOptions(ImageOrPrintOptions value) {#setImageOptions-com.aspose.cells.ImageOrPrintOptions-}
```
public void setImageOptions(ImageOrPrintOptions value)
```


الخيارات لتصيير الصور.

**Remarks**

عند تحديد مثيل واحد من [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)، سيتم استبدال [getSaveFormat()](../../com.aspose.cells/lowcodeimagesaveoptions\#getSaveFormat--) (إذا كان قد تم تحديده مسبقًا).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) |  |

### setOutputFile(String value) {#setOutputFile-java.lang.String-}
```
public void setOutputFile(String value)
```


يضبط الملف (مع المسار إذا لزم) لحفظ البيانات المولدة. عند ضبط هذه الخاصية بقيمة غير null أو سلسلة فارغة، سيتم تجاهل [getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setOutputStream(InputStream value) {#setOutputStream-java.io.InputStream-}
```
public void setOutputStream(InputStream value)
```


يضبط الدفق لكتابة البيانات المولدة إليه. عند ضبط هذه الخاصية بقيمة غير null، سيتم تجاهل [getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.io.InputStream |  |

### setSaveFormat(int value) {#setSaveFormat-int-}
```
public void setSaveFormat(int value)
```


يضبط تنسيق الحفظ.

انظر [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

إذا تم تحديد [getImageOptions()](../../com.aspose.cells/lowcodeimagesaveoptions\#getImageOptions--)، فإن ضبط هذه الخاصية سيغير أيضًا قيمة [ImageOrPrintOptions.getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--) الخاصة به.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider value) {#setSaveOptionsProvider-com.aspose.cells.AbstractLowCodeSaveOptionsProvider-}
```
public void setSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider value)
```


مزود خيارات الحفظ لحفظ الصور المُولدة.

**Remarks**

الإخراج ([LowCodeSaveOptions.getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) أو [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--)) المحدد بواسطة هذه المثيلة لن يكون له أي تأثير عند تحديد هذه الخاصية. بدلاً من ذلك، سيتم تحديد إخراج كل صورة مُولدة بواسطة الموفر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider) |  |

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

