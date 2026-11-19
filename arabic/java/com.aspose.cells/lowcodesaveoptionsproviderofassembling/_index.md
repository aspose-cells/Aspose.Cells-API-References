---
title: "LowCodeSaveOptionsProviderOfAssembling"
second_title: "Aspose.Cells for Java API Reference"
description: "تنفيذ لتوفير خيارات الحفظ التي تحفظ الأجزاء المقسمة إلى ملفات والمسار للملف الناتج يُسمّى كما قد يحتوي على أدلة SheetIndex أو SheetName أو SplitPartIndex."
type: docs
url: /ar/java/com.aspose.cells/lowcodesaveoptionsproviderofassembling/
---

**Inheritance:**
java.lang.Object، [com.aspose.cells.AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider)
```
public class LowCodeSaveOptionsProviderOfAssembling extends AbstractLowCodeSaveOptionsProvider
```

تنفيذ لتوفير خيارات الحفظ التي تحفظ الأجزاء المقسمة إلى ملفات والمسار للملف الناتج يُسمّى كما (قد يحتوي على أدلة): [getPathHeader()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getPathHeader--)+[getSheetPrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSheetPrefix--)+SheetIndex(أو SheetName)+[getSplitPartPrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSplitPartPrefix--)+SplitPartIndex+[getPathTail()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getPathTail--).
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [LowCodeSaveOptionsProviderOfAssembling()](#LowCodeSaveOptionsProviderOfAssembling--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finish(LowCodeSaveOptions part)](#finish-com.aspose.cells.LowCodeSaveOptions-) | يطلق الموارد بعد معالجة الجزء المقسم الحالي. |
| [getBuildPathWithSheetAlways()](#getBuildPathWithSheetAlways--) | ما إذا كان يتم دائمًا إضافة فهرس الورقة أو اسمها إلى مسار الملف. |
| [getBuildPathWithSplitPartAlways()](#getBuildPathWithSplitPartAlways--) | ما إذا كان يتم دائمًا إضافة فهرس الجزء المقسم إلى مسار الملف. |
| [getClass()](#getClass--) |  |
| [getPathHeader()](#getPathHeader--) | الجزء الرأس (قبل المحتوى المضاف للورقة والجزء المقسم) من مسار الملف. |
| [getPathTail()](#getPathTail--) | الجزء اللاحق (بعد أرقام التسلسل) من مسار الملف. |
| [getSaveOptions(SplitPartInfo part)](#getSaveOptions-com.aspose.cells.SplitPartInfo-) | يحصل على خيارات الحفظ التي تُستخرج منها إعدادات الإخراج للجزء المقسم الحالي. |
| [getSaveOptionsTemplate()](#getSaveOptionsTemplate--) | القالب لإنشاء نسخة من خيارات الحفظ في [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSaveOptions-SplitPartInfo-). |
| [getSheetIndexOffset()](#getSheetIndexOffset--) | الإزاحة في فهرس الورقة بين ما يُستخدم في مسار الملف والقيمة الفعلية له ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)). |
| [getSheetPrefix()](#getSheetPrefix--) | بادئة لفهرس ورقة العمل. |
| [getSplitPartIndexOffset()](#getSplitPartIndexOffset--) | الإزاحة لفهرس جزء الانقسام بين ما يُستخدم في مسار الملف والقيمة الفعلية له([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)). |
| [getSplitPartPrefix()](#getSplitPartPrefix--) | بادئة لفهرس جزء الانقسام. |
| [getUseSheetName()](#getUseSheetName--) | ما إذا كان يبني مسار الملف باستخدام اسم الورقة بدلاً من فهرس الورقة. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBuildPathWithSheetAlways(boolean value)](#setBuildPathWithSheetAlways-boolean-) | ما إذا كان يتم دائمًا إضافة فهرس الورقة أو اسمها إلى مسار الملف. |
| [setBuildPathWithSplitPartAlways(boolean value)](#setBuildPathWithSplitPartAlways-boolean-) | ما إذا كان يتم دائمًا إضافة فهرس الجزء المقسم إلى مسار الملف. |
| [setPathHeader(String value)](#setPathHeader-java.lang.String-) | الجزء الرأس (قبل المحتوى المضاف للورقة والجزء المقسم) من مسار الملف. |
| [setPathTail(String value)](#setPathTail-java.lang.String-) | الجزء اللاحق (بعد أرقام التسلسل) من مسار الملف. |
| [setSaveOptionsTemplate(LowCodeSaveOptions value)](#setSaveOptionsTemplate-com.aspose.cells.LowCodeSaveOptions-) | القالب لإنشاء نسخة من خيارات الحفظ في [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSaveOptions-SplitPartInfo-). |
| [setSheetIndexOffset(int value)](#setSheetIndexOffset-int-) | الإزاحة في فهرس الورقة بين ما يُستخدم في مسار الملف والقيمة الفعلية له ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)). |
| [setSheetPrefix(String value)](#setSheetPrefix-java.lang.String-) | بادئة لفهرس ورقة العمل. |
| [setSplitPartIndexOffset(int value)](#setSplitPartIndexOffset-int-) | الإزاحة لفهرس جزء الانقسام بين ما يُستخدم في مسار الملف والقيمة الفعلية له([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)). |
| [setSplitPartPrefix(String value)](#setSplitPartPrefix-java.lang.String-) | بادئة لفهرس جزء الانقسام. |
| [setUseSheetName(boolean value)](#setUseSheetName-boolean-) | ما إذا كان يبني مسار الملف باستخدام اسم الورقة بدلاً من فهرس الورقة. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeSaveOptionsProviderOfAssembling() {#LowCodeSaveOptionsProviderOfAssembling--}
```
public LowCodeSaveOptionsProviderOfAssembling()
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
### finish(LowCodeSaveOptions part) {#finish-com.aspose.cells.LowCodeSaveOptions-}
```
public void finish(LowCodeSaveOptions part)
```


يطلق الموارد بعد معالجة الجزء المقسم الحالي.

**Remarks**

بشكل افتراضي، تقوم هذه الطريقة فقط بإغلاق الدفق المحدد بواسطة [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--) مباشرةً (إذا كانت خيارات الحفظ قد حددت Stream كوجهة). يمكن للمستخدم استبدال هذه الطريقة للتحكم في كيفية تحرير الموارد وفقًا لمتطلباته وتنفيذ [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/abstractlowcodesaveoptionsprovider\#getSaveOptions-SplitPartInfo-).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| part | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | خيارات الحفظ المستخدمة للجزء المقسم الحالي. |

### getBuildPathWithSheetAlways() {#getBuildPathWithSheetAlways--}
```
public boolean getBuildPathWithSheetAlways()
```


ما إذا كان يضيف فهرس الورقة أو اسمها إلى مسار الملف دائمًا. القيمة الافتراضية هي false، أي عندما تكون هناك ورقة واحدة فقط، لن يتم إضافة فهرس الورقة (أو اسمها) والبادئة المقابلة إلى مسار الملف.

**Returns:**
boolean
### getBuildPathWithSplitPartAlways() {#getBuildPathWithSplitPartAlways--}
```
public boolean getBuildPathWithSplitPartAlways()
```


ما إذا كان يضيف فهرس جزء الانقسام إلى مسار الملف دائمًا. القيمة الافتراضية هي false، أي عندما يكون هناك جزء انقسام واحد فقط، لن يتم إضافة فهرس جزء الانقسام والبادئة المقابلة إلى مسار الملف.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getPathHeader() {#getPathHeader--}
```
public String getPathHeader()
```


الجزء الرأس (قبل المحتوى المضاف للورقة والجزء المقسم) من مسار الملف.

**Returns:**
java.lang.String
### getPathTail() {#getPathTail--}
```
public String getPathTail()
```


الجزء اللاحق (بعد أرقام التسلسل) من مسار الملف. يجب أن يتضمن امتداد اسم الملف.

**Returns:**
java.lang.String
### getSaveOptions(SplitPartInfo part) {#getSaveOptions-com.aspose.cells.SplitPartInfo-}
```
public LowCodeSaveOptions getSaveOptions(SplitPartInfo part)
```


يحصل على خيارات الحفظ التي تُستخرج منها إعدادات الإخراج للجزء المقسم الحالي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| part | [SplitPartInfo](../../com.aspose.cells/splitpartinfo) |  |

**Returns:**
[LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
### getSaveOptionsTemplate() {#getSaveOptionsTemplate--}
```
public LowCodeSaveOptions getSaveOptionsTemplate()
```


القالب لإنشاء نسخة من خيارات الحفظ في [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSaveOptions-SplitPartInfo-).

**Remarks**

إذا تم تحديد القالب، فستقوم النسخة المنشأة بنسخ جميع الإعدادات منه وتحديث ملف الإخراج وفقًا لذلك.

**Returns:**
[LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
### getSheetIndexOffset() {#getSheetIndexOffset--}
```
public int getSheetIndexOffset()
```


الإزاحة في فهرس الورقة بين ما يُستخدم في مسار الملف والقيمة الفعلية له ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)).

**Remarks**

يعمل فقط عندما يكون [getUseSheetName()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getUseSheetName--) false.

**Returns:**
int
### getSheetPrefix() {#getSheetPrefix--}
```
public String getSheetPrefix()
```


بادئة لفهرس ورقة العمل.

**Remarks**

إذا كانت هناك ورقة عمل واحدة فقط وكان [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSheetAlways--) false، فلن تتم إضافة هذه البادئة وفهرس الورقة (أو اسمها) إلى مسار الملف الناتج.

**Returns:**
java.lang.String
### getSplitPartIndexOffset() {#getSplitPartIndexOffset--}
```
public int getSplitPartIndexOffset()
```


الإزاحة لفهرس جزء الانقسام بين ما يُستخدم في مسار الملف والقيمة الفعلية له([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)).

**Returns:**
int
### getSplitPartPrefix() {#getSplitPartPrefix--}
```
public String getSplitPartPrefix()
```


بادئة لفهرس جزء الانقسام.

**Remarks**

إذا كان هناك جزء انقسام واحد فقط وكان [getBuildPathWithSplitPartAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSplitPartAlways--) false، فلن تتم إضافة هذه البادئة وفهرس جزء الانقسام (0) إلى مسار الملف الناتج.

**Returns:**
java.lang.String
### getUseSheetName() {#getUseSheetName--}
```
public boolean getUseSheetName()
```


ما إذا كان يبني مسار الملف باستخدام اسم الورقة بدلاً من فهرس الورقة. القيمة الافتراضية هي false.

**Remarks**

لن يتم إعادة بناء اسم الورقة تلقائيًا أبدًا. لذا عند ضبطه على true، يرجى التأكد من عدم وجود اسم ورقة خاص قد يسبب مسار ملف أو اسم غير صالح.

**Returns:**
boolean
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




### setBuildPathWithSheetAlways(boolean value) {#setBuildPathWithSheetAlways-boolean-}
```
public void setBuildPathWithSheetAlways(boolean value)
```


ما إذا كان يضيف فهرس الورقة أو اسمها إلى مسار الملف دائمًا. القيمة الافتراضية هي false، أي عندما تكون هناك ورقة واحدة فقط، لن يتم إضافة فهرس الورقة (أو اسمها) والبادئة المقابلة إلى مسار الملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setBuildPathWithSplitPartAlways(boolean value) {#setBuildPathWithSplitPartAlways-boolean-}
```
public void setBuildPathWithSplitPartAlways(boolean value)
```


ما إذا كان يضيف فهرس جزء الانقسام إلى مسار الملف دائمًا. القيمة الافتراضية هي false، أي عندما يكون هناك جزء انقسام واحد فقط، لن يتم إضافة فهرس جزء الانقسام والبادئة المقابلة إلى مسار الملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setPathHeader(String value) {#setPathHeader-java.lang.String-}
```
public void setPathHeader(String value)
```


الجزء الرأس (قبل المحتوى المضاف للورقة والجزء المقسم) من مسار الملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setPathTail(String value) {#setPathTail-java.lang.String-}
```
public void setPathTail(String value)
```


الجزء اللاحق (بعد أرقام التسلسل) من مسار الملف. يجب أن يتضمن امتداد اسم الملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setSaveOptionsTemplate(LowCodeSaveOptions value) {#setSaveOptionsTemplate-com.aspose.cells.LowCodeSaveOptions-}
```
public void setSaveOptionsTemplate(LowCodeSaveOptions value)
```


القالب لإنشاء نسخة من خيارات الحفظ في [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSaveOptions-SplitPartInfo-).

**Remarks**

إذا تم تحديد القالب، فستقوم النسخة المنشأة بنسخ جميع الإعدادات منه وتحديث ملف الإخراج وفقًا لذلك.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) |  |

### setSheetIndexOffset(int value) {#setSheetIndexOffset-int-}
```
public void setSheetIndexOffset(int value)
```


الإزاحة في فهرس الورقة بين ما يُستخدم في مسار الملف والقيمة الفعلية له ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)).

**Remarks**

يعمل فقط عندما يكون [getUseSheetName()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getUseSheetName--) false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setSheetPrefix(String value) {#setSheetPrefix-java.lang.String-}
```
public void setSheetPrefix(String value)
```


بادئة لفهرس ورقة العمل.

**Remarks**

إذا كانت هناك ورقة عمل واحدة فقط وكان [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSheetAlways--) false، فلن تتم إضافة هذه البادئة وفهرس الورقة (أو اسمها) إلى مسار الملف الناتج.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setSplitPartIndexOffset(int value) {#setSplitPartIndexOffset-int-}
```
public void setSplitPartIndexOffset(int value)
```


الإزاحة لفهرس جزء الانقسام بين ما يُستخدم في مسار الملف والقيمة الفعلية له([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setSplitPartPrefix(String value) {#setSplitPartPrefix-java.lang.String-}
```
public void setSplitPartPrefix(String value)
```


بادئة لفهرس جزء الانقسام.

**Remarks**

إذا كان هناك جزء انقسام واحد فقط وكان [getBuildPathWithSplitPartAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSplitPartAlways--) false، فلن تتم إضافة هذه البادئة وفهرس جزء الانقسام (0) إلى مسار الملف الناتج.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setUseSheetName(boolean value) {#setUseSheetName-boolean-}
```
public void setUseSheetName(boolean value)
```


ما إذا كان يبني مسار الملف باستخدام اسم الورقة بدلاً من فهرس الورقة. القيمة الافتراضية هي false.

**Remarks**

لن يتم إعادة بناء اسم الورقة تلقائيًا أبدًا. لذا عند ضبطه على true، يرجى التأكد من عدم وجود اسم ورقة خاص قد يسبب مسار ملف أو اسم غير صالح.

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

