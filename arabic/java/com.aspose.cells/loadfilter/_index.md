---
title: "LoadFilter"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل الفلتر الذي يوفر خيارات لتحميل البيانات عند تحميل المصنف من القالب."
type: docs
url: /ar/java/com.aspose.cells/loadfilter/
---

**Inheritance:**
java.lang.Object
```
public class LoadFilter
```

يمثل الفلتر الذي يوفر خيارات لتحميل البيانات عند تحميل المصنف من القالب.

**Remarks**

يمكن للمستخدم تحديد خيارات الفلتر أو تنفيذ LoadFilter الخاص به لتحديد كيفية تحميل البيانات.

**Example**

المثال التالي يوضح كيفية تحديد خيارات الفلتر وفقًا لخصائص ورقة العمل.

```
         class LoadFilterSheet extends LoadFilter
         {
             public /*override*/ void startSheet(Worksheet sheet) 
             {
                 if ("Sheet1".equals(sheet.getName()))
                 {
                     setLoadDataFilterOptions(LoadDataFilterOptions.ALL);
                 }
                 else
                 {
                     setLoadDataFilterOptions(LoadDataFilterOptions.STRUCTURE);
                 }
             }
         }
         LoadOptions opts = new LoadOptions();
         opts.setLoadFilter(new LoadFilterSheet());
         Workbook wb = new Workbook("template.xlsx", opts);
         //Custom LoadFilter implementation
```
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [LoadFilter()](#LoadFilter--) | ينشئ LoadFilter واحد مع خيارات الفلتر الافتراضية LoadDataFilterOptions.All. |
| [LoadFilter(int opts)](#LoadFilter-int-) | ينشئ LoadFilter واحد مع خيارات الفلتر المعطاة. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getLoadDataFilterOptions()](#getLoadDataFilterOptions--) | خيارات الفلتر لتحديد البيانات التي يجب تحميلها. |
| [getSheetsInLoadingOrder()](#getSheetsInLoadingOrder--) | يحدد الأوراق (المؤشرات) والترتيب الذي سيتم تحميله. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setLoadDataFilterOptions(int value)](#setLoadDataFilterOptions-int-) | خيارات الفلتر لتحديد البيانات التي يجب تحميلها. |
| [startSheet(Worksheet sheet)](#startSheet-com.aspose.cells.Worksheet-) | يجهز خيارات الفلتر قبل تحميل ورقة العمل المحددة. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LoadFilter() {#LoadFilter--}
```
public LoadFilter()
```


ينشئ LoadFilter واحد مع خيارات الفلتر الافتراضية LoadDataFilterOptions.All.

### LoadFilter(int opts) {#LoadFilter-int-}
```
public LoadFilter(int opts)
```


ينشئ LoadFilter واحد مع خيارات الفلتر المعطاة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| opts | int | [LoadDataFilterOptions](../../com.aspose.cells/loaddatafilteroptions). خيارات الفلتر الافتراضية |

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
### getLoadDataFilterOptions() {#getLoadDataFilterOptions--}
```
public int getLoadDataFilterOptions()
```


خيارات الفلتر لتحديد البيانات التي يجب تحميلها.

انظر [LoadDataFilterOptions](../../com.aspose.cells/loaddatafilteroptions).

**Returns:**
int
### getSheetsInLoadingOrder() {#getSheetsInLoadingOrder--}
```
public int[] getSheetsInLoadingOrder()
```


يحدد الأوراق (المؤشرات) والترتيب الذي سيتم تحميله. القيمة الافتراضية هي null، مما يعني تحميل جميع الأوراق بالترتيب الافتراضي في ملف القالب. إذا لم تكن null وكان مؤشر بعض الورقة غير موجود في المصفوفة المرتجعة، فلن يتم تحميل تلك الورقة.

**Returns:**
int[]
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




### setLoadDataFilterOptions(int value) {#setLoadDataFilterOptions-int-}
```
public void setLoadDataFilterOptions(int value)
```


خيارات الفلتر لتحديد البيانات التي يجب تحميلها.

انظر [LoadDataFilterOptions](../../com.aspose.cells/loaddatafilteroptions).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### startSheet(Worksheet sheet) {#startSheet-com.aspose.cells.Worksheet-}
```
public void startSheet(Worksheet sheet)
```


يجهز خيارات الفلتر قبل تحميل ورقة العمل المحددة. يمكن لتطبيق المستخدم لـ LoadFilter تعديل LoadDataFilterOptions هنا لتحديد كيفية تحميل البيانات لهذه الورقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sheet | [Worksheet](../../com.aspose.cells/worksheet) | ورقة العمل التي سيتم تحميلها. هناك عدد قليل فقط من الخصائص التي يمكن استخدامها لكائن ورقة العمل المحددة هنا لأن معظم البيانات والخصائص لم يتم تحميلها. الخصائص المتاحة هي: Name, Index, VisibilityType |

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

