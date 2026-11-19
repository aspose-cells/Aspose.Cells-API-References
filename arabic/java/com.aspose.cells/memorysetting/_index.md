---
title: "MemorySetting"
second_title: "Aspose.Cells for Java API Reference"
description: "أنماط استخدام الذاكرة لنموذج بيانات الخلايا."
type: docs
url: /ar/java/com.aspose.cells/memorysetting/
---

**Inheritance:**
java.lang.Object
```
public final class MemorySetting
```

أنماط استخدام الذاكرة لنموذج بيانات الخلايا.
## حقول

| حقل | الوصف |
| --- | --- |
| [FILE_CACHE](#FILE-CACHE) | يفضل أداء الذاكرة واستخدام ملف بدلاً من الذاكرة للحفاظ على بيانات الخلايا. |
| [MEMORY_PREFERENCE](#MEMORY-PREFERENCE) | يفضل أداء الذاكرة. |
| [NORMAL](#NORMAL) | الوضع الافتراضي لنموذج الخلايا. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### FILE_CACHE {#FILE-CACHE}
```
public static final int FILE_CACHE
```


يفضل أداء الذاكرة واستخدام ملف بدلاً من الذاكرة للحفاظ على بيانات الخلايا.

**Remarks**

مع هذا الوضع، سيتم الحفاظ على بيانات الخلايا بتنسيق مضغوط وسيتم الحفاظ على الجزء الأكبر من البيانات في ملف مؤقت بدلاً من الذاكرة. لذا عند المقارنة مع وضع [MEMORY\_PREFERENCE](../../com.aspose.cells/memorysetting\#MEMORY-PREFERENCE)، قد يقلل هذا الوضع من استهلاك الذاكرة أكثر، لكن عمليات الإدخال/الإخراج للوصول إلى بيانات الخلايا ستسبب أيضاً تكلفة زمنية أعلى.

هذا الخيار متاح منذ الإصدار v25.7.0.

| بعض الحدود الملحوظة والعمليات الموصى بها عند استخدام هذا الوضع: |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| عند استخدام هذا الوضع لأي ورقة عمل في دفتر واحد، يجب استدعاء [Workbook.dispose()](../../com.aspose.cells/workbook\#dispose--) في نهاية العمل لإطلاق جميع الموارد مثل الملفات المؤقتة. |
| الوصول العشوائي إلى الخلايا سيؤدي إلى أداء ضعيف لأن البيانات تحتاج إلى القراءة عشوائياً وبشكل متكرر (لذلك سيتغير المؤشر في الملف وفقاً لذلك وستُطلب عمليات الإدخال/الإخراج بشكل متكرر). إذا أمكن، يرجى دائماً الوصول إلى البيانات بشكل متسلسل (صفاً بصف). |
| عند تغيير بيانات صف/خلية واحدة، قد تتأثر بيانات الخلايا/الصفوف الأخرى (مثل تحريك البيانات إلى أماكن أخرى لتخصيص مساحة كافية للبيانات المتغيرة). لذا كل تغيير في أي بيانات يتطلب مزامنة الكائنات الموجودة الأخرى (مثل كائن الصف أو الخلية). لذلك، للحصول على أداء أفضل، يرجى عدم الحفاظ على عدة صفوف/خلايا في نفس الوقت. معالجة كل منها على حدة سيقلل من مزامنة البيانات وبالتالي يمكن تحسين الأداء. |

### MEMORY_PREFERENCE {#MEMORY-PREFERENCE}
```
public static final int MEMORY_PREFERENCE
```


يفضل أداء الذاكرة.

**Remarks**

مع هذا الوضع، سيتم الحفاظ على بيانات الخلايا بتنسيق مضغوط لتقليل استهلاك الذاكرة. من ناحية أخرى، قد يتسبب التنسيق المضغوط في تكلفة زمنية أعلى، خاصةً عند تحديث بيانات الخلايا أو الوصول إليها عشوائياً.

هذا الخيار متاح منذ الإصدار v8.0.0.

### NORMAL {#NORMAL}
```
public static final int NORMAL
```


الوضع الافتراضي لنموذج الخلايا.

**Remarks**

يُطبق هذا الوضع على جميع الإصدارات.

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

