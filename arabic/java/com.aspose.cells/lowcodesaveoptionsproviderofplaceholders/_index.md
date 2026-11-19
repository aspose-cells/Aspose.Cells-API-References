---
title: "LowCodeSaveOptionsProviderOfPlaceHolders"
second_title: "Aspose.Cells for Java API Reference"
description: "تنفيذ لتوفير خيارات الحفظ التي تحفظ الأجزاء المقسمة إلى ملفات ويتم تعريف مسار الملف الناتج باستخدام العناصر النائبة."
type: docs
url: /ar/java/com.aspose.cells/lowcodesaveoptionsproviderofplaceholders/
---

**Inheritance:**
java.lang.Object، [com.aspose.cells.AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider)
```
public class LowCodeSaveOptionsProviderOfPlaceHolders extends AbstractLowCodeSaveOptionsProvider
```

تنفيذ لتوفير خيارات الحفظ التي تحفظ الأجزاء المقسمة إلى ملفات ويتم تعريف مسار الملف الناتج باستخدام العناصر النائبة.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [LowCodeSaveOptionsProviderOfPlaceHolders(String pathTemplate)](#LowCodeSaveOptionsProviderOfPlaceHolders-java.lang.String-) | ينشئ كائنًا لتوفير خيارات الحفظ وفقًا للقوالب المحددة. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finish(LowCodeSaveOptions part)](#finish-com.aspose.cells.LowCodeSaveOptions-) | يطلق الموارد بعد معالجة الجزء المقسم الحالي. |
| [getBuildPathWithSheetAlways()](#getBuildPathWithSheetAlways--) | ما إذا كان يتم دائمًا إضافة فهرس الورقة أو اسمها إلى مسار الملف. |
| [getBuildPathWithSplitPartAlways()](#getBuildPathWithSplitPartAlways--) | ما إذا كان يتم دائمًا إضافة فهرس الجزء المقسم إلى مسار الملف. |
| [getClass()](#getClass--) |  |
| [getSaveOptions(SplitPartInfo part)](#getSaveOptions-com.aspose.cells.SplitPartInfo-) | يحصل على خيارات الحفظ التي تُستخرج منها إعدادات الإخراج للجزء المقسم الحالي. |
| [getSaveOptionsTemplate()](#getSaveOptionsTemplate--) | القالب لإنشاء كائن خيارات الحفظ في [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSaveOptions-SplitPartInfo-). |
| [getSheetIndexOffset()](#getSheetIndexOffset--) | الإزاحة في فهرس الورقة بين ما يُستخدم في مسار الملف والقيمة الفعلية له ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)). |
| [getSheetIndexPrefix()](#getSheetIndexPrefix--) | بادئة لفهرس ورقة العمل. |
| [getSheetNamePrefix()](#getSheetNamePrefix--) | بادئة لفهرس ورقة العمل. |
| [getSplitPartIndexOffset()](#getSplitPartIndexOffset--) | الإزاحة لفهرس جزء الانقسام بين ما يُستخدم في مسار الملف والقيمة الفعلية له([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)). |
| [getSplitPartPrefix()](#getSplitPartPrefix--) | بادئة لفهرس جزء الانقسام. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBuildPathWithSheetAlways(boolean value)](#setBuildPathWithSheetAlways-boolean-) | ما إذا كان يتم دائمًا إضافة فهرس الورقة أو اسمها إلى مسار الملف. |
| [setBuildPathWithSplitPartAlways(boolean value)](#setBuildPathWithSplitPartAlways-boolean-) | ما إذا كان يتم دائمًا إضافة فهرس الجزء المقسم إلى مسار الملف. |
| [setSaveOptionsTemplate(LowCodeSaveOptions value)](#setSaveOptionsTemplate-com.aspose.cells.LowCodeSaveOptions-) | القالب لإنشاء كائن خيارات الحفظ في [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSaveOptions-SplitPartInfo-). |
| [setSheetIndexOffset(int value)](#setSheetIndexOffset-int-) | الإزاحة في فهرس الورقة بين ما يُستخدم في مسار الملف والقيمة الفعلية له ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)). |
| [setSheetIndexPrefix(String value)](#setSheetIndexPrefix-java.lang.String-) | بادئة لفهرس ورقة العمل. |
| [setSheetNamePrefix(String value)](#setSheetNamePrefix-java.lang.String-) | بادئة لفهرس ورقة العمل. |
| [setSplitPartIndexOffset(int value)](#setSplitPartIndexOffset-int-) | الإزاحة لفهرس جزء الانقسام بين ما يُستخدم في مسار الملف والقيمة الفعلية له([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)). |
| [setSplitPartPrefix(String value)](#setSplitPartPrefix-java.lang.String-) | بادئة لفهرس جزء الانقسام. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeSaveOptionsProviderOfPlaceHolders(String pathTemplate) {#LowCodeSaveOptionsProviderOfPlaceHolders-java.lang.String-}
```
public LowCodeSaveOptionsProviderOfPlaceHolders(String pathTemplate)
```


ينشئ كائنًا لتوفير خيارات الحفظ وفقًا للقوالب المحددة.

**Remarks**

العناصر النائبة المدعومة في قالب مسار الملف:

 *  $\{SheetIndex\}: will be replaced by the sheet index of the split part
 *  $\{SheetName\}: will be replaced by the sheet name of the split part
 *  $\{SplitPartIndex\}: will be replaced by the index of the split part
 *  $\{SheetIndexPrefix\}: will be replaced by
 *  $\{SheetNamePrefix\}: will be replaced by
 *  $\{SplitPartPrefix\}: will be replaced by

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| pathTemplate | java.lang.String | قالب مسار الملف الناتج. |

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


ما إذا كان يجب إضافة فهرس الورقة أو اسمها إلى مسار الملف دائمًا. القيمة الافتراضية هي false، أي عندما تكون هناك ورقة واحدة فقط، لن يتم إضافة فهرس الورقة والاسم والبادئة المقابلة ([getSheetNamePrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSheetNamePrefix--)) إلى مسار الملف.

**Returns:**
boolean
### getBuildPathWithSplitPartAlways() {#getBuildPathWithSplitPartAlways--}
```
public boolean getBuildPathWithSplitPartAlways()
```


ما إذا كان يجب إضافة فهرس الجزء المقسّم إلى مسار الملف دائمًا. القيمة الافتراضية هي false، أي عندما يكون هناك جزء مقسّم واحد فقط، لن يتم إضافة فهرس الجزء المقسّم والبادئة المقابلة ([getSplitPartPrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSplitPartPrefix--)) إلى مسار الملف.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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


القالب لإنشاء كائن خيارات الحفظ في [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSaveOptions-SplitPartInfo-).

**Remarks**

إذا تم تحديد القالب، فستقوم النسخة المنشأة بنسخ جميع الإعدادات منه وتحديث ملف الإخراج وفقًا لذلك.

**Returns:**
[LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
### getSheetIndexOffset() {#getSheetIndexOffset--}
```
public int getSheetIndexOffset()
```


الإزاحة في فهرس الورقة بين ما يُستخدم في مسار الملف والقيمة الفعلية له ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)).

**Returns:**
int
### getSheetIndexPrefix() {#getSheetIndexPrefix--}
```
public String getSheetIndexPrefix()
```


بادئة لفهرس ورقة العمل.

**Remarks**

إذا كان هناك ورقة عمل واحدة فقط وكان [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSheetAlways--) غير مفعّل (false)، فلن تتم إضافة هذه البادئة وفهرس الورقة (أو اسمها) إلى مسار الملف الناتج.

**Returns:**
java.lang.String
### getSheetNamePrefix() {#getSheetNamePrefix--}
```
public String getSheetNamePrefix()
```


بادئة لفهرس ورقة العمل.

**Remarks**

إذا كان هناك ورقة عمل واحدة فقط وكان [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSheetAlways--) غير مفعّل (false)، فلن تتم إضافة هذه البادئة وفهرس الورقة (أو اسمها) إلى مسار الملف الناتج.

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

إذا كان هناك جزء مقسّم واحد فقط وكان [getBuildPathWithSplitPartAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSplitPartAlways--) غير مفعّل (false)، فلن تتم إضافة هذه البادئة وفهرس الجزء المقسّم (0) إلى مسار الملف الناتج.

**Returns:**
java.lang.String
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


ما إذا كان يجب إضافة فهرس الورقة أو اسمها إلى مسار الملف دائمًا. القيمة الافتراضية هي false، أي عندما تكون هناك ورقة واحدة فقط، لن يتم إضافة فهرس الورقة والاسم والبادئة المقابلة ([getSheetNamePrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSheetNamePrefix--)) إلى مسار الملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setBuildPathWithSplitPartAlways(boolean value) {#setBuildPathWithSplitPartAlways-boolean-}
```
public void setBuildPathWithSplitPartAlways(boolean value)
```


ما إذا كان يجب إضافة فهرس الجزء المقسّم إلى مسار الملف دائمًا. القيمة الافتراضية هي false، أي عندما يكون هناك جزء مقسّم واحد فقط، لن يتم إضافة فهرس الجزء المقسّم والبادئة المقابلة ([getSplitPartPrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSplitPartPrefix--)) إلى مسار الملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSaveOptionsTemplate(LowCodeSaveOptions value) {#setSaveOptionsTemplate-com.aspose.cells.LowCodeSaveOptions-}
```
public void setSaveOptionsTemplate(LowCodeSaveOptions value)
```


القالب لإنشاء كائن خيارات الحفظ في [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSaveOptions-SplitPartInfo-).

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

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setSheetIndexPrefix(String value) {#setSheetIndexPrefix-java.lang.String-}
```
public void setSheetIndexPrefix(String value)
```


بادئة لفهرس ورقة العمل.

**Remarks**

إذا كان هناك ورقة عمل واحدة فقط وكان [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSheetAlways--) غير مفعّل (false)، فلن تتم إضافة هذه البادئة وفهرس الورقة (أو اسمها) إلى مسار الملف الناتج.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setSheetNamePrefix(String value) {#setSheetNamePrefix-java.lang.String-}
```
public void setSheetNamePrefix(String value)
```


بادئة لفهرس ورقة العمل.

**Remarks**

إذا كان هناك ورقة عمل واحدة فقط وكان [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSheetAlways--) غير مفعّل (false)، فلن تتم إضافة هذه البادئة وفهرس الورقة (أو اسمها) إلى مسار الملف الناتج.

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

إذا كان هناك جزء مقسّم واحد فقط وكان [getBuildPathWithSplitPartAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSplitPartAlways--) غير مفعّل (false)، فلن تتم إضافة هذه البادئة وفهرس الجزء المقسّم (0) إلى مسار الملف الناتج.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

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

