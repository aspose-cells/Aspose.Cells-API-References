---
title: "GridJsOptions"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل جميع خيارات التحميل لـ GridJs"
type: docs
url: /ar/java/com.aspose.gridjs/gridjsoptions/
---

**Inheritance:**
java.lang.Object
```
public class GridJsOptions
```

يمثل جميع خيارات التحميل لـ GridJs
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [GridJsOptions()](#GridJsOptions--) |  |
## حقول

| حقل | الوصف |
| --- | --- |
| [CacheImp](#CacheImp) | تنفيذ مخصص لتخزين الذاكرة المؤقتة، إذا كنت تريد تخزين الذاكرة المؤقتة بطريقة تدفق، تحتاج إلى ضبطها وتنفيذها. |
| [RedactionUseClientGenerateId](#RedactionUseClientGenerateId) | يشير إلى ما إذا كان يتم استخدام معرف مولد من العميل بدلاً من معرف الشكل الفعلي في عمليات التعديل المتعلقة. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFitColumnsOnLoad()](#getAutoFitColumnsOnLoad--) | يشير إلى ما إذا كان سيتم ضبط عرض الأعمدة تلقائيًا عند تحميل الملف، القيمة الافتراضية هي false. |
| [getAutoFitRowsHeightOnLoad()](#getAutoFitRowsHeightOnLoad--) | يشير إلى ما إذا كان سيتم ضبط ارتفاع الصفوف تلقائيًا عند تحميل الملف، القيمة الافتراضية هي false. |
| [getAutoOptimizeForLargeCells()](#getAutoOptimizeForLargeCells--) | يحدد ما إذا كان سيتم تحسين أداء التحميل تلقائيًا لورقة العمل التي تحتوي على خلايا كبيرة. |
| [getBaseRouteName()](#getBaseRouteName--) | يحصل على اسم قاعدة مسار URL لمتحكم GridJs. القيمة الافتراضية هي GridJs2. |
| [getClass()](#getClass--) |  |
| [getEmptySheetMaxCol()](#getEmptySheetMaxCol--) | يحصل على الحد الأقصى الافتراضي للأعمدة لورقة عمل فارغة. |
| [getEmptySheetMaxRow()](#getEmptySheetMaxRow--) | يحصل على الحد الأقصى الافتراضي للصفوف لورقة عمل فارغة. |
| [getEnableChartClientRendering()](#getEnableChartClientRendering--) | يحدد ما إذا كان سيتم تمكين عرض المخططات من جانب العميل. |
| [getFileCacheDirectory()](#getFileCacheDirectory--) | يحصل على دليل الذاكرة المؤقتة لتخزين ملف جدول البيانات. |
| [getFontFolders()](#getFontFolders--) | يحصل على مجلدات الخطوط للخطوط في الصور/الأشكال المرسومة. |
| [getIgnoreEmptyContent()](#getIgnoreEmptyContent--) | يحدد ما إذا كان سيتم إظهار النطاق الأقصى الذي يتضمن البيانات، الأنماط، الخلايا المدمجة والأشكال. |
| [getIslimitShapeOrImage()](#getIslimitShapeOrImage--) | يحدد ما إذا كان سيتم تقييد العدد الإجمالي للأشكال/الصور المعروضة في ورقة عمل واحدة، إذا تم ضبطه على true، سيقوم GridJs بتقييد العدد الإجمالي للأشكال أو الصور المعروضة في ورقة عمل واحدة إلى MaxShapeOrImageCount، القيمة الافتراضية هي true. |
| [getJsonCache()](#getJsonCache--) | يحصل على خيارات تكوين الذاكرة المؤقتة بصيغة JSON. |
| [getLazyLoading()](#getLazyLoading--) | يحدد ما إذا كان سيتم تحميل ورقة العمل النشطة فقط، القيمة الافتراضية هي false. |
| [getMaxPdfSaveSeconds()](#getMaxPdfSaveSeconds--) | يحصل على الحد الأقصى لثواني المهلة عند الحفظ إلى PDF. |
| [getMaxShapeOrImageCount()](#getMaxShapeOrImageCount--) | يحصل على العدد الإجمالي للأشكال أو الصور المعروضة في الورقة النشطة، يصبح ساريًا عندما يكون IslimitShapeOrImage=true. |
| [getMaxShapeOrImageWidthOrHeight()](#getMaxShapeOrImageWidthOrHeight--) | يحصل على الحد الأقصى للعرض أو الارتفاع لشكل أو صورة، سيتجاهل GridJs الشكل أو الصورة التي يكون عرضها أو ارتفاعها أكبر من ذلك، يصبح ساريًا عندما يكون IslimitShapeOrImage=true. |
| [getMaxTotalShapeOrImageCount()](#getMaxTotalShapeOrImageCount--) | يحصل على العدد الإجمالي للأشكال أو الصور المعروضة في دفتر العمل، يصبح ساريًا عندما يكون IslimitShapeOrImage=true. |
| [getMessageTopic()](#getMessageTopic--) | يحصل على وجهات الويب سوكت التي تبدأ بـ "/topic". القيمة الافتراضية هي "/topic/opr". تُستخدم في وضع التعاون فقط. |
| [getPictureCacheDirectory()](#getPictureCacheDirectory--) | يحصل على دليل الذاكرة المؤقتة للصور. |
| [getSameImageDetecting()](#getSameImageDetecting--) | يحدد ما إذا كان سيتم التحقق مما إذا كانت الصور لها نفس المصدر، القيمة الافتراضية هي true. |
| [getSaveHtmlAsZip()](#getSaveHtmlAsZip--) | يحدد ما إذا كان سيتم حفظ ملف HTML كأرشيف zip، القيمة الافتراضية هي false. |
| [getShowChartSheet()](#getShowChartSheet--) | يحدد ما إذا كان سيتم إظهار ورقة عمل المخطط. |
| [getSkipInvisibleShapes()](#getSkipInvisibleShapes--) | يحصل على ما إذا كان سيتم تخطي الأشكال غير المرئية لواجهة المستخدم، القيمة الافتراضية هي true. |
| [getUsePrintArea()](#getUsePrintArea--) | يحصل على ما إذا كان سيتم استخدام PageSetup.PrintArea لنطاق عرض واجهة المستخدم عندما تحتوي ورقة العمل على إعداد PageSetup لمنطقة الطباعة. |
| [hashCode()](#hashCode--) |  |
| [isCollaborative()](#isCollaborative--) | يحصل على ما إذا كان سيتم دعم التحرير التعاوني، القيمة الافتراضية هي false. |
| [isWasm()](#isWasm--) | يحصل على ما إذا كان GridJs يعمل داخل مضيف WebAssembly للمتصفح بدلاً من عملية الخادم. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFitColumnsOnLoad(boolean value)](#setAutoFitColumnsOnLoad-boolean-) | يشير إلى ما إذا كان سيتم ضبط عرض الأعمدة تلقائيًا عند تحميل الملف، القيمة الافتراضية هي false. |
| [setAutoFitRowsHeightOnLoad(boolean value)](#setAutoFitRowsHeightOnLoad-boolean-) | يشير إلى ما إذا كان سيتم ضبط ارتفاع الصفوف تلقائيًا عند تحميل الملف، القيمة الافتراضية هي false. |
| [setAutoOptimizeForLargeCells(boolean value)](#setAutoOptimizeForLargeCells-boolean-) | يضبط ما إذا كان سيتم تحسين أداء التحميل تلقائيًا لورقة العمل ذات الخلايا الكبيرة. |
| [setBaseRouteName(String value)](#setBaseRouteName-java.lang.String-) | يضبط الاسم الأساسي لمسار URL لواجهة تحكم GridJs. القيمة الافتراضية هي GridJs2 |
| [setCollaborative(boolean value)](#setCollaborative-boolean-) | يضبط ما إذا كان سيتم دعم التحرير التعاوني، القيمة الافتراضية هي false. |
| [setEmptySheetMaxCol(int value)](#setEmptySheetMaxCol-int-) | يضبط الحد الأقصى الافتراضي للأعمدة لورقة عمل فارغة. |
| [setEmptySheetMaxRow(int value)](#setEmptySheetMaxRow-int-) | يضبط الحد الأقصى الافتراضي للصفوف لورقة عمل فارغة. |
| [setEnableChartClientRendering(boolean value)](#setEnableChartClientRendering-boolean-) | يضبط ما إذا كان سيتم تمكين عرض المخططات من جانب العميل. |
| [setFileCacheDirectory(String value)](#setFileCacheDirectory-java.lang.String-) | يضبط دليل التخزين المؤقت لحفظ ملفات جداول البيانات. |
| [setFontFolders(String[] value)](#setFontFolders-java.lang.String---) | يضبط مجلدات الخطوط للخطوط في الصور/الأشكال المرسومة |
| [setIgnoreEmptyContent(boolean value)](#setIgnoreEmptyContent-boolean-) | يضبط ما إذا كان سيتم إظهار النطاق الأقصى الذي يشمل البيانات، الأنماط، الخلايا المدمجة والأشكال. |
| [setIslimitShapeOrImage(boolean value)](#setIslimitShapeOrImage-boolean-) | يضبط ما إذا كان سيتم تقييد العدد الإجمالي للأشكال/الصور المعروضة في ورقة عمل واحدة، إذا تم ضبطه على true، سيقوم GridJs بتقييد العدد الإجمالي للأشكال أو الصور المعروضة في ورقة عمل واحدة إلى MaxShapeOrImageCount. القيمة الافتراضية هي true. |
| [setJsonCache(JsonCacheOptions value)](#setJsonCache-com.aspose.gridjs.JsonCacheOptions-) | يضبط خيارات تكوين التخزين المؤقت لـ JSON. |
| [setLazyLoading(boolean value)](#setLazyLoading-boolean-) | يضبط ما إذا كان سيتم تحميل ورقة العمل النشطة فقط، القيمة الافتراضية هي false. |
| [setMaxPdfSaveSeconds(int value)](#setMaxPdfSaveSeconds-int-) | يضبط الحد الأقصى لثواني المهلة عند الحفظ إلى PDF. |
| [setMaxShapeOrImageCount(int value)](#setMaxShapeOrImageCount-int-) | يضبط العدد الإجمالي للأشكال أو الصور المعروضة في الورقة النشطة، ويصبح ساريًا عندما يكون IslimitShapeOrImage=true. |
| [setMaxShapeOrImageWidthOrHeight(int value)](#setMaxShapeOrImageWidthOrHeight-int-) | يضبط الحد الأقصى للعرض أو الارتفاع لشكل أو صورة، سيقوم GridJs بتجاهل الشكل أو الصورة التي يتجاوز عرضها أو ارتفاعها هذا الحد، ويصبح ساريًا عندما يكون IslimitShapeOrImage=true. |
| [setMaxTotalShapeOrImageCount(int value)](#setMaxTotalShapeOrImageCount-int-) | يضبط العدد الإجمالي للأشكال أو الصور المعروضة في دفتر العمل، ويصبح ساريًا عندما يكون IslimitShapeOrImage=true. |
| [setMessageTopic(String value)](#setMessageTopic-java.lang.String-) | يضبط وجهات WebSocket التي تبدأ بـ "/topic". القيمة الافتراضية هي "/topic/opr". تُستخدم في وضع التعاون فقط. |
| [setPictureCacheDirectory(String value)](#setPictureCacheDirectory-java.lang.String-) | يضبط دليل التخزين المؤقت للصور. |
| [setSameImageDetecting(boolean value)](#setSameImageDetecting-boolean-) | يضبط ما إذا كان سيتم التحقق مما إذا كانت الصور لها نفس المصدر، القيمة الافتراضية هي true. |
| [setSaveHtmlAsZip(boolean value)](#setSaveHtmlAsZip-boolean-) | يضبط ما إذا كان سيتم حفظ ملف HTML كأرشيف zip، القيمة الافتراضية هي false. |
| [setShowChartSheet(boolean value)](#setShowChartSheet-boolean-) | يضبط ما إذا كان سيتم إظهار ورقة عمل المخطط. |
| [setSkipInvisibleShapes(boolean value)](#setSkipInvisibleShapes-boolean-) | يضبط ما إذا كان سيتم تخطي الأشكال غير المرئية لواجهة المستخدم، القيمة الافتراضية هي true. |
| [setUsePrintArea(boolean value)](#setUsePrintArea-boolean-) | يضبط ما إذا كان سيتم استخدام PageSetup.PrintArea لنطاق عرض واجهة المستخدم عندما تحتوي ورقة العمل على إعداد PageSetup لـ PrintArea. |
| [setWasm(boolean value)](#setWasm-boolean-) | يضبط ما إذا كان GridJs يعمل داخل مضيف WebAssembly للمتصفح بدلاً من عملية خادم. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridJsOptions() {#GridJsOptions--}
```
public GridJsOptions()
```


### CacheImp {#CacheImp}
```
public GridCacheForStream CacheImp
```


تنفيذ مخصص لتخزين الذاكرة المؤقتة، إذا كنت تريد تخزين الذاكرة المؤقتة بطريقة تدفق، تحتاج إلى ضبطه وتنفيذه. يجب على مضيف WebAssembly (IsWasm = true) ضبطه، لأن لا يوجد قرص محلي لذاكرة التخزين المؤقت الافتراضية للملفات.

### RedactionUseClientGenerateId {#RedactionUseClientGenerateId}
```
public boolean RedactionUseClientGenerateId
```


يشير إلى ما إذا كان يتم استخدام معرف مولد من العميل بدلاً من معرف الشكل الفعلي في عمليات التعديل المتعلقة.

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
### getAutoFitColumnsOnLoad() {#getAutoFitColumnsOnLoad--}
```
public boolean getAutoFitColumnsOnLoad()
```


يشير إلى ما إذا كان سيتم ضبط عرض الأعمدة تلقائيًا عند تحميل الملف، القيمة الافتراضية هي false.

**Returns:**
boolean
### getAutoFitRowsHeightOnLoad() {#getAutoFitRowsHeightOnLoad--}
```
public boolean getAutoFitRowsHeightOnLoad()
```


يشير إلى ما إذا كان سيتم ضبط ارتفاع الصفوف تلقائيًا عند تحميل الملف، القيمة الافتراضية هي false.

**Returns:**
boolean
### getAutoOptimizeForLargeCells() {#getAutoOptimizeForLargeCells--}
```
public boolean getAutoOptimizeForLargeCells()
```


يحصل على ما إذا كان سيتم تحسين أداء التحميل تلقائيًا لورقة العمل ذات الخلايا الكبيرة. سيتجاهل بعض الأنماط / الحدود لتقليل وقت التحميل. القيمة الافتراضية هي true.

**Returns:**
boolean
### getBaseRouteName() {#getBaseRouteName--}
```
public String getBaseRouteName()
```


يحصل على اسم قاعدة مسار URL لمتحكم GridJs. القيمة الافتراضية هي GridJs2.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEmptySheetMaxCol() {#getEmptySheetMaxCol--}
```
public int getEmptySheetMaxCol()
```


يحصل على الحد الأقصى الافتراضي للأعمدة لورقة عمل فارغة. القيمة الافتراضية هي 15.

**Returns:**
int
### getEmptySheetMaxRow() {#getEmptySheetMaxRow--}
```
public int getEmptySheetMaxRow()
```


يحصل على الحد الأقصى الافتراضي للصفوف لورقة عمل فارغة. القيمة الافتراضية هي 12.

**Returns:**
int
### getEnableChartClientRendering() {#getEnableChartClientRendering--}
```
public boolean getEnableChartClientRendering()
```


يحصل على ما إذا كان سيتم تمكين رسم المخططات من جانب العميل. إذا تم ضبطه على false، سيصدر GridJs صور/أشكال المخططات فقط ولن يتطلب رسم المخططات من جانب العميل. القيمة الافتراضية هي true.

**Returns:**
boolean
### getFileCacheDirectory() {#getFileCacheDirectory--}
```
public String getFileCacheDirectory()
```


يحصل على دليل الذاكرة المؤقتة لتخزين ملف جدول البيانات. نحتاج إلى ضبطه على مسار محدد قبل استخدام GridJs.

**Returns:**
java.lang.String
### getFontFolders() {#getFontFolders--}
```
public String[] getFontFolders()
```


يحصل على مجلدات الخطوط للخطوط في الصور/الأشكال المرسومة.

**Returns:**
java.lang.String[]
### getIgnoreEmptyContent() {#getIgnoreEmptyContent--}
```
public boolean getIgnoreEmptyContent()
```


يحصل على ما إذا كان سيتم إظهار النطاق الأقصى الذي يشمل البيانات، الأنماط، الخلايا المدمجة والأشكال. إذا كان الصف أو العمود الأخير يحتوي على خلايا بدون قيمة أو صيغة ولكن لها نمط مخصص، فلن نعرض هذا الصف/العمود عندما تكون هذه القيمة true\\u9286?\* القيمة الافتراضية هي true.

**Returns:**
boolean
### getIslimitShapeOrImage() {#getIslimitShapeOrImage--}
```
public boolean getIslimitShapeOrImage()
```


يحدد ما إذا كان سيتم تقييد العدد الإجمالي للأشكال/الصور المعروضة في ورقة عمل واحدة، إذا تم ضبطه على true، سيقوم GridJs بتقييد العدد الإجمالي للأشكال أو الصور المعروضة في ورقة عمل واحدة إلى MaxShapeOrImageCount، القيمة الافتراضية هي true.

**Returns:**
boolean
### getJsonCache() {#getJsonCache--}
```
public JsonCacheOptions getJsonCache()
```


يحصل على خيارات تكوين ذاكرة التخزين المؤقت JSON. يتحكم في سلوك الذاكرة (L1) والقرص (L2) للذاكرة المؤقتة لملف JSON الخاص بكتاب العمل المُنشأ.

**Returns:**
[JsonCacheOptions](../../com.aspose.gridjs/jsoncacheoptions)
### getLazyLoading() {#getLazyLoading--}
```
public boolean getLazyLoading()
```


يحدد ما إذا كان سيتم تحميل ورقة العمل النشطة فقط، القيمة الافتراضية هي false.

**Returns:**
boolean
### getMaxPdfSaveSeconds() {#getMaxPdfSaveSeconds--}
```
public int getMaxPdfSaveSeconds()
```


يحصل على الحد الأقصى للثواني عند انتهاء المهلة عند الحفظ إلى PDF. القيمة الافتراضية هي 10.

**Returns:**
int
### getMaxShapeOrImageCount() {#getMaxShapeOrImageCount--}
```
public int getMaxShapeOrImageCount()
```


يحصل على العدد الإجمالي للأشكال أو الصور المعروضة في الورقة النشطة، يُطبق عندما يكون IslimitShapeOrImage=true. القيمة الافتراضية هي 100.

**Returns:**
int
### getMaxShapeOrImageWidthOrHeight() {#getMaxShapeOrImageWidthOrHeight--}
```
public int getMaxShapeOrImageWidthOrHeight()
```


يحصل على الحد الأقصى للعرض أو الارتفاع لشكل أو صورة، سيتجاهل GridJs الشكل أو الصورة إذا كان العرض أو الارتفاع أكبر من ذلك، يُطبق عندما يكون IslimitShapeOrImage=true. القيمة الافتراضية هي 10000.

**Returns:**
int
### getMaxTotalShapeOrImageCount() {#getMaxTotalShapeOrImageCount--}
```
public int getMaxTotalShapeOrImageCount()
```


يحصل على العدد الإجمالي للأشكال أو الصور المعروضة في كتاب العمل، يُطبق عندما يكون IslimitShapeOrImage=true. القيمة الافتراضية هي 300.

**Returns:**
int
### getMessageTopic() {#getMessageTopic--}
```
public String getMessageTopic()
```


يحصل على وجهات الويب سوكت التي تبدأ بـ "/topic". القيمة الافتراضية هي "/topic/opr". تُستخدم في وضع التعاون فقط.

**Returns:**
java.lang.String
### getPictureCacheDirectory() {#getPictureCacheDirectory--}
```
public String getPictureCacheDirectory()
```


يحصل على دليل الذاكرة المؤقتة للصور. (يُطبق عندما يكون GridJsWorkbook.CacheImp فارغًا) سيكون المسار الافتراضي "\_piccache" داخل FileCacheDirectory.

**Returns:**
java.lang.String
### getSameImageDetecting() {#getSameImageDetecting--}
```
public boolean getSameImageDetecting()
```


يحدد ما إذا كان سيتم التحقق مما إذا كانت الصور لها نفس المصدر، القيمة الافتراضية هي true.

**Returns:**
boolean
### getSaveHtmlAsZip() {#getSaveHtmlAsZip--}
```
public boolean getSaveHtmlAsZip()
```


يحدد ما إذا كان سيتم حفظ ملف HTML كأرشيف zip، القيمة الافتراضية هي false.

**Returns:**
boolean
### getShowChartSheet() {#getShowChartSheet--}
```
public boolean getShowChartSheet()
```


يحصل على ما إذا كان سيتم إظهار ورقة عمل المخطط. القيمة الافتراضية هي false.

**Returns:**
boolean
### getSkipInvisibleShapes() {#getSkipInvisibleShapes--}
```
public boolean getSkipInvisibleShapes()
```


يحصل على ما إذا كان سيتم تخطي الأشكال غير المرئية لواجهة المستخدم، القيمة الافتراضية هي true.

**Returns:**
boolean
### getUsePrintArea() {#getUsePrintArea--}
```
public boolean getUsePrintArea()
```


يحصل على ما إذا كان سيتم استخدام PageSetup.PrintArea لنطاق عرض واجهة المستخدم عندما تحتوي ورقة العمل على إعداد PageSetup لـ PrintArea. القيمة الافتراضية هي false.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCollaborative() {#isCollaborative--}
```
public boolean isCollaborative()
```


يحصل على ما إذا كان سيتم دعم التحرير التعاوني، القيمة الافتراضية هي false.

**Returns:**
boolean
### isWasm() {#isWasm--}
```
public boolean isWasm()
```


يحصل على ما إذا كان GridJs يعمل داخل مضيف WebAssembly للمتصفح بدلاً من عملية خادم. عندما يكون true، لا يتم استخدام FileCacheDirectory / القرص / مسار مقاطعة الخيط، ويجب أن تأتي الذاكرة المؤقتة للملف من CacheImp، لأن مضيف المتصفح لا يملك قرصًا محليًا. يختار مسارات الشيفرة في وقت التشغيل، لذا فإن Aspose.Cells.GridJs.dll واحد يخدم كلا المضيفين. القيمة الافتراضية هي false.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAutoFitColumnsOnLoad(boolean value) {#setAutoFitColumnsOnLoad-boolean-}
```
public void setAutoFitColumnsOnLoad(boolean value)
```


يشير إلى ما إذا كان سيتم ضبط عرض الأعمدة تلقائيًا عند تحميل الملف، القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAutoFitRowsHeightOnLoad(boolean value) {#setAutoFitRowsHeightOnLoad-boolean-}
```
public void setAutoFitRowsHeightOnLoad(boolean value)
```


يشير إلى ما إذا كان سيتم ضبط ارتفاع الصفوف تلقائيًا عند تحميل الملف، القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAutoOptimizeForLargeCells(boolean value) {#setAutoOptimizeForLargeCells-boolean-}
```
public void setAutoOptimizeForLargeCells(boolean value)
```


يضبط ما إذا كان سيتم تحسين أداء التحميل تلقائيًا لورقة العمل ذات الخلايا الكبيرة. سيتجاهل بعض الأنماط / الحدود لتقليل وقت التحميل. القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setBaseRouteName(String value) {#setBaseRouteName-java.lang.String-}
```
public void setBaseRouteName(String value)
```


يضبط الاسم الأساسي لمسار URL لواجهة تحكم GridJs. القيمة الافتراضية هي GridJs2

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setCollaborative(boolean value) {#setCollaborative-boolean-}
```
public void setCollaborative(boolean value)
```


يضبط ما إذا كان سيتم دعم التحرير التعاوني، القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEmptySheetMaxCol(int value) {#setEmptySheetMaxCol-int-}
```
public void setEmptySheetMaxCol(int value)
```


يضبط الحد الأقصى الافتراضي للأعمدة لورقة عمل فارغة. القيمة الافتراضية هي 15.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setEmptySheetMaxRow(int value) {#setEmptySheetMaxRow-int-}
```
public void setEmptySheetMaxRow(int value)
```


يضبط الحد الأقصى الافتراضي للصفوف لورقة عمل فارغة. القيمة الافتراضية هي 12.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setEnableChartClientRendering(boolean value) {#setEnableChartClientRendering-boolean-}
```
public void setEnableChartClientRendering(boolean value)
```


يضبط ما إذا كان سيتم تمكين رسم المخططات من جانب العميل. إذا تم ضبطه على false، سيصدر GridJs صور/أشكال المخططات فقط ولن يتطلب رسم المخططات من جانب العميل. القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setFileCacheDirectory(String value) {#setFileCacheDirectory-java.lang.String-}
```
public void setFileCacheDirectory(String value)
```


يضبط دليل الذاكرة المؤقتة لتخزين ملف جدول البيانات. نحتاج إلى ضبطه على مسار محدد قبل استخدام GridJs.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setFontFolders(String[] value) {#setFontFolders-java.lang.String---}
```
public void setFontFolders(String[] value)
```


يضبط مجلدات الخطوط للخطوط في الصور/الأشكال المرسومة

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String[] |  |

### setIgnoreEmptyContent(boolean value) {#setIgnoreEmptyContent-boolean-}
```
public void setIgnoreEmptyContent(boolean value)
```


يضبط ما إذا كان سيتم إظهار النطاق الأقصى الذي يشمل البيانات، الأنماط، الخلايا المدمجة والأشكال. إذا كان الصف أو العمود الأخير يحتوي على خلايا بدون قيمة أو صيغة ولكن لها نمط مخصص، فلن نعرض هذا الصف/العمود عندما تكون هذه القيمة true\\u9286?\* القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setIslimitShapeOrImage(boolean value) {#setIslimitShapeOrImage-boolean-}
```
public void setIslimitShapeOrImage(boolean value)
```


يضبط ما إذا كان سيتم تقييد العدد الإجمالي للأشكال/الصور المعروضة في ورقة عمل واحدة، إذا تم ضبطه على true، سيقوم GridJs بتقييد العدد الإجمالي للأشكال أو الصور المعروضة في ورقة عمل واحدة إلى MaxShapeOrImageCount. القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setJsonCache(JsonCacheOptions value) {#setJsonCache-com.aspose.gridjs.JsonCacheOptions-}
```
public void setJsonCache(JsonCacheOptions value)
```


يضبط خيارات تكوين ذاكرة التخزين المؤقت JSON. يتحكم في سلوك ذاكرة التخزين المؤقت للذاكرة (L1) والقرص (L2) للـ JSON الخاص بكتاب العمل المُولد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [JsonCacheOptions](../../com.aspose.gridjs/jsoncacheoptions) |  |

### setLazyLoading(boolean value) {#setLazyLoading-boolean-}
```
public void setLazyLoading(boolean value)
```


يضبط ما إذا كان سيتم تحميل ورقة العمل النشطة فقط، القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setMaxPdfSaveSeconds(int value) {#setMaxPdfSaveSeconds-int-}
```
public void setMaxPdfSaveSeconds(int value)
```


يضبط الحد الأقصى لثواني المهلة عند الحفظ إلى PDF. القيمة الافتراضية هي 10.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setMaxShapeOrImageCount(int value) {#setMaxShapeOrImageCount-int-}
```
public void setMaxShapeOrImageCount(int value)
```


يضبط العدد الإجمالي للأشكال أو الصور المعروضة في الورقة النشطة، ويصبح ساريًا عندما يكون IslimitShapeOrImage=true. القيمة الافتراضية هي 100.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setMaxShapeOrImageWidthOrHeight(int value) {#setMaxShapeOrImageWidthOrHeight-int-}
```
public void setMaxShapeOrImageWidthOrHeight(int value)
```


يضبط الحد الأقصى للعرض أو الارتفاع لشكل أو صورة، سيتجاهل GridJs الشكل أو الصورة التي يكون عرضها أو ارتفاعها أكبر من ذلك، ويصبح ساريًا عندما يكون IslimitShapeOrImage=true. القيمة الافتراضية هي 10000.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setMaxTotalShapeOrImageCount(int value) {#setMaxTotalShapeOrImageCount-int-}
```
public void setMaxTotalShapeOrImageCount(int value)
```


يضبط العدد الإجمالي للأشكال أو الصور المعروضة في دفتر العمل، ويصبح ساريًا عندما يكون IslimitShapeOrImage=true. القيمة الافتراضية هي 300.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setMessageTopic(String value) {#setMessageTopic-java.lang.String-}
```
public void setMessageTopic(String value)
```


يضبط وجهات WebSocket التي تبدأ بـ "/topic". القيمة الافتراضية هي "/topic/opr". تُستخدم في وضع التعاون فقط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setPictureCacheDirectory(String value) {#setPictureCacheDirectory-java.lang.String-}
```
public void setPictureCacheDirectory(String value)
```


يضبط دليل التخزين المؤقت للصور. (يصبح ساريًا عندما يكون GridJsWorkbook.CacheImp فارغًا) المسار الافتراضي سيكون "\_piccache" داخل FileCacheDirectory.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setSameImageDetecting(boolean value) {#setSameImageDetecting-boolean-}
```
public void setSameImageDetecting(boolean value)
```


يضبط ما إذا كان سيتم التحقق مما إذا كانت الصور لها نفس المصدر، القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSaveHtmlAsZip(boolean value) {#setSaveHtmlAsZip-boolean-}
```
public void setSaveHtmlAsZip(boolean value)
```


يضبط ما إذا كان سيتم حفظ ملف HTML كأرشيف zip، القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowChartSheet(boolean value) {#setShowChartSheet-boolean-}
```
public void setShowChartSheet(boolean value)
```


يضبط ما إذا كان سيتم إظهار ورقة عمل المخطط. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSkipInvisibleShapes(boolean value) {#setSkipInvisibleShapes-boolean-}
```
public void setSkipInvisibleShapes(boolean value)
```


يضبط ما إذا كان سيتم تخطي الأشكال غير المرئية لواجهة المستخدم، القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setUsePrintArea(boolean value) {#setUsePrintArea-boolean-}
```
public void setUsePrintArea(boolean value)
```


يضبط ما إذا كان سيتم استخدام PageSetup.PrintArea لنطاق العرض في واجهة المستخدم عندما تحتوي ورقة العمل على إعداد PageSetup لـ PrintArea. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setWasm(boolean value) {#setWasm-boolean-}
```
public void setWasm(boolean value)
```


يضبط ما إذا كان GridJs يعمل داخل مضيف WebAssembly للمتصفح بدلاً من عملية خادم. عندما تكون true، لا يتم استخدام أي مسار FileCacheDirectory / قرص / مقاطعة‑الخيط، ويجب أن يأتي التخزين المؤقت للملفات من CacheImp، لأن مضيف المتصفح لا يمتلك قرصًا محليًا. يختار مسارات الشيفرة أثناء التشغيل، لذا فإن Aspose.Cells.GridJs.dll واحدة تخدم كلا المضيفين. القيمة الافتراضية هي false.

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

