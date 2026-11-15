---
title: "فئة HtmlSaveOptions"
linktitle: "HtmlSaveOptions"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة HtmlSaveOptions. تغلف الكائن الذي يمثل htmlsaveoptions في Go."
type: docs
weight: 200
url: /ar/go-cpp/htmlsaveoptions/
---

## HtmlSaveOptions class

يمثل الخيارات لحفظ ملف html.

```go

type HtmlSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewHtmlSaveOptions](./newhtmlsaveoptions/) | ينشئ خيارات لحفظ ملف html. |
| [NewHtmlSaveOptions_SaveFormat](./newhtmlsaveoptions_saveformat/) | ينشئ خيارات لحفظ ملف htm. |
| [NewHtmlSaveOptions_SaveOptions](./newhtmlsaveoptions_saveoptions/) | يُنشئ من كائن أب. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetIgnoreInvisibleShapes](./getignoreinvisibleshapes/) | يشير إلى ما إذا كان يتم تصدير الأشكال غير المرئية |
| [SetIgnoreInvisibleShapes](./setignoreinvisibleshapes/) | يشير إلى ما إذا كان يتم تصدير الأشكال غير المرئية |
| [GetPageTitle](./getpagetitle/) | عنوان صفحة html. فقط لحفظ إلى تدفق html. |
| [SetPageTitle](./setpagetitle/) | عنوان صفحة html. فقط لحفظ إلى تدفق html. |
| [GetAttachedFilesDirectory](./getattachedfilesdirectory/) | الدليل الذي سيتم حفظ الملفات المرفقة فيه. فقط لحفظ إلى تدفق html. |
| [SetAttachedFilesDirectory](./setattachedfilesdirectory/) | الدليل الذي سيتم حفظ الملفات المرفقة فيه. فقط لحفظ إلى تدفق html. |
| [GetAttachedFilesUrlPrefix](./getattachedfilesurlprefix/) | حدد بادئة URL للملفات المرفقة مثل الصورة في ملف html. فقط لحفظ إلى تدفق html. |
| [SetAttachedFilesUrlPrefix](./setattachedfilesurlprefix/) | حدد بادئة URL للملفات المرفقة مثل الصورة في ملف html. فقط لحفظ إلى تدفق html. |
| [GetDefaultFontName](./getdefaultfontname/) | حدد اسم الخط الافتراضي لتصدير html، سيُستخدم الخط الافتراضي عندما لا يكون خط النمط موجودًا، إذا كانت هذه الخاصية فارغة (null)، سيستخدم Aspose.Cells خطًا عالميًا له نفس عائلة الخط الأصلي، القيمة الافتراضية هي null. |
| [SetDefaultFontName](./setdefaultfontname/) | حدد اسم الخط الافتراضي لتصدير html، سيُستخدم الخط الافتراضي عندما لا يكون خط النمط موجودًا، إذا كانت هذه الخاصية فارغة (null)، سيستخدم Aspose.Cells خطًا عالميًا له نفس عائلة الخط الأصلي، القيمة الافتراضية هي null. |
| [GetAddGenericFont](./getaddgenericfont/) | يشير إلى ما إذا كان سيتم إضافة خط عام إلى خاصية CSS font-family. القيمة الافتراضية هي true. |
| [SetAddGenericFont](./setaddgenericfont/) | يشير إلى ما إذا كان سيتم إضافة خط عام إلى خاصية CSS font-family. القيمة الافتراضية هي true. |
| [GetWorksheetScalable](./getworksheetscalable/) | يشير إلى ما إذا كان يتم تكبير أو تصغير ملف HTML عبر مستوى تكبير ورقة العمل عند حفظ الملف إلى HTML، القيمة الافتراضية هي false. |
| [SetWorksheetScalable](./setworksheetscalable/) | يشير إلى ما إذا كان يتم تكبير أو تصغير ملف HTML عبر مستوى تكبير ورقة العمل عند حفظ الملف إلى HTML، القيمة الافتراضية هي false. |
| [IsExportComments](./isexportcomments/) | يشير إلى ما إذا كان يتم تصدير التعليقات عند حفظ الملف إلى HTML، القيمة الافتراضية هي false. |
| [SetIsExportComments](./setisexportcomments/) | يشير إلى ما إذا كان يتم تصدير التعليقات عند حفظ الملف إلى HTML، القيمة الافتراضية هي false. |
| [GetExportCommentsType](./getexportcommentstype/) | يمثل نوع تصدير التعليقات إلى ملفات HTML. |
| [SetExportCommentsType](./setexportcommentstype/) | يمثل نوع تصدير التعليقات إلى ملفات HTML. |
| [GetDisableDownlevelRevealedComments](./getdisabledownlevelrevealedcomments/) | يشير إلى ما إذا كان يتم تعطيل التعليقات الشرطية المكشوفة للنسخ القديمة عند تصدير الملف إلى HTML، القيمة الافتراضية هي false. |
| [SetDisableDownlevelRevealedComments](./setdisabledownlevelrevealedcomments/) | يشير إلى ما إذا كان يتم تعطيل التعليقات الشرطية المكشوفة للنسخ القديمة عند تصدير الملف إلى HTML، القيمة الافتراضية هي false. |
| [IsExpImageToTempDir](./isexpimagetotempdir/) | يشير إلى ما إذا كان يتم تصدير ملفات الصور إلى دليل مؤقت. يستخدم فقط لحفظ تدفق HTML. |
| [SetIsExpImageToTempDir](./setisexpimagetotempdir/) | يشير إلى ما إذا كان يتم تصدير ملفات الصور إلى دليل مؤقت. يستخدم فقط لحفظ تدفق HTML. |
| [GetImageScalable](./getimagescalable/) | يشير إلى ما إذا كان يتم استخدام وحدة قابلة للتوسع لوصف عرض الصورة عند استخدام وحدة قابلة للتوسع لوصف عرض العمود. القيمة الافتراضية هي true. |
| [SetImageScalable](./setimagescalable/) | يشير إلى ما إذا كان يتم استخدام وحدة قابلة للتوسع لوصف عرض الصورة عند استخدام وحدة قابلة للتوسع لوصف عرض العمود. القيمة الافتراضية هي true. |
| [GetWidthScalable](./getwidthscalable/) | يشير إلى ما إذا كان يتم تصدير عرض العمود بوحدة مقياس إلى HTML. القيمة الافتراضية هي false. |
| [SetWidthScalable](./setwidthscalable/) | يشير إلى ما إذا كان يتم تصدير عرض العمود بوحدة مقياس إلى HTML. القيمة الافتراضية هي false. |
| [GetExportSingleTab](./getexportsingletab/) | يشير إلى ما إذا كان يتم تصدير التبويب الوحيد عندما يحتوي الملف على ورقة عمل واحدة فقط. القيمة الافتراضية هي false. |
| [SetExportSingleTab](./setexportsingletab/) | يشير إلى ما إذا كان يتم تصدير التبويب الوحيد عندما يحتوي الملف على ورقة عمل واحدة فقط. القيمة الافتراضية هي false. |
| [GetExportImagesAsBase64](./getexportimagesasbase64/) | يحدد ما إذا كانت الصور تُحفظ بصيغة Base64 إلى HTML أو MHTML أو EPUB. |
| [SetExportImagesAsBase64](./setexportimagesasbase64/) | يحدد ما إذا كانت الصور تُحفظ بصيغة Base64 إلى HTML أو MHTML أو EPUB. |
| [GetExportActiveWorksheetOnly](./getexportactiveworksheetonly/) | يشير إلى ما إذا كان يتم تصدير ورقة العمل النشطة فقط إلى ملف HTML. إذا كان true فستُصدَّر ورقة العمل النشطة فقط إلى ملف HTML؛ إذا كان false فسيُصدَّر المصنف بالكامل إلى ملف HTML. القيمة الافتراضية هي false. |
| [SetExportActiveWorksheetOnly](./setexportactiveworksheetonly/) | يشير إلى ما إذا كان يتم تصدير ورقة العمل النشطة فقط إلى ملف HTML. إذا كان true فستُصدَّر ورقة العمل النشطة فقط إلى ملف HTML؛ إذا كان false فسيُصدَّر المصنف بالكامل إلى ملف HTML. القيمة الافتراضية هي false. |
| [GetExportPrintAreaOnly](./getexportprintareaonly/) | يشير إلى ما إذا كان يتم تصدير منطقة الطباعة فقط إلى ملف HTML. القيمة الافتراضية هي false. |
| [SetExportPrintAreaOnly](./setexportprintareaonly/) | يشير إلى ما إذا كان يتم تصدير منطقة الطباعة فقط إلى ملف HTML. القيمة الافتراضية هي false. |
| [GetExportArea](./getexportarea/) | يحصل أو يضبط منطقة الخلية (CellArea) التي يتم تصديرها للورقة النشطة الحالية. إذا قمت بتعيين هذه الخاصية، سيتم حذف منطقة الطباعة للورقة النشطة الحالية. سيتم تصدير المنطقة المحددة فقط عند حفظ الملف إلى HTML. |
| [SetExportArea](./setexportarea/) | يحصل أو يضبط منطقة الخلية (CellArea) التي يتم تصديرها للورقة النشطة الحالية. إذا قمت بتعيين هذه الخاصية، سيتم حذف منطقة الطباعة للورقة النشطة الحالية. سيتم تصدير المنطقة المحددة فقط عند حفظ الملف إلى HTML. |
| [GetParseHtmlTagInCell](./getparsehtmltagincell/) | يشير إلى ما إذا كان يجب تحليل علامة HTML (مثل <c>&lt;div&gt;&lt;/div&gt;</c>) في الخلية كقيمة خلية أم الحفاظ عليها كما هي. القيمة الافتراضية هي true. |
| [SetParseHtmlTagInCell](./setparsehtmltagincell/) | يشير إلى ما إذا كان يجب تحليل علامة HTML (مثل <c>&lt;div&gt;&lt;/div&gt;</c>) في الخلية كقيمة خلية أم الحفاظ عليها كما هي. القيمة الافتراضية هي true. |
| [GetHtmlCrossStringType](./gethtmlcrossstringtype/) | يشير إلى ما إذا كان سيتم عرض سلسلة عبر خلايا بنفس طريقة MS Excel عند حفظ ملف Excel بصيغة HTML. القيمة الافتراضية هي Default، لذا بالنسبة للسلاسل عبر الخلايا، هناك فرق بسيط بين ملفات HTML التي تُنشئها Aspose.Cells و MS Excel. ولكن الأداء لإنشاء ملفات HTML كبيرة، ضبط القيمة إلى Cross سيكون أسرع عدة مرات مقارنةً بضبطها إلى Default أو Fit2Cell. |
| [SetHtmlCrossStringType](./sethtmlcrossstringtype/) | يشير إلى ما إذا كان سيتم عرض سلسلة عبر خلايا بنفس طريقة MS Excel عند حفظ ملف Excel بصيغة HTML. القيمة الافتراضية هي Default، لذا بالنسبة للسلاسل عبر الخلايا، هناك فرق بسيط بين ملفات HTML التي تُنشئها Aspose.Cells و MS Excel. ولكن الأداء لإنشاء ملفات HTML كبيرة، ضبط القيمة إلى Cross سيكون أسرع عدة مرات مقارنةً بضبطها إلى Default أو Fit2Cell. |
| [GetHiddenColDisplayType](./gethiddencoldisplaytype/) | العمود المخفي (عرض هذا العمود هو 0) في Excel، قبل حفظه بصيغة HTML، إذا كان HtmlHiddenColDisplayType يساوي "Remove"، لن يتم إخراج العمود المخفي؛ إذا كانت القيمة "Hidden"، سيتم إخراج العمود لكنه سيظل مخفيًا، القيمة الافتراضية هي "Hidden". |
| [SetHiddenColDisplayType](./sethiddencoldisplaytype/) | العمود المخفي (عرض هذا العمود هو 0) في Excel، قبل حفظه بصيغة HTML، إذا كان HtmlHiddenColDisplayType يساوي "Remove"، لن يتم إخراج العمود المخفي؛ إذا كانت القيمة "Hidden"، سيتم إخراج العمود لكنه سيظل مخفيًا، القيمة الافتراضية هي "Hidden". |
| [GetHiddenRowDisplayType](./gethiddenrowdisplaytype/) | الصف المخفي (ارتفاع هذا الصف هو 0) في Excel، قبل حفظه بصيغة HTML، إذا كان HtmlHiddenRowDisplayType يساوي "Remove"، لن يتم إخراج الصف المخفي؛ إذا كانت القيمة "Hidden"، سيتم إخراج الصف لكنه سيظل مخفيًا، القيمة الافتراضية هي "Hidden". |
| [SetHiddenRowDisplayType](./sethiddenrowdisplaytype/) | الصف المخفي (ارتفاع هذا الصف هو 0) في Excel، قبل حفظه بصيغة HTML، إذا كان HtmlHiddenRowDisplayType يساوي "Remove"، لن يتم إخراج الصف المخفي؛ إذا كانت القيمة "Hidden"، سيتم إخراج الصف لكنه سيظل مخفيًا، القيمة الافتراضية هي "Hidden". |
| [GetEncoding](./getencoding/) | إذا لم يتم تحديده، يُستخدم Encoding.UTF8 كنوع الترميز الافتراضي. |
| [SetEncoding](./setencoding/) | إذا لم يتم تحديده، يُستخدم Encoding.UTF8 كنوع الترميز الافتراضي. |
| [GetImageOptions](./getimageoptions/) | احصل على كائن ImageOrPrintOptions قبل التصدير |
| [GetSaveAsSingleFile](./getsaveassinglefile/) | يشير إلى ما إذا كان يتم حفظ HTML كملف واحد. القيمة الافتراضية هي false. |
| [SetSaveAsSingleFile](./setsaveassinglefile/) | يشير إلى ما إذا كان يتم حفظ HTML كملف واحد. القيمة الافتراضية هي false. |
| [GetShowAllSheets](./getshowallsheets/) | يشير إلى ما إذا كان يتم عرض جميع الأوراق عند حفظها كملف HTML واحد. |
| [SetShowAllSheets](./setshowallsheets/) | يشير إلى ما إذا كان يتم عرض جميع الأوراق عند حفظها كملف HTML واحد. |
| [GetExportPageHeaders](./getexportpageheaders/) | يشير إلى ما إذا كان يتم تصدير رؤوس الصفحات. |
| [SetExportPageHeaders](./setexportpageheaders/) | يشير إلى ما إذا كان يتم تصدير رؤوس الصفحات. |
| [GetExportPageFooters](./getexportpagefooters/) | يشير إلى ما إذا كان يتم تصدير رؤوس الصفحات. |
| [SetExportPageFooters](./setexportpagefooters/) | يشير إلى ما إذا كان يتم تصدير رؤوس الصفحات. |
| [GetExportHiddenWorksheet](./getexporthiddenworksheet/) | يشير إلى ما إذا كان يتم تصدير محتوى ورقة العمل المخفية. القيمة الافتراضية هي true. |
| [SetExportHiddenWorksheet](./setexporthiddenworksheet/) | يشير إلى ما إذا كان يتم تصدير محتوى ورقة العمل المخفية. القيمة الافتراضية هي true. |
| [GetPresentationPreference](./getpresentationpreference/) | يشير إلى ما إذا كان ملف HTML أو MHT هو تفضيل العرض. القيمة الافتراضية هي false. إذا كنت تريد الحصول على عرض أكثر جمالًا، يرجى ضبط القيمة إلى true. |
| [SetPresentationPreference](./setpresentationpreference/) | يشير إلى ما إذا كان ملف HTML أو MHT هو تفضيل العرض. القيمة الافتراضية هي false. إذا كنت تريد الحصول على عرض أكثر جمالًا، يرجى ضبط القيمة إلى true. |
| [GetCellCssPrefix](./getcellcssprefix/) | يحصل ويضبط بادئة اسم CSS، القيمة الافتراضية هي "". |
| [SetCellCssPrefix](./setcellcssprefix/) | يحصل ويضبط بادئة اسم CSS، القيمة الافتراضية هي "". |
| [GetTableCssId](./gettablecssid/) | يحصل ويضبط بادئة اسم CSS للنوع مثل tr, col, td وما إلى ذلك، وهي موجودة في عنصر الجدول الذي يحتوي على السمة TableCssId المحددة. القيمة الافتراضية هي "". |
| [SetTableCssId](./settablecssid/) | يحصل ويضبط بادئة اسم CSS للنوع مثل tr, col, td وما إلى ذلك، وهي موجودة في عنصر الجدول الذي يحتوي على السمة TableCssId المحددة. القيمة الافتراضية هي "". |
| [IsFullPathLink](./isfullpathlink/) | تشير إلى ما إذا كان يتم استخدام رابط المسار الكامل في sheet00x.htm،filelist.xml و tabstrip.htm. القيمة الافتراضية هي false. |
| [SetIsFullPathLink](./setisfullpathlink/) | تشير إلى ما إذا كان يتم استخدام رابط المسار الكامل في sheet00x.htm،filelist.xml و tabstrip.htm. القيمة الافتراضية هي false. |
| [GetExportWorksheetCSSSeparately](./getexportworksheetcssseparately/) | تشير إلى ما إذا كان يتم تصدير CSS ورقة العمل بشكل منفصل. القيمة الافتراضية هي false. |
| [SetExportWorksheetCSSSeparately](./setexportworksheetcssseparately/) | تشير إلى ما إذا كان يتم تصدير CSS ورقة العمل بشكل منفصل. القيمة الافتراضية هي false. |
| [GetExportSimilarBorderStyle](./getexportsimilarborderstyle/) | تشير إلى ما إذا كان يتم تصدير نمط الحدود المشابه عندما لا يدعم المتصفحات نمط الحدود. إذا كنت تريد استيراد ملف html أو mht إلى Excel، يرجى الحفاظ على القيمة الافتراضية. القيمة الافتراضية هي false. |
| [SetExportSimilarBorderStyle](./setexportsimilarborderstyle/) | تشير إلى ما إذا كان يتم تصدير نمط الحدود المشابه عندما لا يدعم المتصفحات نمط الحدود. إذا كنت تريد استيراد ملف html أو mht إلى Excel، يرجى الحفاظ على القيمة الافتراضية. القيمة الافتراضية هي false. |
| [GetMergeEmptyTdType](./getmergeemptytdtype/) | الخيار لدمج الخلايا الفارغة المتجاورة (عناصر td الفارغة). القيمة الافتراضية هي MergeEmptyTdType.Default. |
| [SetMergeEmptyTdType](./setmergeemptytdtype/) | الخيار لدمج الخلايا الفارغة المتجاورة (عناصر td الفارغة). القيمة الافتراضية هي MergeEmptyTdType.Default. |
| [GetExportCellCoordinate](./getexportcellcoordinate/) | تشير إلى ما إذا كان يتم تصدير إحداثيات Excel للخلايا غير الفارغة عند حفظ الملف كـ html. القيمة الافتراضية هي false. إذا كنت تريد استيراد ملف html الناتج إلى Excel، يرجى الحفاظ على القيمة الافتراضية. |
| [SetExportCellCoordinate](./setexportcellcoordinate/) | تشير إلى ما إذا كان يتم تصدير إحداثيات Excel للخلايا غير الفارغة عند حفظ الملف كـ html. القيمة الافتراضية هي false. إذا كنت تريد استيراد ملف html الناتج إلى Excel، يرجى الحفاظ على القيمة الافتراضية. |
| [GetExportExtraHeadings](./getexportextraheadings/) | تشير إلى ما إذا كان يتم تصدير رؤوس إضافية عندما يكون طول النص أطول من الحد الأقصى لعرض العمود. القيمة الافتراضية هي false. إذا كنت تريد استيراد ملف html إلى Excel، يرجى الحفاظ على القيمة الافتراضية. |
| [SetExportExtraHeadings](./setexportextraheadings/) | تشير إلى ما إذا كان يتم تصدير رؤوس إضافية عندما يكون طول النص أطول من الحد الأقصى لعرض العمود. القيمة الافتراضية هي false. إذا كنت تريد استيراد ملف html إلى Excel، يرجى الحفاظ على القيمة الافتراضية. |
| [GetExportRowColumnHeadings](./getexportrowcolumnheadings/) | تشير إلى ما إذا كان يتم تصدير رؤوس الصفوف والأعمدة للورقة عند الحفظ كملفات HTML. |
| [SetExportRowColumnHeadings](./setexportrowcolumnheadings/) | تشير إلى ما إذا كان يتم تصدير رؤوس الصفوف والأعمدة للورقة عند الحفظ كملفات HTML. |
| [GetExportFormula](./getexportformula/) | تشير إلى ما إذا كان يتم تصدير الصيغ عند حفظ الملف كـ html. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html الناتج إلى Excel، يرجى الحفاظ على القيمة الافتراضية. |
| [SetExportFormula](./setexportformula/) | تشير إلى ما إذا كان يتم تصدير الصيغ عند حفظ الملف كـ html. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html الناتج إلى Excel، يرجى الحفاظ على القيمة الافتراضية. |
| [GetAddTooltipText](./getaddtooltiptext/) | تشير إلى ما إذا كان يتم إضافة نص تلميح الأدوات عندما لا يمكن عرض البيانات بالكامل. القيمة الافتراضية هي false. |
| [SetAddTooltipText](./setaddtooltiptext/) | تشير إلى ما إذا كان يتم إضافة نص تلميح الأدوات عندما لا يمكن عرض البيانات بالكامل. القيمة الافتراضية هي false. |
| [GetExportGridLines](./getexportgridlines/) | تشير إلى ما إذا كان يتم تصدير خطوط الشبكة. القيمة الافتراضية هي false. |
| [SetExportGridLines](./setexportgridlines/) | تشير إلى ما إذا كان يتم تصدير خطوط الشبكة. القيمة الافتراضية هي false. |
| [GetExportBogusRowData](./getexportbogusrowdata/) | تشير إلى ما إذا كان يتم تصدير بيانات الصف السفلي الزائفة. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html أو mht إلى Excel، يرجى الحفاظ على القيمة الافتراضية. |
| [SetExportBogusRowData](./setexportbogusrowdata/) | تشير إلى ما إذا كان يتم تصدير بيانات الصف السفلي الزائفة. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html أو mht إلى Excel، يرجى الحفاظ على القيمة الافتراضية. |
| [GetExcludeUnusedStyles](./getexcludeunusedstyles/) | تشير إلى ما إذا كان يتم استبعاد الأنماط غير المستخدمة. بالنسبة لملفات html المولدة، يمكن أن يجعل استبعاد الأنماط غير المستخدمة حجم الملف أصغر دون التأثير على التأثيرات البصرية. لذلك القيمة الافتراضية لهذه الخاصية هي true. إذا كان المستخدم يحتاج إلى الحفاظ على جميع الأنماط في المصنف للملف html المولد (مثل السيناريو الذي يحتاج فيه المستخدم إلى استعادة المصنف من html المولد لاحقًا)، يرجى ضبط هذه الخاصية إلى false. |
| [SetExcludeUnusedStyles](./setexcludeunusedstyles/) | تشير إلى ما إذا كان يتم استبعاد الأنماط غير المستخدمة. بالنسبة لملفات html المولدة، يمكن أن يجعل استبعاد الأنماط غير المستخدمة حجم الملف أصغر دون التأثير على التأثيرات البصرية. لذلك القيمة الافتراضية لهذه الخاصية هي true. إذا كان المستخدم يحتاج إلى الحفاظ على جميع الأنماط في المصنف للملف html المولد (مثل السيناريو الذي يحتاج فيه المستخدم إلى استعادة المصنف من html المولد لاحقًا)، يرجى ضبط هذه الخاصية إلى false. |
| [GetExportDocumentProperties](./getexportdocumentproperties/) | تشير إلى ما إذا كان يتم تصدير خصائص المستند. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html أو mht إلى Excel، يرجى الحفاظ على القيمة الافتراضية. |
| [SetExportDocumentProperties](./setexportdocumentproperties/) | تشير إلى ما إذا كان يتم تصدير خصائص المستند. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html أو mht إلى Excel، يرجى الحفاظ على القيمة الافتراضية. |
| [GetExportWorksheetProperties](./getexportworksheetproperties/) | تشير إلى ما إذا كان يتم تصدير خصائص ورقة العمل. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html أو mht إلى Excel، يرجى الحفاظ على القيمة الافتراضية. |
| [SetExportWorksheetProperties](./setexportworksheetproperties/) | تشير إلى ما إذا كان يتم تصدير خصائص ورقة العمل. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html أو mht إلى Excel، يرجى الحفاظ على القيمة الافتراضية. |
| [GetExportWorkbookProperties](./getexportworkbookproperties/) | تشير إلى ما إذا كان يتم تصدير خصائص المصنف. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html أو mht إلى Excel، يرجى الحفاظ على القيمة الافتراضية. |
| [SetExportWorkbookProperties](./setexportworkbookproperties/) | تشير إلى ما إذا كان يتم تصدير خصائص المصنف. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html أو mht إلى Excel، يرجى الحفاظ على القيمة الافتراضية. |
| [GetExportFrameScriptsAndProperties](./getexportframescriptsandproperties/) | تشير إلى ما إذا كان يتم تصدير سكريبتات الإطار وخصائص المستند. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html أو mht إلى Excel، يرجى الحفاظ على القيمة الافتراضية. |
| [SetExportFrameScriptsAndProperties](./setexportframescriptsandproperties/) | تشير إلى ما إذا كان يتم تصدير سكريبتات الإطار وخصائص المستند. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html أو mht إلى Excel، يرجى الحفاظ على القيمة الافتراضية. |
| [GetExportDataOptions](./getexportdataoptions/) | تشير إلى قاعدة تصدير بيانات ملف html. القيمة الافتراضية هي All. |
| [SetExportDataOptions](./setexportdataoptions/) | تشير إلى قاعدة تصدير بيانات ملف html. القيمة الافتراضية هي All. |
| [GetLinkTargetType](./getlinktargettype/) | تشير إلى نوع سمة target في رابط <c>&lt;a&gt;</c>. القيمة الافتراضية هي HtmlLinkTargetType.Parent. |
| [SetLinkTargetType](./setlinktargettype/) | تشير إلى نوع سمة target في رابط <c>&lt;a&gt;</c>. القيمة الافتراضية هي HtmlLinkTargetType.Parent. |
| [IsIECompatible](./isiecompatible/) | تشير إلى ما إذا كان HTML الناتج متوافقًا مع متصفح IE. القيمة الافتراضية هي false. |
| [SetIsIECompatible](./setisiecompatible/) | تشير إلى ما إذا كان HTML الناتج متوافقًا مع متصفح IE. القيمة الافتراضية هي false. |
| [GetFormatDataIgnoreColumnWidth](./getformatdataignorecolumnwidth/) | تشير إلى ما إذا كان يتم عرض جميع البيانات المنسقة للخلية عندما يتجاوز العمود. إذا كان true يتم تجاهل عرض العمود وسيتم تصدير جميع بيانات الخلية. إذا كان false سيتم تصدير البيانات كما في Excel. القيمة الافتراضية هي false. |
| [SetFormatDataIgnoreColumnWidth](./setformatdataignorecolumnwidth/) | تشير إلى ما إذا كان يتم عرض جميع البيانات المنسقة للخلية عندما يتجاوز العمود. إذا كان true يتم تجاهل عرض العمود وسيتم تصدير جميع بيانات الخلية. إذا كان false سيتم تصدير البيانات كما في Excel. القيمة الافتراضية هي false. |
| [GetCalculateFormula](./getcalculateformula/) | تشير إلى ما إذا كان يتم حساب الصيغ قبل حفظ ملف html. |
| [SetCalculateFormula](./setcalculateformula/) | تشير إلى ما إذا كان يتم حساب الصيغ قبل حفظ ملف html. |
| [IsJsBrowserCompatible](./isjsbrowsercompatible/) | تشير إلى ما إذا كان JavaScript متوافقًا مع المتصفحات التي لا تدعم JavaScript. القيمة الافتراضية هي true. |
| [SetIsJsBrowserCompatible](./setisjsbrowsercompatible/) | تشير إلى ما إذا كان JavaScript متوافقًا مع المتصفحات التي لا تدعم JavaScript. القيمة الافتراضية هي true. |
| [IsMobileCompatible](./ismobilecompatible/) | تشير إلى ما إذا كان HTML الناتج متوافقًا مع الأجهزة المحمولة. القيمة الافتراضية هي false. |
| [SetIsMobileCompatible](./setismobilecompatible/) | تشير إلى ما إذا كان HTML الناتج متوافقًا مع الأجهزة المحمولة. القيمة الافتراضية هي false. |
| [GetCssStyles](./getcssstyles/) | يحصل أو يعيّن أنماط CSS الإضافية للمنسق. يعمل فقط عندما تكون SaveAsSingleFile هي True. |
| [SetCssStyles](./setcssstyles/) | يحصل أو يعيّن أنماط CSS الإضافية للمنسق. يعمل فقط عندما تكون SaveAsSingleFile هي True. |
| [GetHideOverflowWrappedText](./gethideoverflowwrappedtext/) | تشير إلى ما إذا كان يتم إخفاء النص المتجاوز عندما يكون تنسيق الخلية مضبوطًا على التفاف النص. القيمة الافتراضية هي false |
| [SetHideOverflowWrappedText](./sethideoverflowwrappedtext/) | تشير إلى ما إذا كان يتم إخفاء النص المتجاوز عندما يكون تنسيق الخلية مضبوطًا على التفاف النص. القيمة الافتراضية هي false |
| [IsBorderCollapsed](./isbordercollapsed/) | يشير إلى ما إذا كانت حدود الجدول مدمجة. القيمة الافتراضية هي true. |
| [SetIsBorderCollapsed](./setisbordercollapsed/) | يشير إلى ما إذا كانت حدود الجدول مدمجة. القيمة الافتراضية هي true. |
| [GetEncodeEntityAsCode](./getencodeentityascode/) | يشير إلى ما إذا كانت كيانات الأحرف html يتم استبدالها بالرمز العشري. (مثال: "&amp;nbsp;" يتم استبداله بـ "&amp;#160;"). القيمة الافتراضية هي false. |
| [SetEncodeEntityAsCode](./setencodeentityascode/) | يشير إلى ما إذا كانت كيانات الأحرف html يتم استبدالها بالرمز العشري. (مثال: "&amp;nbsp;" يتم استبداله بـ "&amp;#160;"). القيمة الافتراضية هي false. |
| [GetOfficeMathOutputMode](./getofficemathoutputmode/) | يشير إلى كيفية تصدير كائنات OfficeMath إلى HTML. القيمة الافتراضية هي Image. |
| [SetOfficeMathOutputMode](./setofficemathoutputmode/) | يشير إلى كيفية تصدير كائنات OfficeMath إلى HTML. القيمة الافتراضية هي Image. |
| [GetCellNameAttribute](./getcellnameattribute/) | يحدد السمة التي تشير إلى اسم الخلية CellName ليتم كتابتها. (مثال: إذا كانت القيمة "id"، فإن الخلية "A1" سيصبح الناتج: &lt;td id='A1'&gt;). القيمة الافتراضية هي null. |
| [SetCellNameAttribute](./setcellnameattribute/) | يحدد السمة التي تشير إلى اسم الخلية CellName ليتم كتابتها. (مثال: إذا كانت القيمة "id"، فإن الخلية "A1" سيصبح الناتج: &lt;td id='A1'&gt;). القيمة الافتراضية هي null. |
| [GetDisableCss](./getdisablecss/) | يشير إلى ما إذا كانت الأنماط المضمنة فقط تُطبق، دون الاعتماد على CSS. القيمة الافتراضية هي false. |
| [SetDisableCss](./setdisablecss/) | يشير إلى ما إذا كانت الأنماط المضمنة فقط تُطبق، دون الاعتماد على CSS. القيمة الافتراضية هي false. |
| [GetEnableCssCustomProperties](./getenablecsscustomproperties/) | تحسين مخرجات html باستخدام خصائص CSS المخصصة. على سبيل المثال، في حالة وجود تكرارات متعددة لصورة base64 واحدة، مع الخاصية المخصصة تحتاج بيانات الصورة إلى الحفظ مرة واحدة فقط وبالتالي يمكن تحسين أداء html الناتج. القيمة الافتراضية هي false. |
| [SetEnableCssCustomProperties](./setenablecsscustomproperties/) | تحسين مخرجات html باستخدام خصائص CSS المخصصة. على سبيل المثال، في حالة وجود تكرارات متعددة لصورة base64 واحدة، مع الخاصية المخصصة تحتاج بيانات الصورة إلى الحفظ مرة واحدة فقط وبالتالي يمكن تحسين أداء html الناتج. القيمة الافتراضية هي false. |
| [GetHtmlVersion](./gethtmlversion/) | يحدد نسخة معيار HTML التي يجب استخدامها عند حفظ تنسيق HTML. القيمة الافتراضية هي HtmlVersion.Default. |
| [SetHtmlVersion](./sethtmlversion/) | يحدد نسخة معيار HTML التي يجب استخدامها عند حفظ تنسيق HTML. القيمة الافتراضية هي HtmlVersion.Default. |
| [GetSheetSet](./getsheetset/) | يحصل أو يعيّن الأوراق التي سيتم تصييرها. الافتراضي هو جميع الأوراق المرئية في دفتر العمل: Aspose.Cells.Rendering.SheetSet.Visible. |
| [SetSheetSet](./setsheetset/) | يحصل أو يعيّن الأوراق التي سيتم تصييرها. الافتراضي هو جميع الأوراق المرئية في دفتر العمل: Aspose.Cells.Rendering.SheetSet.Visible. |
| [GetLayoutMode](./getlayoutmode/) | يحصل أو يعيّن وضع التخطيط عند الحفظ إلى HTML. القيمة الافتراضية هي HtmlLayoutMode.Normal |
| [SetLayoutMode](./setlayoutmode/) | يحصل أو يعيّن وضع التخطيط عند الحفظ إلى HTML. القيمة الافتراضية هي HtmlLayoutMode.Normal |
| [GetEmbeddedFontType](./getembeddedfonttype/) | يحصل أو يعيّن نوع تضمين ملف الخط في ملف html. القيمة الافتراضية هي HtmlEmbeddedFontType.None التي تشير إلى عدم تضمين أي خط في html. |
| [SetEmbeddedFontType](./setembeddedfonttype/) | يحصل أو يعيّن نوع تضمين ملف الخط في ملف html. القيمة الافتراضية هي HtmlEmbeddedFontType.None التي تشير إلى عدم تضمين أي خط في html. |
| [GetExportNamedRangeAnchors](./getexportnamedrangeanchors/) | يشير إلى ما إذا كان سيتم تصدير عناصر الربط (anchor) للنطاقات المسماة عند الحفظ كـ HTML. القيمة الافتراضية هي true. |
| [SetExportNamedRangeAnchors](./setexportnamedrangeanchors/) | يشير إلى ما إذا كان سيتم تصدير عناصر الربط (anchor) للنطاقات المسماة عند الحفظ كـ HTML. القيمة الافتراضية هي true. |
| [GetDataBarRenderMode](./getdatabarrendermode/) | يمثل وضع كيفية عرض DataBar عند تحويل ملفات Excel إلى ملفات html. القيمة الافتراضية هي DataBarRenderMode.BackgroundColor. |
| [SetDataBarRenderMode](./setdatabarrendermode/) | يمثل وضع كيفية عرض DataBar عند تحويل ملفات Excel إلى ملفات html. القيمة الافتراضية هي DataBarRenderMode.BackgroundColor. |
| [GetSpaceMode](./getspacemode/) | يشير إلى كيفية عرض المسافات في مخرجات HTML. هذا الخيار يُطبق حالياً فقط على الصيغ الرقمية (مثال: صيغة المحاسبة). القيمة الافتراضية هي HtmlSpaceMode.Css. |
| [SetSpaceMode](./setspacemode/) | يشير إلى كيفية عرض المسافات في مخرجات HTML. هذا الخيار يُطبق حالياً فقط على الصيغ الرقمية (مثال: صيغة المحاسبة). القيمة الافتراضية هي HtmlSpaceMode.Css. |
| [GetSaveFormat](./getsaveformat/) | يحصل على تنسيق ملف الحفظ. |
| [GetClearData](./getcleardata/) | اجعل دفتر العمل فارغًا بعد حفظ الملف. |
| [SetClearData](./setcleardata/) | اجعل دفتر العمل فارغًا بعد حفظ الملف. |
| [GetCachedFileFolder](./getcachedfilefolder/) | المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة مؤقتة للبيانات. |
| [SetCachedFileFolder](./setcachedfilefolder/) | المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة مؤقتة للبيانات. |
| [GetValidateMergedAreas](./getvalidatemergedareas/) | يشير إلى ما إذا كان يتم التحقق من صحة الخلايا المدمجة قبل حفظ الملف. |
| [SetValidateMergedAreas](./setvalidatemergedareas/) | يشير إلى ما إذا كان يتم التحقق من صحة الخلايا المدمجة قبل حفظ الملف. |
| [GetMergeAreas](./getmergeareas/) | يشير إلى ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق قبل حفظ الملف. |
| [SetMergeAreas](./setmergeareas/) | يشير إلى ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق قبل حفظ الملف. |
| [GetCreateDirectory](./getcreatedirectory/) | إذا كان صحيحًا ولم يكن الدليل موجودًا، سيتم إنشاء الدليل تلقائيًا قبل حفظ الملف. |
| [SetCreateDirectory](./setcreatedirectory/) | إذا كان صحيحًا ولم يكن الدليل موجودًا، سيتم إنشاء الدليل تلقائيًا قبل حفظ الملف. |
| [GetSortNames](./getsortnames/) | يشير إلى ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف. |
| [SetSortNames](./setsortnames/) | يشير إلى ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف. |
| [GetSortExternalNames](./getsortexternalnames/) | يشير إلى ما إذا كان يتم فرز الأسماء المعرفة الخارجية قبل حفظ الملف. |
| [SetSortExternalNames](./setsortexternalnames/) | يشير إلى ما إذا كان يتم فرز الأسماء المعرفة الخارجية قبل حفظ الملف. |
| [GetRefreshChartCache](./getrefreshchartcache/) | يشير إلى ما إذا كان يتم تخزين أحدث بيانات المخطط مؤقتًا. |
| [SetRefreshChartCache](./setrefreshchartcache/) | يشير إلى ما إذا كان يتم تخزين أحدث بيانات المخطط مؤقتًا. |
| [GetCheckExcelRestriction](./getcheckexcelrestriction/) | ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المرتبطة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32 كيلوبايت. عندما تقوم بإدخال قيمة أطول من 32 كيلوبايت، سيتم قطعها. |
| [SetCheckExcelRestriction](./setcheckexcelrestriction/) | ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المرتبطة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32 كيلوبايت. عندما تقوم بإدخال قيمة أطول من 32 كيلوبايت، سيتم قطعها. |
| [GetUpdateSmartArt](./getupdatesmartart/) | يشير إلى ما إذا كان يتم تحديث إعدادات Smart Art. القيمة الافتراضية هي false. |
| [SetUpdateSmartArt](./setupdatesmartart/) | يشير إلى ما إذا كان يتم تحديث إعدادات Smart Art. القيمة الافتراضية هي false. |
| [GetEncryptDocumentProperties](./getencryptdocumentproperties/) | يشير إلى ما إذا كان يتم تشفير خصائص المستند عند الحفظ كملف .xls. القيمة الافتراضية هي true. |
| [SetEncryptDocumentProperties](./setencryptdocumentproperties/) | يشير إلى ما إذا كان يتم تشفير خصائص المستند عند الحفظ كملف .xls. القيمة الافتراضية هي true. |
