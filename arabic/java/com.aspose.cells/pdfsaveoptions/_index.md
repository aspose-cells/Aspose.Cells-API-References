---
title: "PdfSaveOptions"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل الخيارات لحفظ ملف PDF."
type: docs
url: /ar/java/com.aspose.cells/pdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions), [com.aspose.cells.PaginatedSaveOptions](../../com.aspose.cells/paginatedsaveoptions)
```
public class PdfSaveOptions extends PaginatedSaveOptions
```

يمثل الخيارات لحفظ ملف PDF.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | ينشئ الخيارات لحفظ ملف pdf. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllColumnsInOnePagePerSheet()](#getAllColumnsInOnePagePerSheet--) | إذا كان AllColumnsInOnePagePerSheet true، سيتم إخراج محتوى جميع الأعمدة في ورقة واحدة إلى صفحة واحدة فقط في النتيجة. |
| [getBookmark()](#getBookmark--) | يحصل على كائن [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry). |
| [getCachedFileFolder()](#getCachedFileFolder--) | المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة تخزين مؤقت للبيانات. |
| [getCalculateFormula()](#getCalculateFormula--) | يشير إلى ما إذا كان يجب حساب الصيغ قبل حفظ ملف PDF. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المرتبطة بالخلايا. |
| [getCheckFontCompatibility()](#getCheckFontCompatibility--) | يشير إلى ما إذا كان يجب فحص توافق الخط لكل حرف في النص. |
| [getCheckWorkbookDefaultFont()](#getCheckWorkbookDefaultFont--) | عند كون الأحرف في Excel يونيكود ولم يتم تعيين الخط الصحيح في نمط الخلية، قد تظهر ككتل في pdf أو صورة. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | اجعل دفتر العمل فارغًا بعد حفظ الملف. |
| [getCompliance()](#getCompliance--) | يحصل على مستوى التوافق مع معايير PDF للمستندات الناتجة. |
| [getCreateDirectory()](#getCreateDirectory--) | إذا كان صحيحًا ولم يكن الدليل موجودًا، فسيتم إنشاء الدليل تلقائيًا قبل حفظ الملف. |
| [getCreatedTime()](#getCreatedTime--) | يحصل على وقت إنشاء مستند PDF. |
| [getCustomPropertiesExport()](#getCustomPropertiesExport--) | يحصل على قيمة تحدد طريقة تصدير [CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection) إلى ملف PDF. |
| [getCustomRenderSettings()](#getCustomRenderSettings--) | يحصل على الإعدادات المخصصة أثناء التصيير. |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | يحصل على لغة التحرير الافتراضية. |
| [getDefaultFont()](#getDefaultFont--) | عند كون الأحرف في Excel يونيكود ولم يتم تعيين الخط الصحيح في نمط الخلية، قد تظهر ككتل في pdf أو صورة. |
| [getDisplayDocTitle()](#getDisplayDocTitle--) | يشير إلى ما إذا كان شريط عنوان النافذة يجب أن يعرض عنوان المستند. |
| [getDrawObjectEventHandler()](#getDrawObjectEventHandler--) | يُنفّذ هذه الواجهة للحصول على DrawObject و Bound عند التصيير. |
| [getEmbedAttachments()](#getEmbedAttachments--) | يشير إلى ما إذا كان يجب تضمين مرفق لكائنات OLE في Excel. |
| [getEmbedStandardWindowsFonts()](#getEmbedStandardWindowsFonts--) | صحيح لتضمين خطوط TrueType. |
| [getEmfRenderSetting()](#getEmfRenderSetting--) | إعداد لتصيير ملف Emf الوصفي. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | يحدد ما إذا كان يتم تشفير خصائص المستند عند الحفظ كملف .xls. |
| [getExportDocumentStructure()](#getExportDocumentStructure--) | يشير إلى ما إذا كان يجب تصدير بنية المستند. |
| [getFontEncoding()](#getFontEncoding--) | يحصل على ترميز الخط المضمن في PDF. |
| [getGridlineColor()](#getGridlineColor--) | يحصل على لون خطوط الشبكة. |
| [getGridlineType()](#getGridlineType--) | يحصل على نوع خطوط الشبكة. |
| [getIgnoreError()](#getIgnoreError--) | يشير إلى ما إذا كنت بحاجة لإخفاء الخطأ أثناء التصيير. |
| [getImageType()](#getImageType--) | يمثل نوع الصورة عند تحويل المخطط والشكل. |
| [getMergeAreas()](#getMergeAreas--) | يحدد ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق قبل حفظ الملف. |
| [getOnePagePerSheet()](#getOnePagePerSheet--) | إذا كان OnePagePerSheet true، سيتم إخراج جميع محتويات ورقة واحدة إلى صفحة واحدة فقط في النتيجة. |
| [getOptimizationType()](#getOptimizationType--) | يحصل على نوع تحسين PDF. |
| [getOutputBlankPageWhenNothingToPrint()](#getOutputBlankPageWhenNothingToPrint--) | يشير إلى ما إذا كان يجب إخراج صفحة فارغة عندما لا يوجد شيء للطباعة. |
| [getPageCount()](#getPageCount--) | يحصل على عدد الصفحات التي سيتم حفظها. |
| [getPageIndex()](#getPageIndex--) | يحصل على الفهرس القائم على الصفر للصفحة الأولى التي سيتم حفظها. |
| [getPageSavingCallback()](#getPageSavingCallback--) | التحكم/الإشارة إلى تقدم عملية حفظ الصفحة. |
| [getPdfCompression()](#getPdfCompression--) | حدد خوارزمية الضغط |
| [getPrintingPageType()](#getPrintingPageType--) | يشير إلى الصفحات التي لن تُطبع. |
| [getProducer()](#getProducer--) | يحصل على المنتج للمستند PDF المُنشأ. |
| [getRefreshChartCache()](#getRefreshChartCache--) | يحدد ما إذا كان يتم تخزين أحدث بيانات المخطط مؤقتًا. |
| [getRenderingBehavior()](#getRenderingBehavior--) | يحصل على سلوكيات التصيير الخاصة بـ Excel لتطبيقها. |
| [getSaveFormat()](#getSaveFormat--) | يحصل على صيغة حفظ الملف. |
| [getSecurityOptions()](#getSecurityOptions--) | قم بتعيين هذه الخيارات عندما تكون الأمان مطلوبًا في نتيجة xls2pdf. |
| [getSheetSet()](#getSheetSet--) | يحصل على الأوراق التي سيتم عرضها. |
| [getSortExternalNames()](#getSortExternalNames--) | يحدد ما إذا كان يتم فرز الأسماء المعرفة الخارجية قبل حفظ الملف. |
| [getSortNames()](#getSortNames--) | يحدد ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف. |
| [getTextCrossType()](#getTextCrossType--) | يحصل على نوع عرض النص عندما يكون عرض النص أكبر من عرض الخلية. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | يحدد ما إذا كان يتم تحديث إعدادات Smart Art. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | يحدد ما إذا كان يتم التحقق من صحة الخلايا المدمجة قبل حفظ الملف. |
| [getWarningCallback()](#getWarningCallback--) | يحصل على رد النداء للتحذير. |
| [getWatermark()](#getWatermark--) | يحصل على العلامة المائية للإخراج. |
| [getZoomBehavior()](#getZoomBehavior--) | يحصل على وضع العرض الأولي عند فتح المستند PDF المُنشأ. |
| [getZoomFactor()](#getZoomFactor--) | يحصل على نسبة التكبير المستخدمة عندما يكون [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\#getZoomBehavior--) هو [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\#ZOOM-FACTOR). |
| [hashCode()](#hashCode--) |  |
| [isFontSubstitutionCharGranularity()](#isFontSubstitutionCharGranularity--) | يشير إلى ما إذا كان يجب استبدال خط الحرف فقط عندما يكون خط الخلية غير متوافق معه. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllColumnsInOnePagePerSheet(boolean value)](#setAllColumnsInOnePagePerSheet-boolean-) | إذا كان AllColumnsInOnePagePerSheet true، سيتم إخراج محتوى جميع الأعمدة في ورقة واحدة إلى صفحة واحدة فقط في النتيجة. |
| [setBookmark(PdfBookmarkEntry value)](#setBookmark-com.aspose.cells.PdfBookmarkEntry-) | يضبط كائن [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry). |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة تخزين مؤقت للبيانات. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | يشير إلى ما إذا كان يجب حساب الصيغ قبل حفظ ملف PDF. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المرتبطة بالخلايا. |
| [setCheckFontCompatibility(boolean value)](#setCheckFontCompatibility-boolean-) | يشير إلى ما إذا كان يجب فحص توافق الخط لكل حرف في النص. |
| [setCheckWorkbookDefaultFont(boolean value)](#setCheckWorkbookDefaultFont-boolean-) | عند كون الأحرف في Excel يونيكود ولم يتم تعيين الخط الصحيح في نمط الخلية، قد تظهر ككتل في pdf أو صورة. |
| [setClearData(boolean value)](#setClearData-boolean-) | اجعل دفتر العمل فارغًا بعد حفظ الملف. |
| [setCompliance(int value)](#setCompliance-int-) | يضبط مستوى التوافق مع معايير PDF للمستندات الناتجة. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | إذا كان صحيحًا ولم يكن الدليل موجودًا، فسيتم إنشاء الدليل تلقائيًا قبل حفظ الملف. |
| [setCreatedTime(DateTime value)](#setCreatedTime-com.aspose.cells.DateTime-) | يضبط وقت إنشاء مستند PDF. |
| [setCustomPropertiesExport(int value)](#setCustomPropertiesExport-int-) | يضبط قيمة تحدد طريقة تصدير [CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection) إلى ملف PDF. |
| [setCustomRenderSettings(CustomRenderSettings value)](#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-) | يضبط الإعدادات المخصصة أثناء التصيير. |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | يضبط لغة التحرير الافتراضية. |
| [setDefaultFont(String value)](#setDefaultFont-java.lang.String-) | عند كون الأحرف في Excel يونيكود ولم يتم تعيين الخط الصحيح في نمط الخلية، قد تظهر ككتل في pdf أو صورة. |
| [setDisplayDocTitle(boolean value)](#setDisplayDocTitle-boolean-) | يشير إلى ما إذا كان شريط عنوان النافذة يجب أن يعرض عنوان المستند. |
| [setDrawObjectEventHandler(DrawObjectEventHandler value)](#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-) | يُنفّذ هذه الواجهة للحصول على DrawObject و Bound عند التصيير. |
| [setEmbedAttachments(boolean value)](#setEmbedAttachments-boolean-) | يشير إلى ما إذا كان يجب تضمين مرفق لكائنات OLE في Excel. |
| [setEmbedStandardWindowsFonts(boolean value)](#setEmbedStandardWindowsFonts-boolean-) | صحيح لتضمين خطوط TrueType. |
| [setEmfRenderSetting(int value)](#setEmfRenderSetting-int-) | إعداد لتصيير ملف Emf الوصفي. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | يحدد ما إذا كان يتم تشفير خصائص المستند عند الحفظ كملف .xls. |
| [setExportDocumentStructure(boolean value)](#setExportDocumentStructure-boolean-) | يشير إلى ما إذا كان يجب تصدير بنية المستند. |
| [setFontEncoding(int value)](#setFontEncoding-int-) | يضبط ترميز الخط المضمن في PDF. |
| [setFontSubstitutionCharGranularity(boolean value)](#setFontSubstitutionCharGranularity-boolean-) | يشير إلى ما إذا كان يجب استبدال خط الحرف فقط عندما يكون خط الخلية غير متوافق معه. |
| [setGridlineColor(Color value)](#setGridlineColor-com.aspose.cells.Color-) | يضبط لون خطوط الشبكة. |
| [setGridlineType(int value)](#setGridlineType-int-) | يضبط نوع خطوط الشبكة. |
| [setIgnoreError(boolean value)](#setIgnoreError-boolean-) | يشير إلى ما إذا كنت بحاجة لإخفاء الخطأ أثناء التصيير. |
| [setImageResample(int desiredPPI, int jpegQuality)](#setImageResample-int-int-) | يضبط الـ PPI (بكسل لكل بوصة) المطلوب للصور المعاد أخذ عيناتها وجودة JPEG. |
| [setImageType(ImageFormat value)](#setImageType-com.aspose.cells.ImageFormat-) | يمثل نوع الصورة عند تحويل المخطط والشكل. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | يحدد ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق قبل حفظ الملف. |
| [setOnePagePerSheet(boolean value)](#setOnePagePerSheet-boolean-) | إذا كان OnePagePerSheet true، سيتم إخراج جميع محتويات ورقة واحدة إلى صفحة واحدة فقط في النتيجة. |
| [setOptimizationType(int value)](#setOptimizationType-int-) | يضبط نوع تحسين PDF. |
| [setOutputBlankPageWhenNothingToPrint(boolean value)](#setOutputBlankPageWhenNothingToPrint-boolean-) | يشير إلى ما إذا كان يجب إخراج صفحة فارغة عندما لا يوجد شيء للطباعة. |
| [setPageCount(int value)](#setPageCount-int-) | يضبط عدد الصفحات التي سيتم حفظها. |
| [setPageIndex(int value)](#setPageIndex-int-) | يضبط الفهرس القائم على الصفر للصفحة الأولى التي سيتم حفظها. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-) | التحكم/الإشارة إلى تقدم عملية حفظ الصفحة. |
| [setPdfCompression(int value)](#setPdfCompression-int-) | حدد خوارزمية الضغط |
| [setPrintingPageType(int value)](#setPrintingPageType-int-) | يشير إلى الصفحات التي لن تُطبع. |
| [setProducer(String value)](#setProducer-java.lang.String-) | يضبط المنتج للمستند PDF المُنشأ. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | يحدد ما إذا كان يتم تخزين أحدث بيانات المخطط مؤقتًا. |
| [setRenderingBehavior(int value)](#setRenderingBehavior-int-) | يضبط سلوكيات التصيير الخاصة بـ Excel لتطبيقها. |
| [setSecurityOptions(PdfSecurityOptions value)](#setSecurityOptions-com.aspose.cells.PdfSecurityOptions-) | قم بتعيين هذه الخيارات عندما تكون الأمان مطلوبًا في نتيجة xls2pdf. |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | يضبط الأوراق التي سيتم عرضها. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | يحدد ما إذا كان يتم فرز الأسماء المعرفة الخارجية قبل حفظ الملف. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | يحدد ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف. |
| [setTextCrossType(int value)](#setTextCrossType-int-) | يضبط نوع عرض النص عندما يكون عرض النص أكبر من عرض الخلية. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | يحدد ما إذا كان يتم تحديث إعدادات Smart Art. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | يحدد ما إذا كان يتم التحقق من صحة الخلايا المدمجة قبل حفظ الملف. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | يضبط رد النداء للتحذير. |
| [setWatermark(RenderingWatermark value)](#setWatermark-com.aspose.cells.RenderingWatermark-) | يضبط العلامة المائية للإخراج. |
| [setZoomBehavior(int value)](#setZoomBehavior-int-) | يضبط وضع العرض الأولي عند فتح مستند PDF المُولَّد. |
| [setZoomFactor(int value)](#setZoomFactor-int-) | يضبط نسبة التكبير المستخدمة عندما يكون [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\#getZoomBehavior--) هو [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\#ZOOM-FACTOR). |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


ينشئ الخيارات لحفظ ملف pdf.

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
### getAllColumnsInOnePagePerSheet() {#getAllColumnsInOnePagePerSheet--}
```
public boolean getAllColumnsInOnePagePerSheet()
```


إذا كان AllColumnsInOnePagePerSheet صحيحًا، سيتم إخراج جميع محتويات الأعمدة في ورقة واحدة إلى صفحة واحدة فقط في النتيجة. سيتم تجاهل عرض حجم الورق في إعدادات الصفحة، وستظل الإعدادات الأخرى لإعدادات الصفحة سارية.

**Returns:**
boolean
### getBookmark() {#getBookmark--}
```
public PdfBookmarkEntry getBookmark()
```


يحصل على كائن [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry).

**Returns:**
[PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry)
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة تخزين مؤقت للبيانات.

**Remarks**

إذا لم يتم تحديد المجلد، تكون القيمة الافتراضية له هي [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). إذا كانت قيمته الافتراضية null أو فارغة، أو تم تحديدها كـ null أو فارغة، فلن يتم استخدام أي ملف ذاكرة مؤقتة عند حفظ دفتر العمل.

**Returns:**
java.lang.String
### getCalculateFormula() {#getCalculateFormula--}
```
public boolean getCalculateFormula()
```


يشير إلى ما إذا كان يجب حساب الصيغ قبل حفظ ملف PDF.

**Remarks**

القيمة الافتراضية هي false.

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المتعلقة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32K. عندما تدخل قيمة أطول من 32K، سيتم قطعها.

**Returns:**
boolean
### getCheckFontCompatibility() {#getCheckFontCompatibility--}
```
public boolean getCheckFontCompatibility()
```


يشير إلى ما إذا كان يجب فحص توافق الخط لكل حرف في النص.

**Remarks**

القيمة الافتراضية هي true. قد يؤدي تعطيل هذه الخاصية إلى تحسين الأداء. ولكن عندما لا يمكن استخدام الخط الافتراضي أو المحدد للنص/الحرف في تصييره، قد تظهر أحرف غير قابلة للقراءة (مثل المربعات) في ملف PDF المُولد. في مثل هذه الحالة يجب على المستخدم إبقاء هذه الخاصية كـ true حتى يتم البحث عن خط بديل واستخدامه لتصيير النص بدلاً من ذلك؛

**Returns:**
boolean
### getCheckWorkbookDefaultFont() {#getCheckWorkbookDefaultFont--}
```
public boolean getCheckWorkbookDefaultFont()
```


عندما تكون الأحرف في Excel يونيكود ولم يتم تعيين الخط الصحيح في نمط الخلية، قد تظهر كمربعات في PDF أو صورة. اضبط هذا إلى true لمحاولة استخدام الخط الافتراضي للدفتر لإظهار هذه الأحرف أولاً.

**Remarks**

القيمة الافتراضية هي true.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getClearData() {#getClearData--}
```
public boolean getClearData()
```


اجعل دفتر العمل فارغًا بعد حفظ الملف.

**Returns:**
boolean
### getCompliance() {#getCompliance--}
```
public int getCompliance()
```


يحصل على مستوى التوافق مع معايير PDF للمستندات الناتجة.

انظر [PdfCompliance](../../com.aspose.cells/pdfcompliance).

**Remarks**

القيمة الافتراضية هي Pdf17.

**Returns:**
int
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


إذا كان صحيحًا ولم يكن الدليل موجودًا، فسيتم إنشاء الدليل تلقائيًا قبل حفظ الملف.

**Remarks**

القيمة الافتراضية هي false.

**Returns:**
boolean
### getCreatedTime() {#getCreatedTime--}
```
public DateTime getCreatedTime()
```


يحصل على وقت إنشاء مستند PDF.

**Remarks**

إذا لم يتم تعيينه، فسيكون وقت إنشاء ملف PDF.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getCustomPropertiesExport() {#getCustomPropertiesExport--}
```
public int getCustomPropertiesExport()
```


يحصل على قيمة تحدد طريقة تصدير [CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection) إلى ملف PDF. القيمة الافتراضية هي None.

انظر [PdfCustomPropertiesExport](../../com.aspose.cells/pdfcustompropertiesexport).

**Returns:**
int
### getCustomRenderSettings() {#getCustomRenderSettings--}
```
public CustomRenderSettings getCustomRenderSettings()
```


يحصل على الإعدادات المخصصة أثناء التصيير.

**Returns:**
[CustomRenderSettings](../../com.aspose.cells/customrendersettings)
### getDefaultEditLanguage() {#getDefaultEditLanguage--}
```
public int getDefaultEditLanguage()
```


يحصل على لغة التحرير الافتراضية.

انظر [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

قد يعرض/يُصوّر تخطيطات مختلفة لفقرة النص عندما يتم تعيين لغات تحرير مختلفة. القيمة الافتراضية هي [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).

**Returns:**
int
### getDefaultFont() {#getDefaultFont--}
```
public String getDefaultFont()
```


عندما تكون الأحرف في Excel يونيكود ولم يتم تعيين الخط الصحيح في نمط الخلية، قد تظهر كمربعات في PDF أو صورة. اضبط DefaultFont مثل MingLiu أو MS Gothic لإظهار هذه الأحرف. إذا لم يتم ضبط هذه الخاصية، سيستخدم Aspose.Cells الخط الافتراضي للنظام لإظهار هذه الأحرف اليونيكود.

**Returns:**
java.lang.String
### getDisplayDocTitle() {#getDisplayDocTitle--}
```
public boolean getDisplayDocTitle()
```


يشير إلى ما إذا كان شريط عنوان النافذة يجب أن يعرض عنوان المستند.

**Remarks**

إذا كان false، يجب أن يعرض شريط العنوان بدلاً من ذلك اسم ملف PDF. القيمة الافتراضية هي false.

**Returns:**
boolean
### getDrawObjectEventHandler() {#getDrawObjectEventHandler--}
```
public DrawObjectEventHandler getDrawObjectEventHandler()
```


يُنفّذ هذه الواجهة للحصول على DrawObject و Bound عند التصيير.

**Returns:**
[DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler)
### getEmbedAttachments() {#getEmbedAttachments--}
```
public boolean getEmbedAttachments()
```


يشير إلى ما إذا كان يجب تضمين مرفق لكائنات OLE في Excel.

**Remarks**

القيمة الافتراضية هي false. يجب أن تكون القيمة false عندما يتم تعيين توافق PDF/A أو تم تمكين تشفير PDF.

**Returns:**
boolean
### getEmbedStandardWindowsFonts() {#getEmbedStandardWindowsFonts--}
```
public boolean getEmbedStandardWindowsFonts()
```


True لتضمين خطوط TrueType. يؤثر فقط على أحرف ASCII من 32 إلى 127. الخطوط لأكواد الأحرف التي تزيد عن 127 يتم تضمينها دائمًا. الخطوط يتم تضمينها دائمًا للمعيار PDF/A-1a و PDF/A-1b. القيمة الافتراضية هي true.

**Returns:**
boolean
### getEmfRenderSetting() {#getEmfRenderSetting--}
```
public int getEmfRenderSetting()
```


إعداد لتصيير ملف Emf الوصفي.

انظر [EmfRenderSetting](../../com.aspose.cells/emfrendersetting).

**Remarks**

يمكن لملفات تعريف EMF التي تم تحديدها كـ "EMF+ Dual" أن تحتوي على كل من سجلات EMF+ وسجلات EMF. يمكن استخدام أي نوع من السجلات لتصيير الصورة، أو سجلات EMF+ فقط، أو سجلات EMF فقط. عندما يتم ضبط [EmfRenderSetting.EMF\_PLUS\_PREFER](../../com.aspose.cells/emfrendersetting\#EMF-PLUS-PREFER)، سيتم تحليل سجلات EMF+ أثناء التصيير إلى الصفحة، وإلا سيتم تحليل سجلات EMF فقط. القيمة الافتراضية هي [EmfRenderSetting.EMF\_ONLY](../../com.aspose.cells/emfrendersetting\#EMF-ONLY).

**Returns:**
int
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```


يشير إلى ما إذا كان يتم تشفير خصائص المستند عند الحفظ كملف .xls. القيمة الافتراضية هي true.

**Remarks**

لملفات .xls, .xlsx, .xlsb و .xlsm فقط.

**Returns:**
boolean
### getExportDocumentStructure() {#getExportDocumentStructure--}
```
public boolean getExportDocumentStructure()
```


يشير إلى ما إذا كان يجب تصدير بنية المستند.

**Returns:**
boolean
### getFontEncoding() {#getFontEncoding--}
```
public int getFontEncoding()
```


يحصل على ترميز الخط المضمن في PDF.

انظر [PdfFontEncoding](../../com.aspose.cells/pdffontencoding).

**Remarks**

القيمة الافتراضية هي [PdfFontEncoding.IDENTITY](../../com.aspose.cells/pdffontencoding\#IDENTITY)

**Returns:**
int
### getGridlineColor() {#getGridlineColor--}
```
public Color getGridlineColor()
```


يحصل على لون خطوط الشبكة.

**Remarks**

سيتجاهل إعدادات لون خطوط الشبكة في ملف المصدر.

**Returns:**
[Color](../../com.aspose.cells/color)
### getGridlineType() {#getGridlineType--}
```
public int getGridlineType()
```


يحصل على نوع خطوط الشبكة.

انظر [GridlineType](../../com.aspose.cells/gridlinetype).

**Remarks**

القيمة الافتراضية هي النوع المنقط.

**Returns:**
int
### getIgnoreError() {#getIgnoreError--}
```
public boolean getIgnoreError()
```


يشير إلى ما إذا كنت بحاجة إلى إخفاء الخطأ أثناء التصيير. قد يكون الخطأ في الشكل أو الصورة أو تصيير المخطط، إلخ.

**Returns:**
boolean
### getImageType() {#getImageType--}
```
public ImageFormat getImageType()
```


يمثل نوع الصورة عند تحويل المخطط والشكل.

**Remarks**

NOTE: هذا العضو الآن مهمل. بدلاً من ذلك، يتم دائمًا عرض **Chart** و **Shape** كعناصر متجهية (مثل النقطة، الخط) لتحسين جودة العرض. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
[ImageFormat](../../com.aspose.cells/imageformat)
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


يحدد ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق قبل حفظ الملف.

**Remarks**

القيمة الافتراضية هي false.

**Returns:**
boolean
### getOnePagePerSheet() {#getOnePagePerSheet--}
```
public boolean getOnePagePerSheet()
```


إذا كان OnePagePerSheet صحيحًا، فسيتم إخراج كل محتوى ورقة واحدة إلى صفحة واحدة فقط في النتيجة. سيكون حجم الورق في pagesetup غير صالح، وستظل الإعدادات الأخرى لـ pagesetup سارية.

**Returns:**
boolean
### getOptimizationType() {#getOptimizationType--}
```
public int getOptimizationType()
```


يحصل على نوع تحسين PDF.

انظر [PdfOptimizationType](../../com.aspose.cells/pdfoptimizationtype).

**Remarks**

القيمة الافتراضية هي [PdfOptimizationType.STANDARD](../../com.aspose.cells/pdfoptimizationtype\#STANDARD)

**Returns:**
int
### getOutputBlankPageWhenNothingToPrint() {#getOutputBlankPageWhenNothingToPrint--}
```
public boolean getOutputBlankPageWhenNothingToPrint()
```


يشير إلى ما إذا كان يجب إخراج صفحة فارغة عندما لا يوجد شيء للطباعة.

**Remarks**

القيمة الافتراضية هي true.

**Returns:**
boolean
### getPageCount() {#getPageCount--}
```
public int getPageCount()
```


يحصل على عدد الصفحات التي سيتم حفظها.

**Remarks**

القيمة الافتراضية هي System.Int32.MaxValue مما يعني أنه سيتم عرض جميع الصفحات.

**Example**

المثال التالي يوضح كيفية تحويل نطاق من الصفحات (3 و 4) في ملف Microsoft Excel إلى PDF.

```
         //Open an Excel file
         Workbook wb = new Workbook("Book1.xlsx");
 
         PdfSaveOptions options = new PdfSaveOptions();
 
         //Print only Page 3 and Page 4 in the output PDF
         //Starting page index (0-based index)
         options.setPageIndex(3);
         //Number of pages to be printed
         options.setPageCount(2);
 
         //Save the PDF file
         wb.save("output.pdf", options);
```

**Returns:**
int
### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


يحصل على الفهرس القائم على الصفر للصفحة الأولى التي سيتم حفظها.

**Remarks**

القيمة الافتراضية هي 0.

**Example**

المثال التالي يوضح كيفية تحويل نطاق من الصفحات (3 و 4) في ملف Microsoft Excel إلى PDF.

```
         //Open an Excel file
         Workbook wb = new Workbook("Book1.xlsx");
 
         PdfSaveOptions options = new PdfSaveOptions();
 
         //Print only Page 3 and Page 4 in the output PDF
         //Starting page index (0-based index)
         options.setPageIndex(3);
         //Number of pages to be printed
         options.setPageCount(2);
 
         //Save the PDF file
         wb.save("output.pdf", options);
```

**Returns:**
int
### getPageSavingCallback() {#getPageSavingCallback--}
```
public IPageSavingCallback getPageSavingCallback()
```


التحكم/الإشارة إلى تقدم عملية حفظ الصفحة.

**Returns:**
[IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback)
### getPdfCompression() {#getPdfCompression--}
```
public int getPdfCompression()
```


حدد خوارزمية الضغط

انظر [PdfCompressionCore](../../com.aspose.cells/pdfcompressioncore).

**Returns:**
int
### getPrintingPageType() {#getPrintingPageType--}
```
public int getPrintingPageType()
```


يشير إلى الصفحات التي لن تُطبع.

انظر [PrintingPageType](../../com.aspose.cells/printingpagetype).

**Remarks**

إذا كان المحتوى في الورقة متفرقًا، فستظهر بعض الصفحات فارغة تمامًا في ملف PDF الناتج. إذا كنت لا تريد هذه الصفحات الفارغة، يمكنك استخدام هذا الخيار لتخطيها.

**Example**

الكود التالي يتخطى الصفحات الفارغة أو الصفحات التي تحتوي فقط على بعض محتوى التنسيق مثل خلفية الخلية والحدود.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
 
         //ignore blank pages
         pdfSaveOptions.setPrintingPageType(PrintingPageType.IGNORE_BLANK);
 
         wb.save("output_ignore_blank_page.pdf", pdfSaveOptions);
 
 
         //ignore blank pages and pages which only contains some style content like cell background
         pdfSaveOptions.setPrintingPageType(PrintingPageType.IGNORE_STYLE);
 
         wb.save("output_ignore_blank_and_style_page.pdf", pdfSaveOptions);
```

**Returns:**
int
### getProducer() {#getProducer--}
```
public String getProducer()
```


يحصل على المنتج للمستند PDF المُنشأ.

**Remarks**

إذا كانت القيمة null، أو لم يتم تعيين LICENSE صالح، سيتم استخدام السلسلة Aspose.Cells vVERSION.

**Returns:**
java.lang.String
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


يحدد ما إذا كان يتم تخزين أحدث بيانات المخطط مؤقتًا.

**Returns:**
boolean
### getRenderingBehavior() {#getRenderingBehavior--}
```
public int getRenderingBehavior()
```


يحصل على سلوكيات التصيير الخاصة بـ Excel لتطبيقها.

انظر [ExcelRenderingBehavior](../../com.aspose.cells/excelrenderingbehavior).

**Remarks**

القيمة الافتراضية هي [ExcelRenderingBehavior.ALL](../../com.aspose.cells/excelrenderingbehavior\#ALL).

**Returns:**
int
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


يحصل على صيغة حفظ الملف.

انظر [SaveFormat](../../com.aspose.cells/saveformat).

**Returns:**
int
### getSecurityOptions() {#getSecurityOptions--}
```
public PdfSecurityOptions getSecurityOptions()
```


قم بتعيين هذه الخيارات عندما تكون الأمان مطلوبًا في نتيجة xls2pdf.

**Example**

الكود التالي يضبط إذن طباعة دقة الارتفاع لملف PDF الناتج.

```
         Workbook wb = new Workbook();
         wb.getWorksheets().get(0).getCells().get("A1").setValue("Aspose");
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
 
 
         PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();
 
         //set owner password
         pdfSecurityOptions.setOwnerPassword("YourOwnerPassword");
 
         //set user password
         pdfSecurityOptions.setUserPassword("YourUserPassword");
 
         //set print permisson
         pdfSecurityOptions.setPrintPermission(true);
 
         //set high resolution for print
         pdfSecurityOptions.setFullQualityPrintPermission(true);
 
 
         pdfSaveOptions.setSecurityOptions(pdfSecurityOptions);
 
         wb.save("output.pdf", pdfSaveOptions);
```

**Returns:**
[PdfSecurityOptions](../../com.aspose.cells/pdfsecurityoptions)
### getSheetSet() {#getSheetSet--}
```
public SheetSet getSheetSet()
```


يحصل على الأوراق التي سيتم عرضها. الافتراضي هو جميع الأوراق المرئية في المصنف: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\\#getVisible--).

**Example**

الكود التالي يعرض فقط الورقة النشطة إلى PDF.

```
         Workbook workbook = new Workbook("Book1.xlsx");
 
         int activeSheetIndex = workbook.getWorksheets().getActiveSheetIndex();
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
         //set active sheet index to sheet set.
         pdfSaveOptions.setSheetSet(new SheetSet(new int[] { activeSheetIndex }));
         workbook.save("output.pdf", pdfSaveOptions);
```

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getSortExternalNames() {#getSortExternalNames--}
```
public boolean getSortExternalNames()
```


يحدد ما إذا كان يتم فرز الأسماء المعرفة الخارجية قبل حفظ الملف.

**Returns:**
boolean
### getSortNames() {#getSortNames--}
```
public boolean getSortNames()
```


يحدد ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف.

**Returns:**
boolean
### getTextCrossType() {#getTextCrossType--}
```
public int getTextCrossType()
```


يحصل على نوع عرض النص عندما يكون عرض النص أكبر من عرض الخلية.

انظر [TextCrossType](../../com.aspose.cells/textcrosstype).

**Returns:**
int
### getUpdateSmartArt() {#getUpdateSmartArt--}
```
public boolean getUpdateSmartArt()
```


يشير إلى ما إذا كان يتم تحديث إعدادات Smart Art. القيمة الافتراضية هي false.

**Remarks**

يؤثر فقط بعد استدعاء الطريقة Shape.GetResultOfSmartArt() ووجود الأشكال المخزنة مؤقتًا في ملف القالب.

**Returns:**
boolean
### getValidateMergedAreas() {#getValidateMergedAreas--}
```
public boolean getValidateMergedAreas()
```


يحدد ما إذا كان يتم التحقق من صحة الخلايا المدمجة قبل حفظ الملف.

**Remarks**

القيمة الافتراضية هي false.

**Returns:**
boolean
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


يحصل على رد النداء للتحذير.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### getWatermark() {#getWatermark--}
```
public RenderingWatermark getWatermark()
```


يحصل على العلامة المائية للإخراج.

**Example**

الكود التالي يضبط العلامة المائية في ملف PDF الناتج.

```
         //prepare a workbook with 3 pages.
         Workbook wb = new Workbook();
         wb.getWorksheets().get(0).getCells().get("A1").putValue("Page1");
         int index = wb.getWorksheets().add();
         wb.getWorksheets().get(index).getCells().get("A1").putValue("Page2");
         index = wb.getWorksheets().add();
         wb.getWorksheets().get(index).getCells().get("A1").putValue("Page3");
         wb.getWorksheets().get(index).getPageSetup().setPaperSize(PaperSizeType.PAPER_A_3);
 
         //create a font for watermark, and specify bold, italic, color
         RenderingFont font = new RenderingFont("Calibri", 68);
         font.setItalic(true);
         font.setBold(true);
         font.setColor(Color.getBlue());
 
         //create a watermark from text and the specified font
         RenderingWatermark watermark = new RenderingWatermark("Watermark", font);
 
         //specify horizontal and vertical alignment
         watermark.setHAlignment(TextAlignmentType.CENTER);
         watermark.setVAlignment(TextAlignmentType.CENTER);
 
         //specify rotation
         watermark.setRotation(30);
 
         //specify opacity
         watermark.setOpacity(0.6f);
 
         //specify the scale to page(e.g. 100, 50) in percent.
         watermark.setScaleToPagePercent(50);
 
         //spcify watermark for rendering to pdf.
         PdfSaveOptions options = new PdfSaveOptions();
         options.setWatermark(watermark);
 
         wb.save("output_watermark.pdf", options);
```

**Returns:**
[RenderingWatermark](../../com.aspose.cells/renderingwatermark)
### getZoomBehavior() {#getZoomBehavior--}
```
public int getZoomBehavior()
```


يحصل على وضع العرض الأولي عند فتح مستند PDF المُولَّد. القيمة الافتراضية هي [PdfZoomBehavior.NONE](../../com.aspose.cells/pdfzoombehavior\#NONE).

انظر [PdfZoomBehavior](../../com.aspose.cells/pdfzoombehavior).

**Returns:**
int
### getZoomFactor() {#getZoomFactor--}
```
public int getZoomFactor()
```


يحصل على نسبة التكبير المستخدمة عندما يكون [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\#getZoomBehavior--) هو [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\#ZOOM-FACTOR).

**Remarks**

يتم تجاهل هذه الخاصية ما لم يكن [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\#getZoomBehavior--) هو [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\#ZOOM-FACTOR).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isFontSubstitutionCharGranularity() {#isFontSubstitutionCharGranularity--}
```
public boolean isFontSubstitutionCharGranularity()
```


يشير إلى ما إذا كان يجب استبدال خط الحرف فقط عندما يكون خط الخلية غير متوافق معه.

**Remarks**

القيمة الافتراضية هي false. سنحاول أولاً الخط الافتراضي لملف Workbook وPdfSaveOption/system لخط الخلية.

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




### setAllColumnsInOnePagePerSheet(boolean value) {#setAllColumnsInOnePagePerSheet-boolean-}
```
public void setAllColumnsInOnePagePerSheet(boolean value)
```


إذا كان AllColumnsInOnePagePerSheet صحيحًا، سيتم إخراج جميع محتويات الأعمدة في ورقة واحدة إلى صفحة واحدة فقط في النتيجة. سيتم تجاهل عرض حجم الورق في إعدادات الصفحة، وستظل الإعدادات الأخرى لإعدادات الصفحة سارية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setBookmark(PdfBookmarkEntry value) {#setBookmark-com.aspose.cells.PdfBookmarkEntry-}
```
public void setBookmark(PdfBookmarkEntry value)
```


يضبط كائن [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry) |  |

### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة تخزين مؤقت للبيانات.

**Remarks**

إذا لم يتم تحديد المجلد، تكون القيمة الافتراضية له هي [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). إذا كانت قيمته الافتراضية null أو فارغة، أو تم تحديدها كـ null أو فارغة، فلن يتم استخدام أي ملف ذاكرة مؤقتة عند حفظ دفتر العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```


يشير إلى ما إذا كان يجب حساب الصيغ قبل حفظ ملف PDF.

**Remarks**

القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المتعلقة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32K. عندما تدخل قيمة أطول من 32K، سيتم قطعها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setCheckFontCompatibility(boolean value) {#setCheckFontCompatibility-boolean-}
```
public void setCheckFontCompatibility(boolean value)
```


يشير إلى ما إذا كان يجب فحص توافق الخط لكل حرف في النص.

**Remarks**

القيمة الافتراضية هي true. قد يؤدي تعطيل هذه الخاصية إلى تحسين الأداء. ولكن عندما لا يمكن استخدام الخط الافتراضي أو المحدد للنص/الحرف في تصييره، قد تظهر أحرف غير قابلة للقراءة (مثل المربعات) في ملف PDF المُولد. في مثل هذه الحالة يجب على المستخدم إبقاء هذه الخاصية كـ true حتى يتم البحث عن خط بديل واستخدامه لتصيير النص بدلاً من ذلك؛

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setCheckWorkbookDefaultFont(boolean value) {#setCheckWorkbookDefaultFont-boolean-}
```
public void setCheckWorkbookDefaultFont(boolean value)
```


عندما تكون الأحرف في Excel يونيكود ولم يتم تعيين الخط الصحيح في نمط الخلية، قد تظهر كمربعات في PDF أو صورة. اضبط هذا إلى true لمحاولة استخدام الخط الافتراضي للدفتر لإظهار هذه الأحرف أولاً.

**Remarks**

القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```


اجعل دفتر العمل فارغًا بعد حفظ الملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setCompliance(int value) {#setCompliance-int-}
```
public void setCompliance(int value)
```


يضبط مستوى التوافق مع معايير PDF للمستندات الناتجة.

انظر [PdfCompliance](../../com.aspose.cells/pdfcompliance).

**Remarks**

القيمة الافتراضية هي Pdf17.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```


إذا كان صحيحًا ولم يكن الدليل موجودًا، فسيتم إنشاء الدليل تلقائيًا قبل حفظ الملف.

**Remarks**

القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setCreatedTime(DateTime value) {#setCreatedTime-com.aspose.cells.DateTime-}
```
public void setCreatedTime(DateTime value)
```


يضبط وقت إنشاء مستند PDF.

**Remarks**

إذا لم يتم تعيينه، فسيكون وقت إنشاء ملف PDF.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setCustomPropertiesExport(int value) {#setCustomPropertiesExport-int-}
```
public void setCustomPropertiesExport(int value)
```


يضبط قيمة تحدد طريقة تصدير [CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection) إلى ملف PDF. القيمة الافتراضية هي None.

انظر [PdfCustomPropertiesExport](../../com.aspose.cells/pdfcustompropertiesexport).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setCustomRenderSettings(CustomRenderSettings value) {#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-}
```
public void setCustomRenderSettings(CustomRenderSettings value)
```


يضبط الإعدادات المخصصة أثناء التصيير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [CustomRenderSettings](../../com.aspose.cells/customrendersettings) |  |

### setDefaultEditLanguage(int value) {#setDefaultEditLanguage-int-}
```
public void setDefaultEditLanguage(int value)
```


يضبط لغة التحرير الافتراضية.

انظر [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

قد يعرض/يُصوّر تخطيطات مختلفة لفقرة النص عندما يتم تعيين لغات تحرير مختلفة. القيمة الافتراضية هي [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setDefaultFont(String value) {#setDefaultFont-java.lang.String-}
```
public void setDefaultFont(String value)
```


عندما تكون الأحرف في Excel يونيكود ولم يتم تعيين الخط الصحيح في نمط الخلية، قد تظهر كمربعات في PDF أو صورة. اضبط DefaultFont مثل MingLiu أو MS Gothic لإظهار هذه الأحرف. إذا لم يتم ضبط هذه الخاصية، سيستخدم Aspose.Cells الخط الافتراضي للنظام لإظهار هذه الأحرف اليونيكود.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setDisplayDocTitle(boolean value) {#setDisplayDocTitle-boolean-}
```
public void setDisplayDocTitle(boolean value)
```


يشير إلى ما إذا كان شريط عنوان النافذة يجب أن يعرض عنوان المستند.

**Remarks**

إذا كان false، يجب أن يعرض شريط العنوان بدلاً من ذلك اسم ملف PDF. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setDrawObjectEventHandler(DrawObjectEventHandler value) {#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-}
```
public void setDrawObjectEventHandler(DrawObjectEventHandler value)
```


يُنفّذ هذه الواجهة للحصول على DrawObject و Bound عند التصيير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler) |  |

### setEmbedAttachments(boolean value) {#setEmbedAttachments-boolean-}
```
public void setEmbedAttachments(boolean value)
```


يشير إلى ما إذا كان يجب تضمين مرفق لكائنات OLE في Excel.

**Remarks**

القيمة الافتراضية هي false. يجب أن تكون القيمة false عندما يتم تعيين توافق PDF/A أو تم تمكين تشفير PDF.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEmbedStandardWindowsFonts(boolean value) {#setEmbedStandardWindowsFonts-boolean-}
```
public void setEmbedStandardWindowsFonts(boolean value)
```


True لتضمين خطوط TrueType. يؤثر فقط على أحرف ASCII من 32 إلى 127. الخطوط لأكواد الأحرف التي تزيد عن 127 يتم تضمينها دائمًا. الخطوط يتم تضمينها دائمًا للمعيار PDF/A-1a و PDF/A-1b. القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEmfRenderSetting(int value) {#setEmfRenderSetting-int-}
```
public void setEmfRenderSetting(int value)
```


إعداد لتصيير ملف Emf الوصفي.

انظر [EmfRenderSetting](../../com.aspose.cells/emfrendersetting).

**Remarks**

يمكن لملفات تعريف EMF التي تم تحديدها كـ "EMF+ Dual" أن تحتوي على كل من سجلات EMF+ وسجلات EMF. يمكن استخدام أي نوع من السجلات لتصيير الصورة، أو سجلات EMF+ فقط، أو سجلات EMF فقط. عندما يتم ضبط [EmfRenderSetting.EMF\_PLUS\_PREFER](../../com.aspose.cells/emfrendersetting\#EMF-PLUS-PREFER)، سيتم تحليل سجلات EMF+ أثناء التصيير إلى الصفحة، وإلا سيتم تحليل سجلات EMF فقط. القيمة الافتراضية هي [EmfRenderSetting.EMF\_ONLY](../../com.aspose.cells/emfrendersetting\#EMF-ONLY).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setEncryptDocumentProperties(boolean value) {#setEncryptDocumentProperties-boolean-}
```
public void setEncryptDocumentProperties(boolean value)
```


يشير إلى ما إذا كان يتم تشفير خصائص المستند عند الحفظ كملف .xls. القيمة الافتراضية هي true.

**Remarks**

لملفات .xls, .xlsx, .xlsb و .xlsm فقط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExportDocumentStructure(boolean value) {#setExportDocumentStructure-boolean-}
```
public void setExportDocumentStructure(boolean value)
```


يشير إلى ما إذا كان يجب تصدير بنية المستند.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setFontEncoding(int value) {#setFontEncoding-int-}
```
public void setFontEncoding(int value)
```


يضبط ترميز الخط المضمن في PDF.

انظر [PdfFontEncoding](../../com.aspose.cells/pdffontencoding).

**Remarks**

القيمة الافتراضية هي [PdfFontEncoding.IDENTITY](../../com.aspose.cells/pdffontencoding\#IDENTITY)

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setFontSubstitutionCharGranularity(boolean value) {#setFontSubstitutionCharGranularity-boolean-}
```
public void setFontSubstitutionCharGranularity(boolean value)
```


يشير إلى ما إذا كان يجب استبدال خط الحرف فقط عندما يكون خط الخلية غير متوافق معه.

**Remarks**

القيمة الافتراضية هي false. سنحاول أولاً الخط الافتراضي لملف Workbook وPdfSaveOption/system لخط الخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setGridlineColor(Color value) {#setGridlineColor-com.aspose.cells.Color-}
```
public void setGridlineColor(Color value)
```


يضبط لون خطوط الشبكة.

**Remarks**

سيتجاهل إعدادات لون خطوط الشبكة في ملف المصدر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setGridlineType(int value) {#setGridlineType-int-}
```
public void setGridlineType(int value)
```


يضبط نوع خطوط الشبكة.

انظر [GridlineType](../../com.aspose.cells/gridlinetype).

**Remarks**

القيمة الافتراضية هي النوع المنقط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setIgnoreError(boolean value) {#setIgnoreError-boolean-}
```
public void setIgnoreError(boolean value)
```


يشير إلى ما إذا كنت بحاجة إلى إخفاء الخطأ أثناء التصيير. قد يكون الخطأ في الشكل أو الصورة أو تصيير المخطط، إلخ.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setImageResample(int desiredPPI, int jpegQuality) {#setImageResample-int-int-}
```
public void setImageResample(int desiredPPI, int jpegQuality)
```


يضبط قيمة PPI (بكسل لكل بوصة) المطلوبة لإعادة تحجيم الصور وجودة JPEG. سيتم تحويل جميع الصور إلى JPEG بالإعداد المحدد للجودة، وستتم إعادة تحجيم الصور التي تتجاوز قيمة PPI المحددة.

**Example**

الكود التالي يضبط قيمة PPI المطلوبة كـ 96 وجودة JPEG كـ 80 للصور في ملف PDF الناتج.

```
         //load the source file with images.
         Workbook wb = new Workbook("Book1.xlsx");
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
 
         //set desired PPI as 96 and jpeg quality as 80.
         pdfSaveOptions.setImageResample(96, 80);
 
         wb.save("output.pdf", pdfSaveOptions);
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| desiredPPI | int | البكسلات المطلوبة لكل بوصة. 220 جودة عالية. 150 جودة الشاشة. 96 جودة البريد الإلكتروني. |
| jpegQuality | int | 0 - 100٪ جودة JPEG. |

### setImageType(ImageFormat value) {#setImageType-com.aspose.cells.ImageFormat-}
```
public void setImageType(ImageFormat value)
```


يمثل نوع الصورة عند تحويل المخطط والشكل.

**Remarks**

NOTE: هذا العضو الآن مهمل. بدلاً من ذلك، يتم دائمًا عرض **Chart** و **Shape** كعناصر متجهية (مثل النقطة، الخط) لتحسين جودة العرض. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [ImageFormat](../../com.aspose.cells/imageformat) |  |

### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```


يحدد ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق قبل حفظ الملف.

**Remarks**

القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setOnePagePerSheet(boolean value) {#setOnePagePerSheet-boolean-}
```
public void setOnePagePerSheet(boolean value)
```


إذا كان OnePagePerSheet صحيحًا، فسيتم إخراج كل محتوى ورقة واحدة إلى صفحة واحدة فقط في النتيجة. سيكون حجم الورق في pagesetup غير صالح، وستظل الإعدادات الأخرى لـ pagesetup سارية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setOptimizationType(int value) {#setOptimizationType-int-}
```
public void setOptimizationType(int value)
```


يضبط نوع تحسين PDF.

انظر [PdfOptimizationType](../../com.aspose.cells/pdfoptimizationtype).

**Remarks**

القيمة الافتراضية هي [PdfOptimizationType.STANDARD](../../com.aspose.cells/pdfoptimizationtype\#STANDARD)

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setOutputBlankPageWhenNothingToPrint(boolean value) {#setOutputBlankPageWhenNothingToPrint-boolean-}
```
public void setOutputBlankPageWhenNothingToPrint(boolean value)
```


يشير إلى ما إذا كان يجب إخراج صفحة فارغة عندما لا يوجد شيء للطباعة.

**Remarks**

القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setPageCount(int value) {#setPageCount-int-}
```
public void setPageCount(int value)
```


يضبط عدد الصفحات التي سيتم حفظها.

**Remarks**

القيمة الافتراضية هي System.Int32.MaxValue مما يعني أنه سيتم عرض جميع الصفحات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPageIndex(int value) {#setPageIndex-int-}
```
public void setPageIndex(int value)
```


يضبط الفهرس القائم على الصفر للصفحة الأولى التي سيتم حفظها.

**Remarks**

القيمة الافتراضية هي 0.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-}
```
public void setPageSavingCallback(IPageSavingCallback value)
```


التحكم/الإشارة إلى تقدم عملية حفظ الصفحة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback) |  |

### setPdfCompression(int value) {#setPdfCompression-int-}
```
public void setPdfCompression(int value)
```


حدد خوارزمية الضغط

انظر [PdfCompressionCore](../../com.aspose.cells/pdfcompressioncore).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPrintingPageType(int value) {#setPrintingPageType-int-}
```
public void setPrintingPageType(int value)
```


يشير إلى الصفحات التي لن تُطبع.

انظر [PrintingPageType](../../com.aspose.cells/printingpagetype).

**Remarks**

إذا كان المحتوى في الورقة متفرقًا، فستظهر بعض الصفحات فارغة تمامًا في ملف PDF الناتج. إذا كنت لا تريد هذه الصفحات الفارغة، يمكنك استخدام هذا الخيار لتخطيها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setProducer(String value) {#setProducer-java.lang.String-}
```
public void setProducer(String value)
```


يضبط المنتج للمستند PDF المُنشأ.

**Remarks**

إذا كانت القيمة null، أو لم يتم تعيين LICENSE صالح، سيتم استخدام السلسلة Aspose.Cells vVERSION.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


يحدد ما إذا كان يتم تخزين أحدث بيانات المخطط مؤقتًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setRenderingBehavior(int value) {#setRenderingBehavior-int-}
```
public void setRenderingBehavior(int value)
```


يضبط سلوكيات التصيير الخاصة بـ Excel لتطبيقها.

انظر [ExcelRenderingBehavior](../../com.aspose.cells/excelrenderingbehavior).

**Remarks**

القيمة الافتراضية هي [ExcelRenderingBehavior.ALL](../../com.aspose.cells/excelrenderingbehavior\#ALL).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setSecurityOptions(PdfSecurityOptions value) {#setSecurityOptions-com.aspose.cells.PdfSecurityOptions-}
```
public void setSecurityOptions(PdfSecurityOptions value)
```


قم بتعيين هذه الخيارات عندما تكون الأمان مطلوبًا في نتيجة xls2pdf.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [PdfSecurityOptions](../../com.aspose.cells/pdfsecurityoptions) |  |

### setSheetSet(SheetSet value) {#setSheetSet-com.aspose.cells.SheetSet-}
```
public void setSheetSet(SheetSet value)
```


يضبط الأوراق التي سيتم عرضها. القيمة الافتراضية هي جميع الأوراق المرئية في المصنف: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [SheetSet](../../com.aspose.cells/sheetset) |  |

### setSortExternalNames(boolean value) {#setSortExternalNames-boolean-}
```
public void setSortExternalNames(boolean value)
```


يحدد ما إذا كان يتم فرز الأسماء المعرفة الخارجية قبل حفظ الملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSortNames(boolean value) {#setSortNames-boolean-}
```
public void setSortNames(boolean value)
```


يحدد ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setTextCrossType(int value) {#setTextCrossType-int-}
```
public void setTextCrossType(int value)
```


يضبط نوع عرض النص عندما يكون عرض النص أكبر من عرض الخلية.

انظر [TextCrossType](../../com.aspose.cells/textcrosstype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setUpdateSmartArt(boolean value) {#setUpdateSmartArt-boolean-}
```
public void setUpdateSmartArt(boolean value)
```


يشير إلى ما إذا كان يتم تحديث إعدادات Smart Art. القيمة الافتراضية هي false.

**Remarks**

يؤثر فقط بعد استدعاء الطريقة Shape.GetResultOfSmartArt() ووجود الأشكال المخزنة مؤقتًا في ملف القالب.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```


يحدد ما إذا كان يتم التحقق من صحة الخلايا المدمجة قبل حفظ الملف.

**Remarks**

القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```


يضبط رد النداء للتحذير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

### setWatermark(RenderingWatermark value) {#setWatermark-com.aspose.cells.RenderingWatermark-}
```
public void setWatermark(RenderingWatermark value)
```


يضبط العلامة المائية للإخراج.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [RenderingWatermark](../../com.aspose.cells/renderingwatermark) |  |

### setZoomBehavior(int value) {#setZoomBehavior-int-}
```
public void setZoomBehavior(int value)
```


يضبط وضع العرض الأولي عند فتح مستند PDF المُولد. القيمة الافتراضية هي [PdfZoomBehavior.NONE](../../com.aspose.cells/pdfzoombehavior\#NONE).

انظر [PdfZoomBehavior](../../com.aspose.cells/pdfzoombehavior).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setZoomFactor(int value) {#setZoomFactor-int-}
```
public void setZoomFactor(int value)
```


يضبط نسبة التكبير المستخدمة عندما يكون [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\#getZoomBehavior--) هو [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\#ZOOM-FACTOR).

**Remarks**

يتم تجاهل هذه الخاصية ما لم يكن [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\#getZoomBehavior--) هو [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\#ZOOM-FACTOR).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

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

