---
title: "HtmlSaveOptions"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل الخيارات لحفظ ملف html."
type: docs
url: /ar/java/com.aspose.cells/htmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class HtmlSaveOptions extends SaveOptions
```

يمثل الخيارات لحفظ ملف html.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [HtmlSaveOptions()](#HtmlSaveOptions--) | ينشئ خيارات لحفظ ملف html. |
| [HtmlSaveOptions(int saveFormat)](#HtmlSaveOptions-int-) | ينشئ خيارات لحفظ ملف htm. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAddGenericFont()](#getAddGenericFont--) | يحدد ما إذا كان سيتم إضافة خط عام إلى خاصية CSS font-family. |
| [getAddTooltipText()](#getAddTooltipText--) | يحدد ما إذا كان سيتم إضافة نص تلميح عندما لا يمكن عرض البيانات بالكامل. |
| [getAttachedFilesDirectory()](#getAttachedFilesDirectory--) | الدليل الذي سيتم حفظ الملفات المرفقة فيه. |
| [getAttachedFilesUrlPrefix()](#getAttachedFilesUrlPrefix--) | حدد بادئة URL للملفات المرفقة مثل الصورة في ملف HTML. |
| [getCachedFileFolder()](#getCachedFileFolder--) | المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة تخزين مؤقت للبيانات. |
| [getCalculateFormula()](#getCalculateFormula--) | يحدد ما إذا كان سيتم حساب الصيغ قبل حفظ ملف HTML. |
| [getCellCssPrefix()](#getCellCssPrefix--) | يحصل على بادئة اسم CSS، القيمة الافتراضية هي "". |
| [getCellNameAttribute()](#getCellNameAttribute--) | يحدد السمة التي تشير إلى اسم الخلية (CellName) التي سيتم كتابتها. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المرتبطة بالخلايا. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | اجعل دفتر العمل فارغًا بعد حفظ الملف. |
| [getCreateDirectory()](#getCreateDirectory--) | إذا كان صحيحًا ولم يكن الدليل موجودًا، فسيتم إنشاء الدليل تلقائيًا قبل حفظ الملف. |
| [getCssStyles()](#getCssStyles--) | يحصل على أنماط CSS الإضافية للمنسق. |
| [getDataBarRenderMode()](#getDataBarRenderMode--) | يمثل وضع كيفية عرض DataBar عند تحويل ملفات Excel إلى ملفات HTML. |
| [getDefaultFontName()](#getDefaultFontName--) | حدد اسم الخط الافتراضي لتصدير HTML، سيتم استخدام الخط الافتراضي عندما لا يكون خط النمط موجودًا، إذا كانت هذه الخاصية فارغة (null)، سيستخدم Aspose.Cells خطًا عالميًا يملك نفس عائلة الخط الأصلي، القيمة الافتراضية هي null. |
| [getDisableCss()](#getDisableCss--) | يحدد ما إذا كانت الأنماط المضمنة فقط هي المطبقة، دون الاعتماد على CSS. |
| [getDisableDownlevelRevealedComments()](#getDisableDownlevelRevealedComments--) | يحدد ما إذا كان يتم تعطيل التعليقات الشرطية Downlevel-revealed عند تصدير الملف إلى HTML، القيمة الافتراضية هي false. |
| [getEmbeddedFontType()](#getEmbeddedFontType--) | يحصل على نوع تضمين ملف الخط في ملف HTML. |
| [getEnableCssCustomProperties()](#getEnableCssCustomProperties--) | تحسين مخرجات HTML باستخدام خصائص CSS المخصصة. |
| [getEncodeEntityAsCode()](#getEncodeEntityAsCode--) | يحدد ما إذا كانت كيانات الأحرف في HTML تُستبدل بالرموز العشرية. |
| [getEncoding()](#getEncoding--) | إذا لم يتم تحديده، استخدم Encoding.UTF8 كنمط الترميز الافتراضي. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | يحدد ما إذا كان يتم تشفير خصائص المستند عند الحفظ كملف .xls. |
| [getExcludeUnusedStyles()](#getExcludeUnusedStyles--) | يحدد ما إذا كان يتم استبعاد الأنماط غير المستخدمة. |
| [getExportActiveWorksheetOnly()](#getExportActiveWorksheetOnly--) | يحدد ما إذا كان يتم تصدير ورقة العمل النشطة فقط إلى ملف HTML. |
| [getExportArea()](#getExportArea--) | يحصل على نطاق الخلايا (CellArea) المُصدَّر للورقة النشطة الحالية. |
| [getExportBogusRowData()](#getExportBogusRowData--) | يحدد ما إذا كان يتم تصدير بيانات الصف السفلي الزائف. |
| [getExportCellCoordinate()](#getExportCellCoordinate--) | يحدد ما إذا كان يتم تصدير إحداثيات Excel للخلايا غير الفارغة عند حفظ الملف إلى HTML. |
| [getExportCommentsType()](#getExportCommentsType--) | يمثل نوع تصدير التعليقات إلى ملفات HTML. |
| [getExportDataOptions()](#getExportDataOptions--) | يحدد قاعدة تصدير بيانات ملف HTML. القيمة الافتراضية هي All. |
| [getExportDocumentProperties()](#getExportDocumentProperties--) | يحدد ما إذا كان يتم تصدير خصائص المستند. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف HTML أو MHT إلى Excel، يرجى الحفاظ على القيمة الافتراضية. |
| [getExportExtraHeadings()](#getExportExtraHeadings--) | يحدد ما إذا كان يتم تصدير عناوين إضافية عندما يكون طول النص أطول من الحد الأقصى للعمود المعروض. |
| [getExportFormula()](#getExportFormula--) | يحدد ما إذا كان يتم تصدير الصيغ عند حفظ الملف إلى HTML. |
| [getExportFrameScriptsAndProperties()](#getExportFrameScriptsAndProperties--) | الإشارة إلى ما إذا كان يتم تصدير سكريبتات الإطار وخصائص المستند. |
| [getExportGridLines()](#getExportGridLines--) | الإشارة إلى ما إذا كان يتم تصدير خطوط الشبكة. القيمة الافتراضية هي false. |
| [getExportHeadings()](#getExportHeadings--) | يحدد ما إذا كان يتم تصدير عناوين الصفوف والأعمدة للورقة عند الحفظ كملفات HTML. |
| [getExportHiddenWorksheet()](#getExportHiddenWorksheet--) | الإشارة إلى ما إذا كان يتم تصدير محتوى ورقة العمل المخفي. القيمة الافتراضية هي true. |
| [getExportImagesAsBase64()](#getExportImagesAsBase64--) | يحدد ما إذا كانت الصور تُحفظ بتنسيق Base64 إلى HTML أو MHTML أو EPUB. |
| [getExportNamedRangeAnchors()](#getExportNamedRangeAnchors--) | يحدد ما إذا كان يتم تصدير عناصر الربط للنطاقات المسماة عند الحفظ كـ HTML. |
| [getExportObjectListener()](#getExportObjectListener--) | يحصل على ExportObjectListener لتصدير الكائنات. |
| [getExportPageFooters()](#getExportPageFooters--) | يحدد ما إذا كان يتم تصدير رؤوس الصفحات. |
| [getExportPageHeaders()](#getExportPageHeaders--) | يحدد ما إذا كان يتم تصدير رؤوس الصفحات. |
| [getExportPrintAreaOnly()](#getExportPrintAreaOnly--) | يحدد ما إذا كان يتم تصدير منطقة الطباعة فقط إلى ملف HTML. |
| [getExportRowColumnHeadings()](#getExportRowColumnHeadings--) | يحدد ما إذا كان يتم تصدير عناوين الصفوف والأعمدة للورقة عند الحفظ كملفات HTML. |
| [getExportSimilarBorderStyle()](#getExportSimilarBorderStyle--) | الإشارة إلى ما إذا كان يتم تصدير نمط الحدود المشابه عندما لا يدعم المتصفحات نمط الحدود. |
| [getExportSingleTab()](#getExportSingleTab--) | يحدد ما إذا كان يتم تصدير علامة التبويب الوحيدة عندما يحتوي الملف على ورقة عمل واحدة فقط. |
| [getExportWorkbookProperties()](#getExportWorkbookProperties--) | الإشارة إلى ما إذا كان يتم تصدير خصائص المصنف. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html أو mht إلى Excel، يرجى الحفاظ على القيمة الافتراضية. |
| [getExportWorksheetCSSSeparately()](#getExportWorksheetCSSSeparately--) | الإشارة إلى ما إذا كان يتم تصدير CSS لورقة العمل بشكل منفصل. القيمة الافتراضية هي false. |
| [getExportWorksheetProperties()](#getExportWorksheetProperties--) | الإشارة إلى ما إذا كان يتم تصدير خصائص ورقة العمل. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html أو mht إلى Excel، يرجى الحفاظ على القيمة الافتراضية. |
| [getFilePathProvider()](#getFilePathProvider--) | يحصل على IFilePathProvider لتصدير ورقة العمل إلى HTML بشكل منفصل. |
| [getFormatDataIgnoreColumnWidth()](#getFormatDataIgnoreColumnWidth--) | الإشارة إلى ما إذا كان يتم عرض كامل البيانات المنسقة للخلية عند تجاوز العمود. |
| [getHiddenColDisplayType()](#getHiddenColDisplayType--) | العمود المخفي (عرض هذا العمود هو 0) في Excel، قبل حفظه بصيغة HTML، إذا كان HtmlHiddenColDisplayType هو "Remove"، فلن يتم إخراج العمود المخفي، إذا كانت القيمة "Hidden"، سيتم إخراج العمود لكنه سيظل مخفيًا، القيمة الافتراضية هي "Hidden". |
| [getHiddenRowDisplayType()](#getHiddenRowDisplayType--) | الصف المخفي (ارتفاع هذا الصف هو 0) في Excel، قبل حفظه بصيغة HTML، إذا كان HtmlHiddenRowDisplayType هو "Remove"، فلن يتم إخراج الصف المخفي، إذا كانت القيمة "Hidden"، سيتم إخراج الصف لكنه سيظل مخفيًا، القيمة الافتراضية هي "Hidden". |
| [getHideOverflowWrappedText()](#getHideOverflowWrappedText--) | يحدد ما إذا كان يتم إخفاء النص المتجاوز عندما يكون تنسيق الخلية مضبوطًا على التفاف النص. |
| [getHtmlCrossStringType()](#getHtmlCrossStringType--) | يحدد ما إذا كان سيتم عرض سلسلة عبر خلايا بنفس طريقة MS Excel عند حفظ ملف Excel بصيغة HTML. |
| [getHtmlVersion()](#getHtmlVersion--) | يحدد إصدار معيار HTML الذي يجب استخدامه عند حفظ الصيغة HTML. |
| [getIgnoreInvisibleShapes()](#getIgnoreInvisibleShapes--) | الإشارة إلى ما إذا كان يتم تصدير الأشكال غير المرئية. |
| [getImageOptions()](#getImageOptions--) | احصل على كائن ImageOrPrintOptions قبل التصدير. |
| [getImageScalable()](#getImageScalable--) | يحدد ما إذا كان يتم استخدام وحدة قابلة للتوسع لوصف عرض الصورة عند استخدام وحدة قابلة للتوسع لوصف عرض العمود. |
| [getLayoutMode()](#getLayoutMode--) | يحصل على وضع التخطيط عند الحفظ كـ HTML. |
| [getLinkTargetType()](#getLinkTargetType--) | الإشارة إلى نوع السمة المستهدفة في رابط `<a>`. |
| [getMergeAreas()](#getMergeAreas--) | يحدد ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق قبل حفظ الملف. |
| [getMergeEmptyTdForcely()](#getMergeEmptyTdForcely--) | يحدد ما إذا كان يتم دمج عنصر TD الفارغ قسريًا عند تصدير الملف إلى HTML. |
| [getMergeEmptyTdType()](#getMergeEmptyTdType--) | الخيار لدمج الخلايا الفارغة المتجاورة (عناصر td الفارغة). القيمة الافتراضية هي MergeEmptyTdType.Default. |
| [getOfficeMathOutputMode()](#getOfficeMathOutputMode--) | يحدد كيفية تصدير كائنات OfficeMath إلى HTML، القيمة الافتراضية هي Image. |
| [getPageTitle()](#getPageTitle--) | عنوان صفحة HTML. |
| [getParseHtmlTagInCell()](#getParseHtmlTagInCell--) | يحدد ما إذا كان يجب تحليل علامة HTML (مثل `<div></div>`) في الخلية كقيمة خلية أم الحفاظ عليها كما هي. |
| [getPresentationPreference()](#getPresentationPreference--) | الإشارة إلى ما إذا كان ملف HTML أو MHT هو تفضيل العرض. |
| [getRefreshChartCache()](#getRefreshChartCache--) | يحدد ما إذا كان يتم تخزين أحدث بيانات المخطط مؤقتًا. |
| [getSaveAsSingleFile()](#getSaveAsSingleFile--) | يحدد ما إذا كان يتم حفظ HTML كملف واحد. |
| [getSaveFormat()](#getSaveFormat--) | يحصل على صيغة حفظ الملف. |
| [getSheetSet()](#getSheetSet--) | يحصل على الأوراق التي سيتم عرضها. |
| [getShowAllSheets()](#getShowAllSheets--) | يحدد ما إذا كان يتم عرض جميع الأوراق عند حفظها كملف HTML واحد. |
| [getSortExternalNames()](#getSortExternalNames--) | يحدد ما إذا كان يتم فرز الأسماء المعرفة الخارجية قبل حفظ الملف. |
| [getSortNames()](#getSortNames--) | يحدد ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف. |
| [getSpaceMode()](#getSpaceMode--) | يحدد كيفية عرض المسافات في مخرجات HTML. |
| [getStreamProvider()](#getStreamProvider--) | يحصل على IStreamProvider لتصدير الكائنات. |
| [getTableCssId()](#getTableCssId--) | يحصل على بادئة اسم CSS للنوع مثل tr و col و td وما إلى ذلك، وهي موجودة في عنصر الجدول الذي يحتوي على السمة TableCssId المحددة. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | يحدد ما إذا كان يتم تحديث إعدادات Smart Art. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | يحدد ما إذا كان يتم التحقق من صحة الخلايا المدمجة قبل حفظ الملف. |
| [getWarningCallback()](#getWarningCallback--) | يحصل على رد النداء للتحذير. |
| [getWidthScalable()](#getWidthScalable--) | يحدد ما إذا كان يتم تصدير عرض العمود بوحدة المقياس إلى HTML. |
| [getWorksheetScalable()](#getWorksheetScalable--) | يحدد ما إذا كان يتم تكبير أو تصغير HTML عبر مستوى تكبير ورقة العمل عند حفظ الملف إلى HTML، القيمة الافتراضية هي false. |
| [hashCode()](#hashCode--) |  |
| [isBorderCollapsed()](#isBorderCollapsed--) | يحدد ما إذا كانت حدود الجدول مدمجة. |
| [isExpImageToTempDir()](#isExpImageToTempDir--) | يحدد ما إذا كان يتم تصدير ملفات الصور إلى الدليل المؤقت. |
| [isExportComments()](#isExportComments--) | يحدد ما إذا كان يتم تصدير التعليقات عند حفظ الملف إلى HTML، القيمة الافتراضية هي false. |
| [isFullPathLink()](#isFullPathLink--) | الإشارة إلى ما إذا كان يتم استخدام رابط المسار الكامل في sheet00x.htm و filelist.xml و tabstrip.htm. |
| [isIECompatible()](#isIECompatible--) | الإشارة إلى ما إذا كان HTML الناتج متوافقًا مع متصفح IE. |
| [isJsBrowserCompatible()](#isJsBrowserCompatible--) | يحدد ما إذا كان JavaScript متوافقًا مع المتصفحات التي لا تدعم JavaScript. |
| [isMobileCompatible()](#isMobileCompatible--) | يحدد ما إذا كان HTML الناتج متوافقًا مع الأجهزة المحمولة. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAddGenericFont(boolean value)](#setAddGenericFont-boolean-) | يحدد ما إذا كان سيتم إضافة خط عام إلى خاصية CSS font-family. |
| [setAddTooltipText(boolean value)](#setAddTooltipText-boolean-) | يحدد ما إذا كان سيتم إضافة نص تلميح عندما لا يمكن عرض البيانات بالكامل. |
| [setAttachedFilesDirectory(String value)](#setAttachedFilesDirectory-java.lang.String-) | الدليل الذي سيتم حفظ الملفات المرفقة فيه. |
| [setAttachedFilesUrlPrefix(String value)](#setAttachedFilesUrlPrefix-java.lang.String-) | حدد بادئة URL للملفات المرفقة مثل الصورة في ملف HTML. |
| [setBorderCollapsed(boolean value)](#setBorderCollapsed-boolean-) | يحدد ما إذا كانت حدود الجدول مدمجة. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة تخزين مؤقت للبيانات. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | يحدد ما إذا كان سيتم حساب الصيغ قبل حفظ ملف HTML. |
| [setCellCssPrefix(String value)](#setCellCssPrefix-java.lang.String-) | يضبط بادئة اسم CSS، القيمة الافتراضية هي \"\". |
| [setCellNameAttribute(String value)](#setCellNameAttribute-java.lang.String-) | يحدد السمة التي تشير إلى اسم الخلية (CellName) التي سيتم كتابتها. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المرتبطة بالخلايا. |
| [setClearData(boolean value)](#setClearData-boolean-) | اجعل دفتر العمل فارغًا بعد حفظ الملف. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | إذا كان صحيحًا ولم يكن الدليل موجودًا، فسيتم إنشاء الدليل تلقائيًا قبل حفظ الملف. |
| [setCssStyles(String value)](#setCssStyles-java.lang.String-) | يضبط أنماط CSS الإضافية للمنسق. |
| [setDataBarRenderMode(int value)](#setDataBarRenderMode-int-) | يمثل وضع كيفية عرض DataBar عند تحويل ملفات Excel إلى ملفات HTML. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | حدد اسم الخط الافتراضي لتصدير HTML، سيتم استخدام الخط الافتراضي عندما لا يكون خط النمط موجودًا، إذا كانت هذه الخاصية فارغة (null)، سيستخدم Aspose.Cells خطًا عالميًا يملك نفس عائلة الخط الأصلي، القيمة الافتراضية هي null. |
| [setDisableCss(boolean value)](#setDisableCss-boolean-) | يحدد ما إذا كانت الأنماط المضمنة فقط هي المطبقة، دون الاعتماد على CSS. |
| [setDisableDownlevelRevealedComments(boolean value)](#setDisableDownlevelRevealedComments-boolean-) | يحدد ما إذا كان يتم تعطيل التعليقات الشرطية Downlevel-revealed عند تصدير الملف إلى HTML، القيمة الافتراضية هي false. |
| [setEmbeddedFontType(int value)](#setEmbeddedFontType-int-) | يضبط نوع تضمين ملف الخط داخل ملف HTML. |
| [setEnableCssCustomProperties(boolean value)](#setEnableCssCustomProperties-boolean-) | تحسين مخرجات HTML باستخدام خصائص CSS المخصصة. |
| [setEncodeEntityAsCode(boolean value)](#setEncodeEntityAsCode-boolean-) | يحدد ما إذا كانت كيانات الأحرف في HTML تُستبدل بالرموز العشرية. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | إذا لم يتم تحديده، استخدم Encoding.UTF8 كنمط الترميز الافتراضي. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | يحدد ما إذا كان يتم تشفير خصائص المستند عند الحفظ كملف .xls. |
| [setExcludeUnusedStyles(boolean value)](#setExcludeUnusedStyles-boolean-) | يحدد ما إذا كان يتم استبعاد الأنماط غير المستخدمة. |
| [setExpImageToTempDir(boolean value)](#setExpImageToTempDir-boolean-) | يحدد ما إذا كان يتم تصدير ملفات الصور إلى الدليل المؤقت. |
| [setExportActiveWorksheetOnly(boolean value)](#setExportActiveWorksheetOnly-boolean-) | يحدد ما إذا كان يتم تصدير ورقة العمل النشطة فقط إلى ملف HTML. |
| [setExportArea(CellArea value)](#setExportArea-com.aspose.cells.CellArea-) | يضبط نطاق CellArea المُصدّر للورقة النشطة الحالية. |
| [setExportBogusRowData(boolean value)](#setExportBogusRowData-boolean-) | يحدد ما إذا كان يتم تصدير بيانات الصف السفلي الزائف. |
| [setExportCellCoordinate(boolean value)](#setExportCellCoordinate-boolean-) | يحدد ما إذا كان يتم تصدير إحداثيات Excel للخلايا غير الفارغة عند حفظ الملف إلى HTML. |
| [setExportComments(boolean value)](#setExportComments-boolean-) | يحدد ما إذا كان يتم تصدير التعليقات عند حفظ الملف إلى HTML، القيمة الافتراضية هي false. |
| [setExportCommentsType(int value)](#setExportCommentsType-int-) | يمثل نوع تصدير التعليقات إلى ملفات HTML. |
| [setExportDataOptions(int value)](#setExportDataOptions-int-) | يحدد قاعدة تصدير بيانات ملف HTML. القيمة الافتراضية هي All. |
| [setExportDocumentProperties(boolean value)](#setExportDocumentProperties-boolean-) | يحدد ما إذا كان يتم تصدير خصائص المستند. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف HTML أو MHT إلى Excel، يرجى الحفاظ على القيمة الافتراضية. |
| [setExportExtraHeadings(boolean value)](#setExportExtraHeadings-boolean-) | يحدد ما إذا كان يتم تصدير عناوين إضافية عندما يكون طول النص أطول من الحد الأقصى للعمود المعروض. |
| [setExportFormula(boolean value)](#setExportFormula-boolean-) | يحدد ما إذا كان يتم تصدير الصيغ عند حفظ الملف إلى HTML. |
| [setExportFrameScriptsAndProperties(boolean value)](#setExportFrameScriptsAndProperties-boolean-) | الإشارة إلى ما إذا كان يتم تصدير سكريبتات الإطار وخصائص المستند. |
| [setExportGridLines(boolean value)](#setExportGridLines-boolean-) | الإشارة إلى ما إذا كان يتم تصدير خطوط الشبكة. القيمة الافتراضية هي false. |
| [setExportHeadings(boolean value)](#setExportHeadings-boolean-) | يحدد ما إذا كان يتم تصدير عناوين الصفوف والأعمدة للورقة عند الحفظ كملفات HTML. |
| [setExportHiddenWorksheet(boolean value)](#setExportHiddenWorksheet-boolean-) | الإشارة إلى ما إذا كان يتم تصدير محتوى ورقة العمل المخفي. القيمة الافتراضية هي true. |
| [setExportImagesAsBase64(boolean value)](#setExportImagesAsBase64-boolean-) | يحدد ما إذا كانت الصور تُحفظ بتنسيق Base64 إلى HTML أو MHTML أو EPUB. |
| [setExportNamedRangeAnchors(boolean value)](#setExportNamedRangeAnchors-boolean-) | يحدد ما إذا كان يتم تصدير عناصر الربط للنطاقات المسماة عند الحفظ كـ HTML. |
| [setExportObjectListener(IExportObjectListener value)](#setExportObjectListener-com.aspose.cells.IExportObjectListener-) | يضبط ExportObjectListener لتصدير الكائنات. |
| [setExportPageFooters(boolean value)](#setExportPageFooters-boolean-) | يحدد ما إذا كان يتم تصدير رؤوس الصفحات. |
| [setExportPageHeaders(boolean value)](#setExportPageHeaders-boolean-) | يحدد ما إذا كان يتم تصدير رؤوس الصفحات. |
| [setExportPrintAreaOnly(boolean value)](#setExportPrintAreaOnly-boolean-) | يحدد ما إذا كان يتم تصدير منطقة الطباعة فقط إلى ملف HTML. |
| [setExportRowColumnHeadings(boolean value)](#setExportRowColumnHeadings-boolean-) | يحدد ما إذا كان يتم تصدير عناوين الصفوف والأعمدة للورقة عند الحفظ كملفات HTML. |
| [setExportSimilarBorderStyle(boolean value)](#setExportSimilarBorderStyle-boolean-) | الإشارة إلى ما إذا كان يتم تصدير نمط الحدود المشابه عندما لا يدعم المتصفحات نمط الحدود. |
| [setExportSingleTab(boolean value)](#setExportSingleTab-boolean-) | يحدد ما إذا كان يتم تصدير علامة التبويب الوحيدة عندما يحتوي الملف على ورقة عمل واحدة فقط. |
| [setExportWorkbookProperties(boolean value)](#setExportWorkbookProperties-boolean-) | الإشارة إلى ما إذا كان يتم تصدير خصائص المصنف. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html أو mht إلى Excel، يرجى الحفاظ على القيمة الافتراضية. |
| [setExportWorksheetCSSSeparately(boolean value)](#setExportWorksheetCSSSeparately-boolean-) | الإشارة إلى ما إذا كان يتم تصدير CSS لورقة العمل بشكل منفصل. القيمة الافتراضية هي false. |
| [setExportWorksheetProperties(boolean value)](#setExportWorksheetProperties-boolean-) | الإشارة إلى ما إذا كان يتم تصدير خصائص ورقة العمل. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html أو mht إلى Excel، يرجى الحفاظ على القيمة الافتراضية. |
| [setFilePathProvider(IFilePathProvider value)](#setFilePathProvider-com.aspose.cells.IFilePathProvider-) | يضبط IFilePathProvider لتصدير Worksheet إلى HTML بشكل منفصل. |
| [setFormatDataIgnoreColumnWidth(boolean value)](#setFormatDataIgnoreColumnWidth-boolean-) | الإشارة إلى ما إذا كان يتم عرض كامل البيانات المنسقة للخلية عند تجاوز العمود. |
| [setFullPathLink(boolean value)](#setFullPathLink-boolean-) | الإشارة إلى ما إذا كان يتم استخدام رابط المسار الكامل في sheet00x.htm و filelist.xml و tabstrip.htm. |
| [setHiddenColDisplayType(int value)](#setHiddenColDisplayType-int-) | العمود المخفي (عرض هذا العمود هو 0) في Excel، قبل حفظه بصيغة HTML، إذا كان HtmlHiddenColDisplayType هو "Remove"، فلن يتم إخراج العمود المخفي، إذا كانت القيمة "Hidden"، سيتم إخراج العمود لكنه سيظل مخفيًا، القيمة الافتراضية هي "Hidden". |
| [setHiddenRowDisplayType(int value)](#setHiddenRowDisplayType-int-) | الصف المخفي (ارتفاع هذا الصف هو 0) في Excel، قبل حفظه بصيغة HTML، إذا كان HtmlHiddenRowDisplayType هو "Remove"، فلن يتم إخراج الصف المخفي، إذا كانت القيمة "Hidden"، سيتم إخراج الصف لكنه سيظل مخفيًا، القيمة الافتراضية هي "Hidden". |
| [setHideOverflowWrappedText(boolean value)](#setHideOverflowWrappedText-boolean-) | يحدد ما إذا كان يتم إخفاء النص المتجاوز عندما يكون تنسيق الخلية مضبوطًا على التفاف النص. |
| [setHtmlCrossStringType(int value)](#setHtmlCrossStringType-int-) | يحدد ما إذا كان سيتم عرض سلسلة عبر خلايا بنفس طريقة MS Excel عند حفظ ملف Excel بصيغة HTML. |
| [setHtmlVersion(int value)](#setHtmlVersion-int-) | يحدد إصدار معيار HTML الذي يجب استخدامه عند حفظ الصيغة HTML. |
| [setIECompatible(boolean value)](#setIECompatible-boolean-) | الإشارة إلى ما إذا كان HTML الناتج متوافقًا مع متصفح IE. |
| [setIgnoreInvisibleShapes(boolean value)](#setIgnoreInvisibleShapes-boolean-) | الإشارة إلى ما إذا كان يتم تصدير الأشكال غير المرئية. |
| [setImageScalable(boolean value)](#setImageScalable-boolean-) | يحدد ما إذا كان يتم استخدام وحدة قابلة للتوسع لوصف عرض الصورة عند استخدام وحدة قابلة للتوسع لوصف عرض العمود. |
| [setJsBrowserCompatible(boolean value)](#setJsBrowserCompatible-boolean-) | يحدد ما إذا كان JavaScript متوافقًا مع المتصفحات التي لا تدعم JavaScript. |
| [setLayoutMode(int value)](#setLayoutMode-int-) | يضبط وضع التخطيط عند الحفظ إلى HTML. |
| [setLinkTargetType(int value)](#setLinkTargetType-int-) | الإشارة إلى نوع السمة المستهدفة في رابط `<a>`. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | يحدد ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق قبل حفظ الملف. |
| [setMergeEmptyTdForcely(boolean value)](#setMergeEmptyTdForcely-boolean-) | يحدد ما إذا كان يتم دمج عنصر TD الفارغ قسريًا عند تصدير الملف إلى HTML. |
| [setMergeEmptyTdType(int value)](#setMergeEmptyTdType-int-) | الخيار لدمج الخلايا الفارغة المتجاورة (عناصر td الفارغة). القيمة الافتراضية هي MergeEmptyTdType.Default. |
| [setMobileCompatible(boolean value)](#setMobileCompatible-boolean-) | يحدد ما إذا كان HTML الناتج متوافقًا مع الأجهزة المحمولة. |
| [setOfficeMathOutputMode(int value)](#setOfficeMathOutputMode-int-) | يحدد كيفية تصدير كائنات OfficeMath إلى HTML، القيمة الافتراضية هي Image. |
| [setPageTitle(String value)](#setPageTitle-java.lang.String-) | عنوان صفحة HTML. |
| [setParseHtmlTagInCell(boolean value)](#setParseHtmlTagInCell-boolean-) | يحدد ما إذا كان يجب تحليل علامة HTML (مثل `<div></div>`) في الخلية كقيمة خلية أم الحفاظ عليها كما هي. |
| [setPresentationPreference(boolean value)](#setPresentationPreference-boolean-) | الإشارة إلى ما إذا كان ملف HTML أو MHT هو تفضيل العرض. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | يحدد ما إذا كان يتم تخزين أحدث بيانات المخطط مؤقتًا. |
| [setSaveAsSingleFile(boolean value)](#setSaveAsSingleFile-boolean-) | يحدد ما إذا كان يتم حفظ HTML كملف واحد. |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | يضبط الأوراق التي سيتم عرضها. |
| [setShowAllSheets(boolean value)](#setShowAllSheets-boolean-) | يحدد ما إذا كان يتم عرض جميع الأوراق عند حفظها كملف HTML واحد. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | يحدد ما إذا كان يتم فرز الأسماء المعرفة الخارجية قبل حفظ الملف. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | يحدد ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف. |
| [setSpaceMode(int value)](#setSpaceMode-int-) | يحدد كيفية عرض المسافات في مخرجات HTML. |
| [setStreamProvider(IStreamProvider value)](#setStreamProvider-com.aspose.cells.IStreamProvider-) | يضبط IStreamProvider لتصدير الكائنات. |
| [setTableCssId(String value)](#setTableCssId-java.lang.String-) | يضبط البادئة لاسم نوع CSS مثل tr و col و td وما إلى ذلك، وهي موجودة داخل عنصر الجدول الذي يحتوي على السمة TableCssId المحددة. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | يحدد ما إذا كان يتم تحديث إعدادات Smart Art. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | يحدد ما إذا كان يتم التحقق من صحة الخلايا المدمجة قبل حفظ الملف. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | يضبط رد النداء للتحذير. |
| [setWidthScalable(boolean value)](#setWidthScalable-boolean-) | يحدد ما إذا كان يتم تصدير عرض العمود بوحدة المقياس إلى HTML. |
| [setWorksheetScalable(boolean value)](#setWorksheetScalable-boolean-) | يحدد ما إذا كان يتم تكبير أو تصغير HTML عبر مستوى تكبير ورقة العمل عند حفظ الملف إلى HTML، القيمة الافتراضية هي false. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### HtmlSaveOptions() {#HtmlSaveOptions--}
```
public HtmlSaveOptions()
```


ينشئ خيارات لحفظ ملف html.

### HtmlSaveOptions(int saveFormat) {#HtmlSaveOptions-int-}
```
public HtmlSaveOptions(int saveFormat)
```


ينشئ خيارات لحفظ ملف htm.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). تنسيق الملف. يجب أن يكون أحد الأنواع التالية: [SaveFormat.HTML](../../com.aspose.cells/saveformat\#HTML) أو [SaveFormat.M\_HTML](../../com.aspose.cells/saveformat\#M-HTML)، وإلا سيتم تعيين تنسيق الحفظ كـ [SaveFormat.HTML](../../com.aspose.cells/saveformat\#HTML) تلقائيًا. |

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
### getAddGenericFont() {#getAddGenericFont--}
```
public boolean getAddGenericFont()
```


يشير إلى ما إذا كان يجب إضافة خط عام إلى خاصية CSS font-family. القيمة الافتراضية هي true.

**Returns:**
boolean
### getAddTooltipText() {#getAddTooltipText--}
```
public boolean getAddTooltipText()
```


يشير إلى ما إذا كان يتم إضافة نص تلميح عندما لا يمكن عرض البيانات بالكامل. القيمة الافتراضية هي false.

**Returns:**
boolean
### getAttachedFilesDirectory() {#getAttachedFilesDirectory--}
```
public String getAttachedFilesDirectory()
```


الدليل الذي سيتم حفظ الملفات المرفقة فيه. يُستخدم فقط لحفظ تدفق HTML.

**Returns:**
java.lang.String
### getAttachedFilesUrlPrefix() {#getAttachedFilesUrlPrefix--}
```
public String getAttachedFilesUrlPrefix()
```


حدد بادئة URL للملفات المرفقة مثل الصورة في ملف HTML. يُستخدم فقط لحفظ تدفق HTML.

**Returns:**
java.lang.String
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


يحدد ما إذا كان سيتم حساب الصيغ قبل حفظ ملف HTML.

**Remarks**

القيمة الافتراضية هي false.

**Returns:**
boolean
### getCellCssPrefix() {#getCellCssPrefix--}
```
public String getCellCssPrefix()
```


يحصل على بادئة اسم CSS، القيمة الافتراضية هي "".

**Returns:**
java.lang.String
### getCellNameAttribute() {#getCellNameAttribute--}
```
public String getCellNameAttribute()
```


يحدد السمة التي تشير إلى اسم الخلية (CellName) الذي سيُكتب. (مثال: إذا كانت القيمة "id"، فبالنسبة للخلية "A1" سيكون الناتج: <td id='A1'>). القيمة الافتراضية هي null.

**Returns:**
java.lang.String
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المتعلقة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32K. عندما تدخل قيمة أطول من 32K، سيتم قطعها.

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
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


إذا كان صحيحًا ولم يكن الدليل موجودًا، فسيتم إنشاء الدليل تلقائيًا قبل حفظ الملف.

**Remarks**

القيمة الافتراضية هي false.

**Returns:**
boolean
### getCssStyles() {#getCssStyles--}
```
public String getCssStyles()
```


يحصل على أنماط CSS الإضافية للمنسق. يعمل فقط عندما تكون [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) مساوية لـ True.  CssStyles="body \{ padding: 5px \}";

**Returns:**
java.lang.String
### getDataBarRenderMode() {#getDataBarRenderMode--}
```
public int getDataBarRenderMode()
```


يمثل وضع كيفية عرض DataBar عند تحويل ملفات Excel إلى ملفات HTML. القيمة الافتراضية هي [DataBarRenderMode.BACKGROUND\_COLOR](../../com.aspose.cells/databarrendermode\#BACKGROUND-COLOR).

انظر إلى [DataBarRenderMode](../../com.aspose.cells/databarrendermode).

**Returns:**
int
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


حدد اسم الخط الافتراضي لتصدير HTML، سيتم استخدام الخط الافتراضي عندما لا يكون خط النمط موجودًا، إذا كانت هذه الخاصية فارغة (null)، سيستخدم Aspose.Cells خطًا عالميًا يملك نفس عائلة الخط الأصلي، القيمة الافتراضية هي null.

**Returns:**
java.lang.String
### getDisableCss() {#getDisableCss--}
```
public boolean getDisableCss()
```


يشير إلى ما إذا كانت الأنماط المضمنة فقط تُطبق دون الاعتماد على CSS. القيمة الافتراضية هي false.

**Returns:**
boolean
### getDisableDownlevelRevealedComments() {#getDisableDownlevelRevealedComments--}
```
public boolean getDisableDownlevelRevealedComments()
```


يحدد ما إذا كان يتم تعطيل التعليقات الشرطية Downlevel-revealed عند تصدير الملف إلى HTML، القيمة الافتراضية هي false.

**Returns:**
boolean
### getEmbeddedFontType() {#getEmbeddedFontType--}
```
public int getEmbeddedFontType()
```


يحصل على نوع تضمين ملف الخط داخل ملف HTML. القيمة الافتراضية هي [HtmlEmbeddedFontType.NONE](../../com.aspose.cells/htmlembeddedfonttype\#NONE) مما يعني عدم تضمين أي خط في HTML.

انظر إلى [HtmlEmbeddedFontType](../../com.aspose.cells/htmlembeddedfonttype).

**Returns:**
int
### getEnableCssCustomProperties() {#getEnableCssCustomProperties--}
```
public boolean getEnableCssCustomProperties()
```


حسّن مخرجات HTML باستخدام خصائص CSS المخصصة. على سبيل المثال، في حالة وجود تكرارات متعددة لصورة base64 واحدة، تسمح الخاصية المخصصة بحفظ بيانات الصورة مرة واحدة فقط، مما يحسن أداء HTML الناتج. القيمة الافتراضية هي false.

**Returns:**
boolean
### getEncodeEntityAsCode() {#getEncodeEntityAsCode--}
```
public boolean getEncodeEntityAsCode()
```


يشير إلى ما إذا كانت كيانات أحرف HTML تُستبدل بالرمز العشري. (مثال: "&nbsp;" تُستبدل بـ "&\#160;"). القيمة الافتراضية هي false.

**Returns:**
boolean
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


إذا لم يتم تحديده، استخدم Encoding.UTF8 كنمط الترميز الافتراضي.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```


يشير إلى ما إذا كان يتم تشفير خصائص المستند عند الحفظ كملف .xls. القيمة الافتراضية هي true.

**Remarks**

لملفات .xls, .xlsx, .xlsb و .xlsm فقط.

**Returns:**
boolean
### getExcludeUnusedStyles() {#getExcludeUnusedStyles--}
```
public boolean getExcludeUnusedStyles()
```


يشير إلى ما إذا كان يتم استبعاد الأنماط غير المستخدمة. بالنسبة لملفات HTML المُولدة، يمكن أن يؤدي استبعاد الأنماط غير المستخدمة إلى تقليل حجم الملف دون التأثير على المظهر البصري. لذلك القيمة الافتراضية لهذه الخاصية هي true. إذا كان المستخدم يحتاج إلى الاحتفاظ بجميع الأنماط في المصنف للـ HTML المُولد (مثل السيناريو الذي يحتاج فيه المستخدم إلى استعادة المصنف من الـ HTML المُولد لاحقًا)، يرجى ضبط هذه الخاصية على false.

**Returns:**
boolean
### getExportActiveWorksheetOnly() {#getExportActiveWorksheetOnly--}
```
public boolean getExportActiveWorksheetOnly()
```


يشير إلى ما إذا كان يتم تصدير الورقة النشطة فقط إلى ملف HTML. إذا كانت true فستُصدَّر الورقة النشطة فقط إلى ملف HTML؛ إذا كانت false فسيُصدَّر المصنف بالكامل إلى ملف HTML. القيمة الافتراضية هي false.

**Returns:**
boolean
### getExportArea() {#getExportArea--}
```
public CellArea getExportArea()
```


يحصل على نطاق CellArea المُصدّر للورقة النشطة الحالية. إذا قمت بتعيين هذه السمة، سيتم حذف منطقة الطباعة للورقة النشطة الحالية. سيتم تصدير المنطقة المحددة فقط عند حفظ الملف إلى HTML.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getExportBogusRowData() {#getExportBogusRowData--}
```
public boolean getExportBogusRowData()
```


يشير إلى ما إذا كان يتم تصدير بيانات الصف السفلي الزائفة. القيمة الافتراضية هي true. إذا كنت ترغب في استيراد ملف HTML أو MHT إلى Excel، يرجى الحفاظ على القيمة الافتراضية.

**Returns:**
boolean
### getExportCellCoordinate() {#getExportCellCoordinate--}
```
public boolean getExportCellCoordinate()
```


يشير إلى ما إذا كان يتم تصدير إحداثيات إكسل للخلايا غير الفارغة عند حفظ الملف بصيغة html. القيمة الافتراضية هي false. إذا كنت ترغب في استيراد ملف html الناتج إلى إكسل، يرجى الحفاظ على القيمة الافتراضية.

**Returns:**
boolean
### getExportCommentsType() {#getExportCommentsType--}
```
public int getExportCommentsType()
```


يمثل نوع تصدير التعليقات إلى ملفات HTML.

انظر [PrintCommentsType](../../com.aspose.cells/printcommentstype).

**Returns:**
int
### getExportDataOptions() {#getExportDataOptions--}
```
public int getExportDataOptions()
```


يحدد قاعدة تصدير بيانات ملف HTML. القيمة الافتراضية هي All.

انظر [HtmlExportDataOptions](../../com.aspose.cells/htmlexportdataoptions).

**Returns:**
int
### getExportDocumentProperties() {#getExportDocumentProperties--}
```
public boolean getExportDocumentProperties()
```


يحدد ما إذا كان يتم تصدير خصائص المستند. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف HTML أو MHT إلى Excel، يرجى الحفاظ على القيمة الافتراضية.

**Returns:**
boolean
### getExportExtraHeadings() {#getExportExtraHeadings--}
```
public boolean getExportExtraHeadings()
```


يشير إلى ما إذا كان يتم تصدير عناوين إضافية عندما يكون طول النص أطول من الحد الأقصى لعرض العمود. القيمة الافتراضية هي false. إذا كنت ترغب في استيراد ملف html إلى إكسل، يرجى الحفاظ على القيمة الافتراضية.

**Returns:**
boolean
### getExportFormula() {#getExportFormula--}
```
public boolean getExportFormula()
```


يشير إلى ما إذا كان يتم تصدير الصيغ عند حفظ الملف بصيغة html. القيمة الافتراضية هي true. إذا كنت ترغب في استيراد ملف html الناتج إلى إكسل، يرجى الحفاظ على القيمة الافتراضية.

**Returns:**
boolean
### getExportFrameScriptsAndProperties() {#getExportFrameScriptsAndProperties--}
```
public boolean getExportFrameScriptsAndProperties()
```


يشير إلى ما إذا كان يتم تصدير سكريبتات الإطار وخصائص المستند. القيمة الافتراضية هي true. إذا كنت ترغب في استيراد ملف html أو mht إلى إكسل، يرجى الحفاظ على القيمة الافتراضية.

**Returns:**
boolean
### getExportGridLines() {#getExportGridLines--}
```
public boolean getExportGridLines()
```


الإشارة إلى ما إذا كان يتم تصدير خطوط الشبكة. القيمة الافتراضية هي false.

**Returns:**
boolean
### getExportHeadings() {#getExportHeadings--}
```
public boolean getExportHeadings()
```


يحدد ما إذا كان يتم تصدير عناوين الصفوف والأعمدة للورقة عند الحفظ كملفات HTML.

**Remarks**

ملاحظة: هذا العضو الآن غير صالح. بدلاً من ذلك، يرجى استخدام خاصية HtmlSaveOptions.ExportRowColumnHeadings. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
boolean
### getExportHiddenWorksheet() {#getExportHiddenWorksheet--}
```
public boolean getExportHiddenWorksheet()
```


الإشارة إلى ما إذا كان يتم تصدير محتوى ورقة العمل المخفي. القيمة الافتراضية هي true.

**Returns:**
boolean
### getExportImagesAsBase64() {#getExportImagesAsBase64--}
```
public boolean getExportImagesAsBase64()
```


يحدد ما إذا كانت الصور تُحفظ بتنسيق Base64 إلى HTML أو MHTML أو EPUB.

**Remarks**

عند ضبط هذه الخاصية على true يتم تصدير بيانات الصورة مباشرةً على عناصر img ولا يتم إنشاء ملفات منفصلة.

**Returns:**
boolean
### getExportNamedRangeAnchors() {#getExportNamedRangeAnchors--}
```
public boolean getExportNamedRangeAnchors()
```


يشير إلى ما إذا كان يتم تصدير عناصر الربط (anchor) للنطاقات المسماة عند الحفظ بصيغة HTML. القيمة الافتراضية هي true.

**Returns:**
boolean
### getExportObjectListener() {#getExportObjectListener--}
```
public IExportObjectListener getExportObjectListener()
```


يحصل على ExportObjectListener لتصدير الكائنات.

**Remarks**

ملاحظة: هذه الخاصية الآن غير صالحة. بدلاً من ذلك، يرجى استخدام خاصية HtmlSaveOptions.IStreamProvider. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أغسطس 2015. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
[IExportObjectListener](../../com.aspose.cells/iexportobjectlistener)
### getExportPageFooters() {#getExportPageFooters--}
```
public boolean getExportPageFooters()
```


يحدد ما إذا كان يتم تصدير رؤوس الصفحات.

**Remarks**

يعمل فقط عندما يكون [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) هو True.

**Returns:**
boolean
### getExportPageHeaders() {#getExportPageHeaders--}
```
public boolean getExportPageHeaders()
```


يحدد ما إذا كان يتم تصدير رؤوس الصفحات.

**Remarks**

يعمل فقط عندما يكون [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) هو True.

**Returns:**
boolean
### getExportPrintAreaOnly() {#getExportPrintAreaOnly--}
```
public boolean getExportPrintAreaOnly()
```


يشير إلى ما إذا كان يتم تصدير منطقة الطباعة فقط إلى ملف html. القيمة الافتراضية هي false.

**Returns:**
boolean
### getExportRowColumnHeadings() {#getExportRowColumnHeadings--}
```
public boolean getExportRowColumnHeadings()
```


يحدد ما إذا كان يتم تصدير عناوين الصفوف والأعمدة للورقة عند الحفظ كملفات HTML.

**Remarks**

القيمة الافتراضية هي false.

**Returns:**
boolean
### getExportSimilarBorderStyle() {#getExportSimilarBorderStyle--}
```
public boolean getExportSimilarBorderStyle()
```


يشير إلى ما إذا كان يتم تصدير نمط الحدود المشابه عندما لا يدعم المتصفحات نمط الحدود. إذا كنت ترغب في استيراد ملف html أو mht إلى إكسل، يرجى الحفاظ على القيمة الافتراضية. القيمة الافتراضية هي false.

**Returns:**
boolean
### getExportSingleTab() {#getExportSingleTab--}
```
public boolean getExportSingleTab()
```


يشير إلى ما إذا كان يتم تصدير علامة التبويب الوحيدة عندما يحتوي الملف على ورقة عمل واحدة فقط. القيمة الافتراضية هي false.

**Returns:**
boolean
### getExportWorkbookProperties() {#getExportWorkbookProperties--}
```
public boolean getExportWorkbookProperties()
```


الإشارة إلى ما إذا كان يتم تصدير خصائص المصنف. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html أو mht إلى Excel، يرجى الحفاظ على القيمة الافتراضية.

**Returns:**
boolean
### getExportWorksheetCSSSeparately() {#getExportWorksheetCSSSeparately--}
```
public boolean getExportWorksheetCSSSeparately()
```


الإشارة إلى ما إذا كان يتم تصدير CSS لورقة العمل بشكل منفصل. القيمة الافتراضية هي false.

**Returns:**
boolean
### getExportWorksheetProperties() {#getExportWorksheetProperties--}
```
public boolean getExportWorksheetProperties()
```


الإشارة إلى ما إذا كان يتم تصدير خصائص ورقة العمل. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html أو mht إلى Excel، يرجى الحفاظ على القيمة الافتراضية.

**Returns:**
boolean
### getFilePathProvider() {#getFilePathProvider--}
```
public IFilePathProvider getFilePathProvider()
```


يحصل على IFilePathProvider لتصدير ورقة العمل إلى HTML بشكل منفصل.

**Returns:**
[IFilePathProvider](../../com.aspose.cells/ifilepathprovider)
### getFormatDataIgnoreColumnWidth() {#getFormatDataIgnoreColumnWidth--}
```
public boolean getFormatDataIgnoreColumnWidth()
```


يشير إلى ما إذا كان يتم عرض جميع البيانات المنسقة للخلية عندما يتجاوز النص عرض العمود. إذا كان true يتم تجاهل عرض العمود وتُصدَّر جميع بيانات الخلية. إذا كان false تُصدَّر البيانات كما في Excel. القيمة الافتراضية هي false.

**Returns:**
boolean
### getHiddenColDisplayType() {#getHiddenColDisplayType--}
```
public int getHiddenColDisplayType()
```


العمود المخفي (عرض هذا العمود هو 0) في Excel، قبل حفظه بصيغة HTML، إذا كان HtmlHiddenColDisplayType هو "Remove"، فلن يتم إخراج العمود المخفي، إذا كانت القيمة "Hidden"، سيتم إخراج العمود لكنه سيظل مخفيًا، القيمة الافتراضية هي "Hidden".

انظر [HtmlHiddenColDisplayType](../../com.aspose.cells/htmlhiddencoldisplaytype).

**Returns:**
int
### getHiddenRowDisplayType() {#getHiddenRowDisplayType--}
```
public int getHiddenRowDisplayType()
```


الصف المخفي (ارتفاع هذا الصف هو 0) في Excel، قبل حفظه بصيغة HTML، إذا كان HtmlHiddenRowDisplayType هو "Remove"، فلن يتم إخراج الصف المخفي، إذا كانت القيمة "Hidden"، سيتم إخراج الصف لكنه سيظل مخفيًا، القيمة الافتراضية هي "Hidden".

انظر [HtmlHiddenRowDisplayType](../../com.aspose.cells/htmlhiddenrowdisplaytype).

**Returns:**
int
### getHideOverflowWrappedText() {#getHideOverflowWrappedText--}
```
public boolean getHideOverflowWrappedText()
```


يشير إلى ما إذا كان يتم إخفاء النص المتجاوز عندما يكون تنسيق الخلية مضبوطًا على التفاف النص. القيمة الافتراضية هي false

**Returns:**
boolean
### getHtmlCrossStringType() {#getHtmlCrossStringType--}
```
public int getHtmlCrossStringType()
```


يشير إلى ما إذا كان سيتم عرض سلسلة عبر الخلايا بنفس طريقة MS Excel عند حفظ ملف Excel بصيغة html. القيمة الافتراضية هي Default، لذا بالنسبة للسلاسل عبر الخلايا، هناك فرق بسيط بين ملفات html التي تُنشئها Aspose.Cells و MS Excel. لكن الأداء لإنشاء ملفات html الكبيرة، ضبط القيمة إلى Cross سيكون أسرع عدة مرات مقارنةً بضبطها إلى Default أو Fit2Cell.

انظر [HtmlCrossType](../../com.aspose.cells/htmlcrosstype).

**Returns:**
int
### getHtmlVersion() {#getHtmlVersion--}
```
public int getHtmlVersion()
```


يحدد نسخة معيار HTML التي يجب استخدامها عند حفظ الصيغة HTML. القيمة الافتراضية هي HtmlVersion.Default.

انظر [HtmlVersion](../../com.aspose.cells/htmlversion).

**Returns:**
int
### getIgnoreInvisibleShapes() {#getIgnoreInvisibleShapes--}
```
public boolean getIgnoreInvisibleShapes()
```


الإشارة إلى ما إذا كان يتم تصدير الأشكال غير المرئية.

**Remarks**

القيمة الافتراضية هي false.

**Returns:**
boolean
### getImageOptions() {#getImageOptions--}
```
public ImageOrPrintOptions getImageOptions()
```


احصل على كائن ImageOrPrintOptions قبل التصدير.

**Returns:**
[ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)
### getImageScalable() {#getImageScalable--}
```
public boolean getImageScalable()
```


يشير إلى ما إذا كان يتم استخدام وحدة قابلة للتوسع لوصف عرض الصورة عند استخدام وحدة قابلة للتوسع لوصف عرض العمود. القيمة الافتراضية هي true.

**Returns:**
boolean
### getLayoutMode() {#getLayoutMode--}
```
public int getLayoutMode()
```


يحصل على وضع التخطيط عند الحفظ إلى HTML. القيمة الافتراضية هي [HtmlLayoutMode.NORMAL](../../com.aspose.cells/htmllayoutmode\#NORMAL)

انظر [HtmlLayoutMode](../../com.aspose.cells/htmllayoutmode).

**Returns:**
int
### getLinkTargetType() {#getLinkTargetType--}
```
public int getLinkTargetType()
```


تشير إلى نوع سمة الهدف في رابط `<a>`. القيمة الافتراضية هي HtmlLinkTargetType.Parent.

انظر [HtmlLinkTargetType](../../com.aspose.cells/htmllinktargettype).

**Returns:**
int
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


يحدد ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق قبل حفظ الملف.

**Remarks**

القيمة الافتراضية هي false.

**Returns:**
boolean
### getMergeEmptyTdForcely() {#getMergeEmptyTdForcely--}
```
public boolean getMergeEmptyTdForcely()
```


يشير إلى ما إذا كان سيتم دمج عنصر TD الفارغ قسراً عند تصدير الملف إلى html. سيقل حجم ملف html بشكل كبير بعد تعيين القيمة إلى true. القيمة الافتراضية هي false. إذا كنت ترغب في استيراد ملف html إلى Excel أو تصدير خطوط شبكة مثالية عند حفظ الملف إلى html، يرجى الحفاظ على القيمة الافتراضية.

**Returns:**
boolean
### getMergeEmptyTdType() {#getMergeEmptyTdType--}
```
public int getMergeEmptyTdType()
```


الخيار لدمج الخلايا الفارغة المتجاورة (عناصر td الفارغة). القيمة الافتراضية هي MergeEmptyTdType.Default.

انظر [MergeEmptyTdType](../../com.aspose.cells/mergeemptytdtype).

**Returns:**
int
### getOfficeMathOutputMode() {#getOfficeMathOutputMode--}
```
public int getOfficeMathOutputMode()
```


يحدد كيفية تصدير كائنات OfficeMath إلى HTML، القيمة الافتراضية هي Image.

انظر [HtmlOfficeMathOutputType](../../com.aspose.cells/htmlofficemathoutputtype).

**Returns:**
int
### getPageTitle() {#getPageTitle--}
```
public String getPageTitle()
```


عنوان صفحة html. يستخدم فقط عند حفظ إلى تدفق html.

**Returns:**
java.lang.String
### getParseHtmlTagInCell() {#getParseHtmlTagInCell--}
```
public boolean getParseHtmlTagInCell()
```


يشير إلى ما إذا كان يجب تحليل علامة html (مثل `<div></div>`) في الخلية كقيمة خلية أم الحفاظ عليها كما هي. القيمة الافتراضية هي true.

**Returns:**
boolean
### getPresentationPreference() {#getPresentationPreference--}
```
public boolean getPresentationPreference()
```


تشير إلى ما إذا كان ملف html أو mht هو تفضيل العرض. القيمة الافتراضية هي false. إذا كنت تريد الحصول على عرض أكثر جمالاً، يرجى تعيين القيمة إلى true.

**Returns:**
boolean
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


يحدد ما إذا كان يتم تخزين أحدث بيانات المخطط مؤقتًا.

**Returns:**
boolean
### getSaveAsSingleFile() {#getSaveAsSingleFile--}
```
public boolean getSaveAsSingleFile()
```


يشير إلى ما إذا كان سيتم حفظ html كملف واحد. القيمة الافتراضية هي false.

**Remarks**

إذا كان هناك عدة أوراق عمل أو موارد أخرى مطلوبة مثل الصور في المصنف، عادةً ما تحتاج تلك الأوراق والموارد إلى حفظها في ملفات منفصلة. في بعض السيناريوهات، قد يحتاج المستخدم إلى الحصول على ملف واحد فقط لتسهيل النقل. إذا كان الأمر كذلك، يمكن للمستخدم تعيين هذه الخاصية إلى true.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


يحصل على صيغة حفظ الملف.

انظر [SaveFormat](../../com.aspose.cells/saveformat).

**Returns:**
int
### getSheetSet() {#getSheetSet--}
```
public SheetSet getSheetSet()
```


يحصل على الأوراق التي سيتم عرضها. الافتراضي هو جميع الأوراق المرئية في المصنف: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\\#getVisible--).

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getShowAllSheets() {#getShowAllSheets--}
```
public boolean getShowAllSheets()
```


يحدد ما إذا كان يتم عرض جميع الأوراق عند حفظها كملف HTML واحد.

**Remarks**

يعمل فقط عندما يكون [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) هو True.

**Returns:**
boolean
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
### getSpaceMode() {#getSpaceMode--}
```
public int getSpaceMode()
```


يشير إلى كيفية عرض المسافات في مخرجات HTML. يتم تطبيق هذا الخيار حالياً فقط على التنسيقات الرقمية (مثل تنسيق المحاسبة). القيمة الافتراضية هي [HtmlSpaceMode.CSS](../../com.aspose.cells/htmlspacemode\\#CSS).

انظر [HtmlSpaceMode](../../com.aspose.cells/htmlspacemode).

**Returns:**
int
### getStreamProvider() {#getStreamProvider--}
```
public IStreamProvider getStreamProvider()
```


يحصل على IStreamProvider لتصدير الكائنات.

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getTableCssId() {#getTableCssId--}
```
public String getTableCssId()
```


يحصل على بادئة اسم نوع css مثل tr, col, td وما إلى ذلك، وهي موجودة في عنصر الجدول الذي يحتوي على السمة TableCssId المحددة. القيمة الافتراضية هي "".

**Returns:**
java.lang.String
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
### getWidthScalable() {#getWidthScalable--}
```
public boolean getWidthScalable()
```


يشير إلى ما إذا كان سيتم تصدير عرض العمود بوحدة المقياس إلى html. القيمة الافتراضية هي false.

**Returns:**
boolean
### getWorksheetScalable() {#getWorksheetScalable--}
```
public boolean getWorksheetScalable()
```


يحدد ما إذا كان يتم تكبير أو تصغير HTML عبر مستوى تكبير ورقة العمل عند حفظ الملف إلى HTML، القيمة الافتراضية هي false.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBorderCollapsed() {#isBorderCollapsed--}
```
public boolean isBorderCollapsed()
```


يشير إلى ما إذا كانت حدود الجدول مدمجة. القيمة الافتراضية هي true.

**Returns:**
boolean
### isExpImageToTempDir() {#isExpImageToTempDir--}
```
public boolean isExpImageToTempDir()
```


يشير إلى ما إذا كان سيتم تصدير ملفات الصور إلى دليل مؤقت. يستخدم فقط عند حفظ إلى تدفق html.

**Returns:**
boolean
### isExportComments() {#isExportComments--}
```
public boolean isExportComments()
```


يحدد ما إذا كان يتم تصدير التعليقات عند حفظ الملف إلى HTML، القيمة الافتراضية هي false.

**Returns:**
boolean
### isFullPathLink() {#isFullPathLink--}
```
public boolean isFullPathLink()
```


تشير إلى ما إذا كان سيتم استخدام رابط المسار الكامل في sheet00x.htm, filelist.xml و tabstrip.htm. القيمة الافتراضية هي false.

**Returns:**
boolean
### isIECompatible() {#isIECompatible--}
```
public boolean isIECompatible()
```


تشير إلى ما إذا كان HTML الناتج متوافقًا مع متصفح IE. القيمة الافتراضية هي false.

**Returns:**
boolean
### isJsBrowserCompatible() {#isJsBrowserCompatible--}
```
public boolean isJsBrowserCompatible()
```


يشير إلى ما إذا كان JavaScript متوافقًا مع المتصفحات التي لا تدعم JavaScript. القيمة الافتراضية هي true.

**Returns:**
boolean
### isMobileCompatible() {#isMobileCompatible--}
```
public boolean isMobileCompatible()
```


يشير إلى ما إذا كان HTML الناتج متوافقًا مع الأجهزة المحمولة. القيمة الافتراضية هي false.

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




### setAddGenericFont(boolean value) {#setAddGenericFont-boolean-}
```
public void setAddGenericFont(boolean value)
```


يشير إلى ما إذا كان يجب إضافة خط عام إلى خاصية CSS font-family. القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAddTooltipText(boolean value) {#setAddTooltipText-boolean-}
```
public void setAddTooltipText(boolean value)
```


يشير إلى ما إذا كان يتم إضافة نص تلميح عندما لا يمكن عرض البيانات بالكامل. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAttachedFilesDirectory(String value) {#setAttachedFilesDirectory-java.lang.String-}
```
public void setAttachedFilesDirectory(String value)
```


الدليل الذي سيتم حفظ الملفات المرفقة فيه. يُستخدم فقط لحفظ تدفق HTML.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setAttachedFilesUrlPrefix(String value) {#setAttachedFilesUrlPrefix-java.lang.String-}
```
public void setAttachedFilesUrlPrefix(String value)
```


حدد بادئة URL للملفات المرفقة مثل الصورة في ملف HTML. يُستخدم فقط لحفظ تدفق HTML.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setBorderCollapsed(boolean value) {#setBorderCollapsed-boolean-}
```
public void setBorderCollapsed(boolean value)
```


يشير إلى ما إذا كانت حدود الجدول مدمجة. القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

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


يحدد ما إذا كان سيتم حساب الصيغ قبل حفظ ملف HTML.

**Remarks**

القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setCellCssPrefix(String value) {#setCellCssPrefix-java.lang.String-}
```
public void setCellCssPrefix(String value)
```


يضبط بادئة اسم CSS، القيمة الافتراضية هي \"\".

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setCellNameAttribute(String value) {#setCellNameAttribute-java.lang.String-}
```
public void setCellNameAttribute(String value)
```


يحدد السمة التي تشير إلى اسم الخلية (CellName) الذي سيُكتب. (مثال: إذا كانت القيمة "id"، فبالنسبة للخلية "A1" سيكون الناتج: <td id='A1'>). القيمة الافتراضية هي null.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المتعلقة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32K. عندما تدخل قيمة أطول من 32K، سيتم قطعها.

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

### setCssStyles(String value) {#setCssStyles-java.lang.String-}
```
public void setCssStyles(String value)
```


يضبط أنماط css الإضافية للمنسق. يعمل فقط عندما تكون [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\\#getSaveAsSingleFile--) مساوية لـ True.  CssStyles=\"body \\{ padding: 5px \\}\";

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setDataBarRenderMode(int value) {#setDataBarRenderMode-int-}
```
public void setDataBarRenderMode(int value)
```


يمثل وضع كيفية عرض DataBar عند تحويل ملفات Excel إلى ملفات HTML. القيمة الافتراضية هي [DataBarRenderMode.BACKGROUND\_COLOR](../../com.aspose.cells/databarrendermode\#BACKGROUND-COLOR).

انظر إلى [DataBarRenderMode](../../com.aspose.cells/databarrendermode).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


حدد اسم الخط الافتراضي لتصدير HTML، سيتم استخدام الخط الافتراضي عندما لا يكون خط النمط موجودًا، إذا كانت هذه الخاصية فارغة (null)، سيستخدم Aspose.Cells خطًا عالميًا يملك نفس عائلة الخط الأصلي، القيمة الافتراضية هي null.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setDisableCss(boolean value) {#setDisableCss-boolean-}
```
public void setDisableCss(boolean value)
```


يشير إلى ما إذا كانت الأنماط المضمنة فقط تُطبق دون الاعتماد على CSS. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setDisableDownlevelRevealedComments(boolean value) {#setDisableDownlevelRevealedComments-boolean-}
```
public void setDisableDownlevelRevealedComments(boolean value)
```


يحدد ما إذا كان يتم تعطيل التعليقات الشرطية Downlevel-revealed عند تصدير الملف إلى HTML، القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEmbeddedFontType(int value) {#setEmbeddedFontType-int-}
```
public void setEmbeddedFontType(int value)
```


يضبط نوع تضمين ملف الخط في ملف html. القيمة الافتراضية هي [HtmlEmbeddedFontType.NONE](../../com.aspose.cells/htmlembeddedfonttype\\#NONE) والتي تشير إلى عدم تضمين أي خط في html.

انظر إلى [HtmlEmbeddedFontType](../../com.aspose.cells/htmlembeddedfonttype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setEnableCssCustomProperties(boolean value) {#setEnableCssCustomProperties-boolean-}
```
public void setEnableCssCustomProperties(boolean value)
```


حسّن مخرجات HTML باستخدام خصائص CSS المخصصة. على سبيل المثال، في حالة وجود تكرارات متعددة لصورة base64 واحدة، تسمح الخاصية المخصصة بحفظ بيانات الصورة مرة واحدة فقط، مما يحسن أداء HTML الناتج. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEncodeEntityAsCode(boolean value) {#setEncodeEntityAsCode-boolean-}
```
public void setEncodeEntityAsCode(boolean value)
```


يشير إلى ما إذا كانت كيانات أحرف HTML تُستبدل بالرمز العشري. (مثال: "&nbsp;" تُستبدل بـ "&\#160;"). القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


إذا لم يتم تحديده، استخدم Encoding.UTF8 كنمط الترميز الافتراضي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

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

### setExcludeUnusedStyles(boolean value) {#setExcludeUnusedStyles-boolean-}
```
public void setExcludeUnusedStyles(boolean value)
```


يشير إلى ما إذا كان يتم استبعاد الأنماط غير المستخدمة. بالنسبة لملفات HTML المُولدة، يمكن أن يؤدي استبعاد الأنماط غير المستخدمة إلى تقليل حجم الملف دون التأثير على المظهر البصري. لذلك القيمة الافتراضية لهذه الخاصية هي true. إذا كان المستخدم يحتاج إلى الاحتفاظ بجميع الأنماط في المصنف للـ HTML المُولد (مثل السيناريو الذي يحتاج فيه المستخدم إلى استعادة المصنف من الـ HTML المُولد لاحقًا)، يرجى ضبط هذه الخاصية على false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExpImageToTempDir(boolean value) {#setExpImageToTempDir-boolean-}
```
public void setExpImageToTempDir(boolean value)
```


يشير إلى ما إذا كان سيتم تصدير ملفات الصور إلى دليل مؤقت. يستخدم فقط عند حفظ إلى تدفق html.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExportActiveWorksheetOnly(boolean value) {#setExportActiveWorksheetOnly-boolean-}
```
public void setExportActiveWorksheetOnly(boolean value)
```


يشير إلى ما إذا كان يتم تصدير الورقة النشطة فقط إلى ملف HTML. إذا كانت true فستُصدَّر الورقة النشطة فقط إلى ملف HTML؛ إذا كانت false فسيُصدَّر المصنف بالكامل إلى ملف HTML. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExportArea(CellArea value) {#setExportArea-com.aspose.cells.CellArea-}
```
public void setExportArea(CellArea value)
```


يضبط نطاق الخلايا (CellArea) الذي سيتم تصديره من ورقة العمل النشطة الحالية. إذا قمت بتعيين هذه السمة، سيتم حذف منطقة الطباعة من ورقة العمل النشطة الحالية. سيتم تصدير المنطقة المحددة فقط عند حفظ الملف إلى html.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [CellArea](../../com.aspose.cells/cellarea) |  |

### setExportBogusRowData(boolean value) {#setExportBogusRowData-boolean-}
```
public void setExportBogusRowData(boolean value)
```


يشير إلى ما إذا كان يتم تصدير بيانات الصف السفلي الزائفة. القيمة الافتراضية هي true. إذا كنت ترغب في استيراد ملف HTML أو MHT إلى Excel، يرجى الحفاظ على القيمة الافتراضية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExportCellCoordinate(boolean value) {#setExportCellCoordinate-boolean-}
```
public void setExportCellCoordinate(boolean value)
```


يشير إلى ما إذا كان يتم تصدير إحداثيات إكسل للخلايا غير الفارغة عند حفظ الملف بصيغة html. القيمة الافتراضية هي false. إذا كنت ترغب في استيراد ملف html الناتج إلى إكسل، يرجى الحفاظ على القيمة الافتراضية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExportComments(boolean value) {#setExportComments-boolean-}
```
public void setExportComments(boolean value)
```


يحدد ما إذا كان يتم تصدير التعليقات عند حفظ الملف إلى HTML، القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExportCommentsType(int value) {#setExportCommentsType-int-}
```
public void setExportCommentsType(int value)
```


يمثل نوع تصدير التعليقات إلى ملفات HTML.

انظر [PrintCommentsType](../../com.aspose.cells/printcommentstype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setExportDataOptions(int value) {#setExportDataOptions-int-}
```
public void setExportDataOptions(int value)
```


يحدد قاعدة تصدير بيانات ملف HTML. القيمة الافتراضية هي All.

انظر [HtmlExportDataOptions](../../com.aspose.cells/htmlexportdataoptions).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setExportDocumentProperties(boolean value) {#setExportDocumentProperties-boolean-}
```
public void setExportDocumentProperties(boolean value)
```


يحدد ما إذا كان يتم تصدير خصائص المستند. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف HTML أو MHT إلى Excel، يرجى الحفاظ على القيمة الافتراضية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExportExtraHeadings(boolean value) {#setExportExtraHeadings-boolean-}
```
public void setExportExtraHeadings(boolean value)
```


يشير إلى ما إذا كان يتم تصدير عناوين إضافية عندما يكون طول النص أطول من الحد الأقصى لعرض العمود. القيمة الافتراضية هي false. إذا كنت ترغب في استيراد ملف html إلى إكسل، يرجى الحفاظ على القيمة الافتراضية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExportFormula(boolean value) {#setExportFormula-boolean-}
```
public void setExportFormula(boolean value)
```


يشير إلى ما إذا كان يتم تصدير الصيغ عند حفظ الملف بصيغة html. القيمة الافتراضية هي true. إذا كنت ترغب في استيراد ملف html الناتج إلى إكسل، يرجى الحفاظ على القيمة الافتراضية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExportFrameScriptsAndProperties(boolean value) {#setExportFrameScriptsAndProperties-boolean-}
```
public void setExportFrameScriptsAndProperties(boolean value)
```


يشير إلى ما إذا كان يتم تصدير سكريبتات الإطار وخصائص المستند. القيمة الافتراضية هي true. إذا كنت ترغب في استيراد ملف html أو mht إلى إكسل، يرجى الحفاظ على القيمة الافتراضية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExportGridLines(boolean value) {#setExportGridLines-boolean-}
```
public void setExportGridLines(boolean value)
```


الإشارة إلى ما إذا كان يتم تصدير خطوط الشبكة. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExportHeadings(boolean value) {#setExportHeadings-boolean-}
```
public void setExportHeadings(boolean value)
```


يحدد ما إذا كان يتم تصدير عناوين الصفوف والأعمدة للورقة عند الحفظ كملفات HTML.

**Remarks**

ملاحظة: هذا العضو الآن غير صالح. بدلاً من ذلك، يرجى استخدام خاصية HtmlSaveOptions.ExportRowColumnHeadings. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExportHiddenWorksheet(boolean value) {#setExportHiddenWorksheet-boolean-}
```
public void setExportHiddenWorksheet(boolean value)
```


الإشارة إلى ما إذا كان يتم تصدير محتوى ورقة العمل المخفي. القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExportImagesAsBase64(boolean value) {#setExportImagesAsBase64-boolean-}
```
public void setExportImagesAsBase64(boolean value)
```


يحدد ما إذا كانت الصور تُحفظ بتنسيق Base64 إلى HTML أو MHTML أو EPUB.

**Remarks**

عند ضبط هذه الخاصية على true يتم تصدير بيانات الصورة مباشرةً على عناصر img ولا يتم إنشاء ملفات منفصلة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExportNamedRangeAnchors(boolean value) {#setExportNamedRangeAnchors-boolean-}
```
public void setExportNamedRangeAnchors(boolean value)
```


يشير إلى ما إذا كان يتم تصدير عناصر الربط (anchor) للنطاقات المسماة عند الحفظ بصيغة HTML. القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExportObjectListener(IExportObjectListener value) {#setExportObjectListener-com.aspose.cells.IExportObjectListener-}
```
public void setExportObjectListener(IExportObjectListener value)
```


يضبط ExportObjectListener لتصدير الكائنات.

**Remarks**

ملاحظة: هذه الخاصية الآن غير صالحة. بدلاً من ذلك، يرجى استخدام خاصية HtmlSaveOptions.IStreamProvider. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أغسطس 2015. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [IExportObjectListener](../../com.aspose.cells/iexportobjectlistener) |  |

### setExportPageFooters(boolean value) {#setExportPageFooters-boolean-}
```
public void setExportPageFooters(boolean value)
```


يحدد ما إذا كان يتم تصدير رؤوس الصفحات.

**Remarks**

يعمل فقط عندما يكون [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) هو True.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExportPageHeaders(boolean value) {#setExportPageHeaders-boolean-}
```
public void setExportPageHeaders(boolean value)
```


يحدد ما إذا كان يتم تصدير رؤوس الصفحات.

**Remarks**

يعمل فقط عندما يكون [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) هو True.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExportPrintAreaOnly(boolean value) {#setExportPrintAreaOnly-boolean-}
```
public void setExportPrintAreaOnly(boolean value)
```


يشير إلى ما إذا كان يتم تصدير منطقة الطباعة فقط إلى ملف html. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExportRowColumnHeadings(boolean value) {#setExportRowColumnHeadings-boolean-}
```
public void setExportRowColumnHeadings(boolean value)
```


يحدد ما إذا كان يتم تصدير عناوين الصفوف والأعمدة للورقة عند الحفظ كملفات HTML.

**Remarks**

القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExportSimilarBorderStyle(boolean value) {#setExportSimilarBorderStyle-boolean-}
```
public void setExportSimilarBorderStyle(boolean value)
```


يشير إلى ما إذا كان يتم تصدير نمط الحدود المشابه عندما لا يدعم المتصفحات نمط الحدود. إذا كنت ترغب في استيراد ملف html أو mht إلى إكسل، يرجى الحفاظ على القيمة الافتراضية. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExportSingleTab(boolean value) {#setExportSingleTab-boolean-}
```
public void setExportSingleTab(boolean value)
```


يشير إلى ما إذا كان يتم تصدير علامة التبويب الوحيدة عندما يحتوي الملف على ورقة عمل واحدة فقط. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExportWorkbookProperties(boolean value) {#setExportWorkbookProperties-boolean-}
```
public void setExportWorkbookProperties(boolean value)
```


الإشارة إلى ما إذا كان يتم تصدير خصائص المصنف. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html أو mht إلى Excel، يرجى الحفاظ على القيمة الافتراضية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExportWorksheetCSSSeparately(boolean value) {#setExportWorksheetCSSSeparately-boolean-}
```
public void setExportWorksheetCSSSeparately(boolean value)
```


الإشارة إلى ما إذا كان يتم تصدير CSS لورقة العمل بشكل منفصل. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExportWorksheetProperties(boolean value) {#setExportWorksheetProperties-boolean-}
```
public void setExportWorksheetProperties(boolean value)
```


الإشارة إلى ما إذا كان يتم تصدير خصائص ورقة العمل. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html أو mht إلى Excel، يرجى الحفاظ على القيمة الافتراضية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setFilePathProvider(IFilePathProvider value) {#setFilePathProvider-com.aspose.cells.IFilePathProvider-}
```
public void setFilePathProvider(IFilePathProvider value)
```


يضبط IFilePathProvider لتصدير Worksheet إلى HTML بشكل منفصل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [IFilePathProvider](../../com.aspose.cells/ifilepathprovider) |  |

### setFormatDataIgnoreColumnWidth(boolean value) {#setFormatDataIgnoreColumnWidth-boolean-}
```
public void setFormatDataIgnoreColumnWidth(boolean value)
```


يشير إلى ما إذا كان يتم عرض جميع البيانات المنسقة للخلية عندما يتجاوز النص عرض العمود. إذا كان true يتم تجاهل عرض العمود وتُصدَّر جميع بيانات الخلية. إذا كان false تُصدَّر البيانات كما في Excel. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setFullPathLink(boolean value) {#setFullPathLink-boolean-}
```
public void setFullPathLink(boolean value)
```


تشير إلى ما إذا كان سيتم استخدام رابط المسار الكامل في sheet00x.htm, filelist.xml و tabstrip.htm. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHiddenColDisplayType(int value) {#setHiddenColDisplayType-int-}
```
public void setHiddenColDisplayType(int value)
```


العمود المخفي (عرض هذا العمود هو 0) في Excel، قبل حفظه بصيغة HTML، إذا كان HtmlHiddenColDisplayType هو "Remove"، فلن يتم إخراج العمود المخفي، إذا كانت القيمة "Hidden"، سيتم إخراج العمود لكنه سيظل مخفيًا، القيمة الافتراضية هي "Hidden".

انظر [HtmlHiddenColDisplayType](../../com.aspose.cells/htmlhiddencoldisplaytype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setHiddenRowDisplayType(int value) {#setHiddenRowDisplayType-int-}
```
public void setHiddenRowDisplayType(int value)
```


الصف المخفي (ارتفاع هذا الصف هو 0) في Excel، قبل حفظه بصيغة HTML، إذا كان HtmlHiddenRowDisplayType هو "Remove"، فلن يتم إخراج الصف المخفي، إذا كانت القيمة "Hidden"، سيتم إخراج الصف لكنه سيظل مخفيًا، القيمة الافتراضية هي "Hidden".

انظر [HtmlHiddenRowDisplayType](../../com.aspose.cells/htmlhiddenrowdisplaytype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setHideOverflowWrappedText(boolean value) {#setHideOverflowWrappedText-boolean-}
```
public void setHideOverflowWrappedText(boolean value)
```


يشير إلى ما إذا كان يتم إخفاء النص المتجاوز عندما يكون تنسيق الخلية مضبوطًا على التفاف النص. القيمة الافتراضية هي false

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHtmlCrossStringType(int value) {#setHtmlCrossStringType-int-}
```
public void setHtmlCrossStringType(int value)
```


يشير إلى ما إذا كان سيتم عرض سلسلة عبر الخلايا بنفس طريقة MS Excel عند حفظ ملف Excel بصيغة html. القيمة الافتراضية هي Default، لذا بالنسبة للسلاسل عبر الخلايا، هناك فرق بسيط بين ملفات html التي تُنشئها Aspose.Cells و MS Excel. لكن الأداء لإنشاء ملفات html الكبيرة، ضبط القيمة إلى Cross سيكون أسرع عدة مرات مقارنةً بضبطها إلى Default أو Fit2Cell.

انظر [HtmlCrossType](../../com.aspose.cells/htmlcrosstype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setHtmlVersion(int value) {#setHtmlVersion-int-}
```
public void setHtmlVersion(int value)
```


يحدد نسخة معيار HTML التي يجب استخدامها عند حفظ الصيغة HTML. القيمة الافتراضية هي HtmlVersion.Default.

انظر [HtmlVersion](../../com.aspose.cells/htmlversion).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setIECompatible(boolean value) {#setIECompatible-boolean-}
```
public void setIECompatible(boolean value)
```


تشير إلى ما إذا كان HTML الناتج متوافقًا مع متصفح IE. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setIgnoreInvisibleShapes(boolean value) {#setIgnoreInvisibleShapes-boolean-}
```
public void setIgnoreInvisibleShapes(boolean value)
```


الإشارة إلى ما إذا كان يتم تصدير الأشكال غير المرئية.

**Remarks**

القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setImageScalable(boolean value) {#setImageScalable-boolean-}
```
public void setImageScalable(boolean value)
```


يشير إلى ما إذا كان يتم استخدام وحدة قابلة للتوسع لوصف عرض الصورة عند استخدام وحدة قابلة للتوسع لوصف عرض العمود. القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setJsBrowserCompatible(boolean value) {#setJsBrowserCompatible-boolean-}
```
public void setJsBrowserCompatible(boolean value)
```


يشير إلى ما إذا كان JavaScript متوافقًا مع المتصفحات التي لا تدعم JavaScript. القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setLayoutMode(int value) {#setLayoutMode-int-}
```
public void setLayoutMode(int value)
```


يضبط وضع التخطيط عند الحفظ إلى HTML. القيمة الافتراضية هي [HtmlLayoutMode.NORMAL](../../com.aspose.cells/htmllayoutmode\#NORMAL)

انظر [HtmlLayoutMode](../../com.aspose.cells/htmllayoutmode).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setLinkTargetType(int value) {#setLinkTargetType-int-}
```
public void setLinkTargetType(int value)
```


تشير إلى نوع سمة الهدف في رابط `<a>`. القيمة الافتراضية هي HtmlLinkTargetType.Parent.

انظر [HtmlLinkTargetType](../../com.aspose.cells/htmllinktargettype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

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

### setMergeEmptyTdForcely(boolean value) {#setMergeEmptyTdForcely-boolean-}
```
public void setMergeEmptyTdForcely(boolean value)
```


يشير إلى ما إذا كان سيتم دمج عنصر TD الفارغ قسراً عند تصدير الملف إلى html. سيقل حجم ملف html بشكل كبير بعد تعيين القيمة إلى true. القيمة الافتراضية هي false. إذا كنت ترغب في استيراد ملف html إلى Excel أو تصدير خطوط شبكة مثالية عند حفظ الملف إلى html، يرجى الحفاظ على القيمة الافتراضية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setMergeEmptyTdType(int value) {#setMergeEmptyTdType-int-}
```
public void setMergeEmptyTdType(int value)
```


الخيار لدمج الخلايا الفارغة المتجاورة (عناصر td الفارغة). القيمة الافتراضية هي MergeEmptyTdType.Default.

انظر [MergeEmptyTdType](../../com.aspose.cells/mergeemptytdtype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setMobileCompatible(boolean value) {#setMobileCompatible-boolean-}
```
public void setMobileCompatible(boolean value)
```


يشير إلى ما إذا كان HTML الناتج متوافقًا مع الأجهزة المحمولة. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setOfficeMathOutputMode(int value) {#setOfficeMathOutputMode-int-}
```
public void setOfficeMathOutputMode(int value)
```


يحدد كيفية تصدير كائنات OfficeMath إلى HTML، القيمة الافتراضية هي Image.

انظر [HtmlOfficeMathOutputType](../../com.aspose.cells/htmlofficemathoutputtype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPageTitle(String value) {#setPageTitle-java.lang.String-}
```
public void setPageTitle(String value)
```


عنوان صفحة html. يستخدم فقط عند حفظ إلى تدفق html.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setParseHtmlTagInCell(boolean value) {#setParseHtmlTagInCell-boolean-}
```
public void setParseHtmlTagInCell(boolean value)
```


يشير إلى ما إذا كان يجب تحليل علامة html (مثل `<div></div>`) في الخلية كقيمة خلية أم الحفاظ عليها كما هي. القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setPresentationPreference(boolean value) {#setPresentationPreference-boolean-}
```
public void setPresentationPreference(boolean value)
```


تشير إلى ما إذا كان ملف html أو mht هو تفضيل العرض. القيمة الافتراضية هي false. إذا كنت تريد الحصول على عرض أكثر جمالاً، يرجى تعيين القيمة إلى true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


يحدد ما إذا كان يتم تخزين أحدث بيانات المخطط مؤقتًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSaveAsSingleFile(boolean value) {#setSaveAsSingleFile-boolean-}
```
public void setSaveAsSingleFile(boolean value)
```


يشير إلى ما إذا كان سيتم حفظ html كملف واحد. القيمة الافتراضية هي false.

**Remarks**

إذا كان هناك عدة أوراق عمل أو موارد أخرى مطلوبة مثل الصور في المصنف، عادةً ما تحتاج تلك الأوراق والموارد إلى حفظها في ملفات منفصلة. في بعض السيناريوهات، قد يحتاج المستخدم إلى الحصول على ملف واحد فقط لتسهيل النقل. إذا كان الأمر كذلك، يمكن للمستخدم تعيين هذه الخاصية إلى true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSheetSet(SheetSet value) {#setSheetSet-com.aspose.cells.SheetSet-}
```
public void setSheetSet(SheetSet value)
```


يضبط الأوراق التي سيتم عرضها. القيمة الافتراضية هي جميع الأوراق المرئية في المصنف: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [SheetSet](../../com.aspose.cells/sheetset) |  |

### setShowAllSheets(boolean value) {#setShowAllSheets-boolean-}
```
public void setShowAllSheets(boolean value)
```


يحدد ما إذا كان يتم عرض جميع الأوراق عند حفظها كملف HTML واحد.

**Remarks**

يعمل فقط عندما يكون [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) هو True.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

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

### setSpaceMode(int value) {#setSpaceMode-int-}
```
public void setSpaceMode(int value)
```


يشير إلى كيفية عرض المسافات في مخرجات HTML. يتم تطبيق هذا الخيار حالياً فقط على التنسيقات الرقمية (مثل تنسيق المحاسبة). القيمة الافتراضية هي [HtmlSpaceMode.CSS](../../com.aspose.cells/htmlspacemode\\#CSS).

انظر [HtmlSpaceMode](../../com.aspose.cells/htmlspacemode).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setStreamProvider(IStreamProvider value) {#setStreamProvider-com.aspose.cells.IStreamProvider-}
```
public void setStreamProvider(IStreamProvider value)
```


يضبط IStreamProvider لتصدير الكائنات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setTableCssId(String value) {#setTableCssId-java.lang.String-}
```
public void setTableCssId(String value)
```


يضبط بادئة اسم نوع CSS مثل tr, col, td وما إلى ذلك، وهي موجودة في عنصر الجدول الذي يحتوي على السمة TableCssId المحددة. القيمة الافتراضية هي "".

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

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

### setWidthScalable(boolean value) {#setWidthScalable-boolean-}
```
public void setWidthScalable(boolean value)
```


يشير إلى ما إذا كان سيتم تصدير عرض العمود بوحدة المقياس إلى html. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setWorksheetScalable(boolean value) {#setWorksheetScalable-boolean-}
```
public void setWorksheetScalable(boolean value)
```


يحدد ما إذا كان يتم تكبير أو تصغير HTML عبر مستوى تكبير ورقة العمل عند حفظ الملف إلى HTML، القيمة الافتراضية هي false.

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

