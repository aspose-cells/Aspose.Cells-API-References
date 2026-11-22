---
title: "فئة EbookSaveOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Saving.EbookSaveOptions. تمثل الخيارات لحفظ ملف الكتاب الإلكتروني."
type: docs
url: /ar/net/aspose.cells.saving/ebooksaveoptions/
---
## EbookSaveOptions class

يمثل خيارات حفظ ملف ebook.

```csharp
public class EbookSaveOptions : HtmlSaveOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [EbookSaveOptions](ebooksaveoptions/#constructor)() | ينشئ خيارات لحفظ ملف الكتاب الإلكتروني. |
| [EbookSaveOptions](ebooksaveoptions/#constructor_1)(SaveFormat) | ينشئ خيارات لحفظ ملف الكتاب الإلكتروني. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AddGenericFont](../../aspose.cells/htmlsaveoptions/addgenericfont/) { get; set; } | يشير إلى ما إذا كان يجب إضافة خط عام إلى خاصية CSS font-family. القيمة الافتراضية هي true (موروثة من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [AddTooltipText](../../aspose.cells/htmlsaveoptions/addtooltiptext/) { get; set; } | يشير إلى ما إذا كان يتم إضافة نص تلميح عندما لا يمكن عرض البيانات بالكامل. القيمة الافتراضية هي false. (موروثة من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [AttachedFilesDirectory](../../aspose.cells/htmlsaveoptions/attachedfilesdirectory/) { get; set; } | الدليل الذي سيتم حفظ الملفات المرفقة فيه. يُستخدم فقط لحفظ إلى تدفق html. (موروثة من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [AttachedFilesUrlPrefix](../../aspose.cells/htmlsaveoptions/attachedfilesurlprefix/) { get; set; } | حدد بادئة Url للملفات المرفقة مثل الصورة في ملف html. يُستخدم فقط لحفظ إلى تدفق html. (موروثة من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة تخزين مؤقت للبيانات. (موروثة من [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CalculateFormula](../../aspose.cells/htmlsaveoptions/calculateformula/) { get; set; } | يشير إلى ما إذا كان يجب حساب الصيغ قبل حفظ ملف html. (موروثة من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [CellCssPrefix](../../aspose.cells/htmlsaveoptions/cellcssprefix/) { get; set; } | يحصل على ويضبط بادئة اسم css، القيمة الافتراضية هي "". (موروثة من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [CellNameAttribute](../../aspose.cells/htmlsaveoptions/cellnameattribute/) { get; set; } | يحدد السمة التي تشير إلى CellName ليتم كتابتها. (مثال: إذا كانت القيمة "id"، فبالنسبة للخلية "A1"، سيكون الناتج: &lt;td id='A1'&gt;). القيمة الافتراضية هي null. (موروثة من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | ما إذا كان يتم التحقق من قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المتعلقة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32K. عندما تُدخل قيمة أطول من 32K، سيتم قطعها. (موروثة من [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | اجعل دفتر العمل فارغًا بعد حفظ الملف. (موروثة من [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | إذا كانت true وكان الدليل غير موجود، سيتم إنشاء الدليل تلقائيًا قبل حفظ الملف. (موروثة من [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CssStyles](../../aspose.cells/htmlsaveoptions/cssstyles/) { get; set; } | يحصل على أو يضبط أنماط css الإضافية للمنسق. يعمل فقط عندما يكون [`SaveAsSingleFile`](../../aspose.cells/htmlsaveoptions/saveassinglefile/) هو True. CssStyles="body { padding: 5px }"; (موروثة من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [DataBarRenderMode](../../aspose.cells/htmlsaveoptions/databarrendermode/) { get; set; } | يمثل وضع كيفية عرض DataBar عند تحويل ملفات Excel إلى ملفات html. القيمة الافتراضية هي BackgroundColor. (موروثة من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [DefaultFontName](../../aspose.cells/htmlsaveoptions/defaultfontname/) { get; set; } | حدد اسم الخط الافتراضي لتصدير html، سيُستخدم الخط الافتراضي عندما لا يكون خط النمط موجودًا، إذا كانت هذه الخاصية null، سيستخدم Aspose.Cells خطًا عالميًا يملك نفس عائلة الخط الأصلي، القيمة الافتراضية هي null. (موروثة من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [DisableCss](../../aspose.cells/htmlsaveoptions/disablecss/) { get; set; } | يشير إلى ما إذا كانت الأنماط المضمنة فقط هي المطبقة، دون الاعتماد على CSS. القيمة الافتراضية هي false. (موروثة من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [DisableDownlevelRevealedComments](../../aspose.cells/htmlsaveoptions/disabledownlevelrevealedcomments/) { get; set; } | يشير إلى ما إذا كان يتم تعطيل التعليقات الشرطية Downlevel-revealed عند تصدير الملف إلى html، القيمة الافتراضية هي false. (موروثة من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [EmbeddedFontType](../../aspose.cells/htmlsaveoptions/embeddedfonttype/) { get; set; } | يحصل على أو يضبط نوع تضمين ملف الخط في ملف html. القيمة الافتراضية هي None والتي تشير إلى عدم تضمين أي خط في html. (موروثة من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [EnableCssCustomProperties](../../aspose.cells/htmlsaveoptions/enablecsscustomproperties/) { get; set; } | حسّن مخرجات html باستخدام خصائص CSS المخصصة. على سبيل المثال، في السيناريو الذي توجد فيه تكرارات متعددة لصورة base64 واحدة، مع الخاصية المخصصة يحتاج حفظ بيانات الصورة مرة واحدة فقط وبالتالي يمكن تحسين أداء html الناتج. القيمة الافتراضية هي false. (موروثة من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [EncodeEntityAsCode](../../aspose.cells/htmlsaveoptions/encodeentityascode/) { get; set; } | يشير إلى ما إذا كانت كيانات أحرف html تُستبدل بالرمز العشري. (مثال: "&amp;nbsp;" تُستبدل بـ "&amp;#160;"). القيمة الافتراضية هي false. (موروثة من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [Encoding](../../aspose.cells/htmlsaveoptions/encoding/) { get; set; } | إذا لم يتم الضبط، استخدم Encoding.UTF8 كنمط الترميز الافتراضي. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | يشير إلى ما إذا كان يتم تشفير خصائص المستند عند الحفظ كملف .xls. القيمة الافتراضية هي true. (موروث من [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ExcludeUnusedStyles](../../aspose.cells/htmlsaveoptions/excludeunusedstyles/) { get; set; } | يشير إلى ما إذا كان يتم استبعاد الأنماط غير المستخدمة. بالنسبة لملفات html المُولَّدة، يمكن أن يؤدي استبعاد الأنماط غير المستخدمة إلى تقليل حجم الملف دون التأثير على التأثيرات البصرية. لذلك القيمة الافتراضية لهذه الخاصية هي true. إذا كان المستخدم يحتاج إلى الاحتفاظ بجميع الأنماط في المصنف للـ html المُولَّد (مثل السيناريو الذي يحتاج فيه المستخدم إلى استعادة المصنف من الـ html المُولَّد لاحقًا)، يرجى ضبط هذه الخاصية على false. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportActiveWorksheetOnly](../../aspose.cells/htmlsaveoptions/exportactiveworksheetonly/) { get; set; } | يشير إلى ما إذا كان يتم تصدير ورقة العمل النشطة فقط إلى ملف html. إذا كانت true فستُصدَّر ورقة العمل النشطة فقط إلى ملف html؛ إذا كانت false فسيُصدَّر المصنف بالكامل إلى ملف html. القيمة الافتراضية هي false. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportArea](../../aspose.cells/htmlsaveoptions/exportarea/) { get; set; } | يحصل أو يضبط منطقة الخلايا (CellArea) المُصدَّرة لورقة العمل النشطة الحالية. إذا قمت بضبط هذا السمة، سيتم حذف منطقة الطباعة لورقة العمل النشطة الحالية. سيتم تصدير المنطقة المحددة فقط عند حفظ الملف كـ html. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportBogusRowData](../../aspose.cells/htmlsaveoptions/exportbogusrowdata/) { get; set; } | يشير إلى ما إذا كان يتم تصدير بيانات الصف السفلي الزائفة. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html أو mht إلى Excel، يرجى الحفاظ على القيمة الافتراضية. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportCellCoordinate](../../aspose.cells/htmlsaveoptions/exportcellcoordinate/) { get; set; } | يشير إلى ما إذا كان يتم تصدير إحداثيات Excel للخلايا غير الفارغة عند حفظ الملف كـ html. القيمة الافتراضية هي false. إذا كنت تريد استيراد الـ html الناتج إلى Excel، يرجى الحفاظ على القيمة الافتراضية. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportCommentsType](../../aspose.cells/htmlsaveoptions/exportcommentstype/) { get; set; } | يمثل نوع تصدير التعليقات إلى ملفات html. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportDataOptions](../../aspose.cells/htmlsaveoptions/exportdataoptions/) { get; set; } | يشير إلى قاعدة تصدير بيانات ملف html. القيمة الافتراضية هي All. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportDocumentProperties](../../aspose.cells/htmlsaveoptions/exportdocumentproperties/) { get; set; } | يشير إلى ما إذا كان يتم تصدير خصائص المستند. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html أو mht إلى Excel، يرجى الحفاظ على القيمة الافتراضية. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportExtraHeadings](../../aspose.cells/htmlsaveoptions/exportextraheadings/) { get; set; } | يشير إلى ما إذا كان يتم تصدير عناوين إضافية عندما يكون طول النص أطول من الحد الأقصى لعمود العرض. القيمة الافتراضية هي false. إذا كنت تريد استيراد ملف html إلى Excel، يرجى الحفاظ على القيمة الافتراضية. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportFormula](../../aspose.cells/htmlsaveoptions/exportformula/) { get; set; } | يشير إلى ما إذا كان يتم تصدير الصيغ عند حفظ الملف كـ html. القيمة الافتراضية هي true. إذا كنت تريد استيراد الـ html الناتج إلى Excel، يرجى الحفاظ على القيمة الافتراضية. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportFrameScriptsAndProperties](../../aspose.cells/htmlsaveoptions/exportframescriptsandproperties/) { get; set; } | يشير إلى ما إذا كان يتم تصدير سكريبتات الإطار وخصائص المستند. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html أو mht إلى Excel، يرجى الحفاظ على القيمة الافتراضية. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportGridLines](../../aspose.cells/htmlsaveoptions/exportgridlines/) { get; set; } | يشير إلى ما إذا كان يتم تصدير خطوط الشبكة. القيمة الافتراضية هي false. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportHeadings](../../aspose.cells/htmlsaveoptions/exportheadings/) { get; set; } | (**Obsolete.**) يشير إلى ما إذا كان يتم تصدير عناوين الصفوف والأعمدة للورقة عند الحفظ إلى ملفات HTML. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportHiddenWorksheet](../../aspose.cells/htmlsaveoptions/exporthiddenworksheet/) { get; set; } | يشير إلى ما إذا كان يتم تصدير محتوى ورقة العمل المخفية. القيمة الافتراضية هي true. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportImagesAsBase64](../../aspose.cells/htmlsaveoptions/exportimagesasbase64/) { get; set; } | يحدد ما إذا كانت الصور تُحفظ بتنسيق Base64 إلى HTML أو MHTML أو EPUB. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportNamedRangeAnchors](../../aspose.cells/htmlsaveoptions/exportnamedrangeanchors/) { get; set; } | يشير إلى ما إذا كان يتم تصدير عناصر الربط للنطاقات المسماة عند الحفظ كـ HTML. القيمة الافتراضية هي true. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportObjectListener](../../aspose.cells/htmlsaveoptions/exportobjectlistener/) { get; set; } | (**Obsolete.**) يحصل أو يعيّن ExportObjectListener لتصدير الكائنات. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportPageFooters](../../aspose.cells/htmlsaveoptions/exportpagefooters/) { get; set; } | يشير إلى ما إذا كان يتم تصدير رؤوس الصفحات. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportPageHeaders](../../aspose.cells/htmlsaveoptions/exportpageheaders/) { get; set; } | يشير إلى ما إذا كان يتم تصدير رؤوس الصفحات. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportPrintAreaOnly](../../aspose.cells/htmlsaveoptions/exportprintareaonly/) { get; set; } | يشير إلى ما إذا كان يتم تصدير منطقة الطباعة فقط إلى ملف html. القيمة الافتراضية هي false. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportRowColumnHeadings](../../aspose.cells/htmlsaveoptions/exportrowcolumnheadings/) { get; set; } | يشير إلى ما إذا كان يتم تصدير رؤوس الصفوف والأعمدة للورقة عند الحفظ إلى ملفات HTML. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportSimilarBorderStyle](../../aspose.cells/htmlsaveoptions/exportsimilarborderstyle/) { get; set; } | يشير إلى ما إذا كان يتم تصدير نمط الحدود المشابه عندما لا يدعم المتصفحات نمط الحدود. إذا كنت تريد استيراد ملف html أو mht إلى Excel، يرجى الحفاظ على القيمة الافتراضية. القيمة الافتراضية هي false. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportSingleTab](../../aspose.cells/htmlsaveoptions/exportsingletab/) { get; set; } | يشير إلى ما إذا كان يتم تصدير علامة التبويب الوحيدة عندما يحتوي الملف على ورقة عمل واحدة فقط. القيمة الافتراضية هي false. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportWorkbookProperties](../../aspose.cells/htmlsaveoptions/exportworkbookproperties/) { get; set; } | يشير إلى ما إذا كان يتم تصدير خصائص دفتر العمل. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html أو mht إلى Excel، يرجى الحفاظ على القيمة الافتراضية. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportWorksheetCSSSeparately](../../aspose.cells/htmlsaveoptions/exportworksheetcssseparately/) { get; set; } | يشير إلى ما إذا كان يتم تصدير CSS للورقة بشكل منفصل. القيمة الافتراضية هي false. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ExportWorksheetProperties](../../aspose.cells/htmlsaveoptions/exportworksheetproperties/) { get; set; } | يشير إلى ما إذا كان يتم تصدير خصائص الورقة. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html أو mht إلى Excel، يرجى الحفاظ على القيمة الافتراضية. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [FilePathProvider](../../aspose.cells/htmlsaveoptions/filepathprovider/) { get; set; } | يحصل أو يعيّن IFilePathProvider لتصدير Worksheet إلى html بشكل منفصل. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [FormatDataIgnoreColumnWidth](../../aspose.cells/htmlsaveoptions/formatdataignorecolumnwidth/) { get; set; } | يشير إلى ما إذا كان يتم عرض جميع البيانات المنسقة للخلية عند تجاوز العمود. إذا كان true يتم تجاهل عرض العمود وسيتم تصدير جميع بيانات الخلية. إذا كان false سيتم تصدير البيانات كما في Excel. القيمة الافتراضية هي false. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HiddenColDisplayType](../../aspose.cells/htmlsaveoptions/hiddencoldisplaytype/) { get; set; } | عمود مخفي (عرض هذا العمود هو 0) في Excel، قبل حفظه بتنسيق html، إذا كان HtmlHiddenColDisplayType هو "Remove"، لن يتم إخراج العمود المخفي، إذا كانت القيمة "Hidden"، سيتم إخراج العمود لكنه سيبقى مخفيًا، القيمة الافتراضية هي "Hidden". (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HiddenRowDisplayType](../../aspose.cells/htmlsaveoptions/hiddenrowdisplaytype/) { get; set; } | صف مخفي (ارتفاع هذا الصف هو 0) في Excel، قبل حفظه بتنسيق html، إذا كان HtmlHiddenRowDisplayType هو "Remove"، لن يتم إخراج الصف المخفي، إذا كانت القيمة "Hidden"، سيتم إخراج الصف لكنه سيبقى مخفيًا، القيمة الافتراضية هي "Hidden". (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HideOverflowWrappedText](../../aspose.cells/htmlsaveoptions/hideoverflowwrappedtext/) { get; set; } | يشير إلى ما إذا كان يتم إخفاء النص المتجاوز عندما يكون تنسيق الخلية مضبوطًا على التفاف النص. القيمة الافتراضية هي false. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HtmlCrossStringType](../../aspose.cells/htmlsaveoptions/htmlcrossstringtype/) { get; set; } | يشير إلى ما إذا كان سيتم عرض سلسلة عابرة للخلية بنفس طريقة MS Excel عند حفظ ملف Excel بتنسيق html. بشكل افتراضي القيمة هي Default، لذا بالنسبة للسلاسل العابرة للخلية، هناك فرق بسيط بين ملفات html التي أنشأتها Aspose.Cells و MS Excel. لكن الأداء لإنشاء ملفات html الكبيرة، ضبط القيمة إلى Cross سيكون أسرع عدة مرات مقارنةً بضبطها إلى Default أو Fit2Cell. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [HtmlVersion](../../aspose.cells/htmlsaveoptions/htmlversion/) { get; set; } | يحدد إصدار معيار HTML الذي يجب استخدامه عند حفظ التنسيق HTML. القيمة الافتراضية هي HtmlVersion.Default. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IgnoreInvisibleShapes](../../aspose.cells/htmlsaveoptions/ignoreinvisibleshapes/) { get; set; } | يشير إلى ما إذا كان يتم تصدير الأشكال غير المرئية. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ImageOptions](../../aspose.cells/htmlsaveoptions/imageoptions/) { get; } | احصل على كائن ImageOrPrintOptions قبل التصدير. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ImageScalable](../../aspose.cells/htmlsaveoptions/imagescalable/) { get; set; } | يشير إلى ما إذا كان يتم استخدام وحدة قابلة للتوسع لوصف عرض الصورة عند استخدام وحدة قابلة للتوسع لوصف عرض العمود. القيمة الافتراضية هي true. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsBorderCollapsed](../../aspose.cells/htmlsaveoptions/isbordercollapsed/) { get; set; } | يشير إلى ما إذا كانت حدود الجدول مدمجة. القيمة الافتراضية هي true. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsExpImageToTempDir](../../aspose.cells/htmlsaveoptions/isexpimagetotempdir/) { get; set; } | يشير إلى ما إذا كان يتم تصدير ملفات الصور إلى دليل مؤقت. يستخدم فقط عند حفظ إلى تدفق html. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsExportComments](../../aspose.cells/htmlsaveoptions/isexportcomments/) { get; set; } | يشير إلى ما إذا كان يتم تصدير التعليقات عند حفظ الملف إلى html، القيمة الافتراضية هي false. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsFullPathLink](../../aspose.cells/htmlsaveoptions/isfullpathlink/) { get; set; } | يشير إلى ما إذا كان يتم استخدام رابط المسار الكامل في sheet00x.htm، filelist.xml و tabstrip.htm. القيمة الافتراضية هي false. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsIECompatible](../../aspose.cells/htmlsaveoptions/isiecompatible/) { get; set; } | يشير إلى ما إذا كان HTML الناتج متوافقًا مع متصفح IE. القيمة الافتراضية هي false (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsJsBrowserCompatible](../../aspose.cells/htmlsaveoptions/isjsbrowsercompatible/) { get; set; } | يشير إلى ما إذا كان JavaScript متوافقًا مع المتصفحات التي لا تدعم JavaScript. القيمة الافتراضية هي true. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [IsMobileCompatible](../../aspose.cells/htmlsaveoptions/ismobilecompatible/) { get; set; } | يشير إلى ما إذا كان HTML الناتج متوافقًا مع الأجهزة المحمولة. القيمة الافتراضية هي false. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [LayoutMode](../../aspose.cells/htmlsaveoptions/layoutmode/) { get; set; } | يحصل أو يضبط وضع التخطيط عند الحفظ إلى HTML. القيمة الافتراضية هي Normal (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [LinkTargetType](../../aspose.cells/htmlsaveoptions/linktargettype/) { get; set; } | يشير إلى نوع سمة target في رابط `<a>`. القيمة الافتراضية هي HtmlLinkTargetType.Parent. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | يشير إلى ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق قبل حفظ الملف. (موروث من [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [MergeEmptyTdForcely](../../aspose.cells/htmlsaveoptions/mergeemptytdforcely/) { get; set; } | (**Obsolete.**) يشير إلى ما إذا كان يتم دمج عنصر TD الفارغ بالقوة عند تصدير الملف إلى html. سيقل حجم ملف html بشكل كبير بعد ضبط القيمة إلى true. القيمة الافتراضية هي false. إذا كنت ترغب في استيراد ملف html إلى Excel أو تصدير خطوط شبكة مثالية عند حفظ الملف إلى html، يرجى الحفاظ على القيمة الافتراضية. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [MergeEmptyTdType](../../aspose.cells/htmlsaveoptions/mergeemptytdtype/) { get; set; } | الخيار لدمج الخلايا الفارغة المتجاورة (عناصر td الفارغة). القيمة الافتراضية هي MergeEmptyTdType.Default. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [OfficeMathOutputMode](../../aspose.cells/htmlsaveoptions/officemathoutputmode/) { get; set; } | يشير إلى كيفية تصدير كائنات OfficeMath إلى HTML، القيمة الافتراضية هي Image. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [PageTitle](../../aspose.cells/htmlsaveoptions/pagetitle/) { get; set; } | عنوان صفحة html. يستخدم فقط عند حفظ إلى تدفق html. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ParseHtmlTagInCell](../../aspose.cells/htmlsaveoptions/parsehtmltagincell/) { get; set; } | يشير إلى ما إذا كان يجب تحليل علامة html (مثل `<div></div>`) في الخلية كقيمة خلية أو الحفاظ عليها كما هي. القيمة الافتراضية هي true. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [PresentationPreference](../../aspose.cells/htmlsaveoptions/presentationpreference/) { get; set; } | يشير إلى ما إذا كان ملف html أو mht هو تفضيل العرض. القيمة الافتراضية هي false. إذا كنت تريد الحصول على عرض أكثر جمالًا، يرجى ضبط القيمة إلى true. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | يشير إلى ما إذا كان يجب تخزين أحدث بيانات المخطط في الذاكرة المؤقتة. (موروث من [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SaveAsSingleFile](../../aspose.cells/htmlsaveoptions/saveassinglefile/) { get; set; } | يشير إلى ما إذا كان يتم حفظ html كملف واحد. القيمة الافتراضية هي false. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | يحصل على تنسيق ملف الحفظ. (موروث من [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SheetSet](../../aspose.cells/htmlsaveoptions/sheetset/) { get; set; } | يحصل أو يضبط الأوراق التي سيتم عرضها. الافتراضي هو جميع الأوراق المرئية في المصنف: [`Visible`](../../aspose.cells.rendering/sheetset/visible/). (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [ShowAllSheets](../../aspose.cells/htmlsaveoptions/showallsheets/) { get; set; } | يشير إلى ما إذا كان يتم عرض جميع الأوراق عند الحفظ كملف html واحد. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | يشير إلى ما إذا كان يتم فرز الأسماء المعرفة الخارجية قبل حفظ الملف. (موروث من [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | يشير إلى ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف. (موروث من [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SpaceMode](../../aspose.cells/htmlsaveoptions/spacemode/) { get; set; } | يشير إلى كيفية عرض الفراغات في مخرجات HTML. يتم تطبيق هذا الخيار حالياً فقط على التنسيقات الرقمية (مثل تنسيق المحاسبة). القيمة الافتراضية هي Css. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [StreamProvider](../../aspose.cells/htmlsaveoptions/streamprovider/) { get; set; } | يحصل أو يعيّن IStreamProvider لتصدير الكائنات. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [TableCssId](../../aspose.cells/htmlsaveoptions/tablecssid/) { get; set; } | يحصل ويعيّن بادئة اسم نوع CSS مثل tr, col, td وما إلى ذلك، وهي موجودة في عنصر الجدول الذي يحتوي على السمة TableCssId المحددة. القيمة الافتراضية هي \"\". (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | يشير إلى ما إذا كان يتم تحديث إعداد Smart Art. القيمة الافتراضية هي false. (موروث من [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | يشير إلى ما إذا كان يتم التحقق من صحة الخلايا المدمجة قبل حفظ الملف. (موروث من [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | يحصل أو يعيّن رد الاتصال للتحذير. (موروث من [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [WidthScalable](../../aspose.cells/htmlsaveoptions/widthscalable/) { get; set; } | يشير إلى ما إذا كان يتم تصدير عرض العمود بوحدة المقياس إلى HTML. القيمة الافتراضية هي false. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |
| [WorksheetScalable](../../aspose.cells/htmlsaveoptions/worksheetscalable/) { get; set; } | يشير إلى ما إذا كان يتم تكبير أو تصغير HTML عبر مستوى تكبير ورقة العمل عند حفظ الملف إلى HTML، القيمة الافتراضية هي false. (موروث من [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/).) |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class EbookSaveOptionsDemo
    {
        public static void EbookSaveOptionsExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue("Hello World");

            // إنشاء مثيل من EbookSaveOptions
            EbookSaveOptions saveOptions = new EbookSaveOptions();

            // ضبط الخصائص
            saveOptions.IgnoreInvisibleShapes = true;
            saveOptions.PageTitle = "Sample Page Title";
            saveOptions.AttachedFilesDirectory = "attached_files";
            saveOptions.AttachedFilesUrlPrefix = "http://example.com/files/";
            saveOptions.DefaultFontName = "Arial";
            saveOptions.AddGenericFont = true;
            saveOptions.WorksheetScalable = false;
            saveOptions.IsExportComments = false;
            saveOptions.ExportCommentsType = PrintCommentsType.PrintNoComments;
            saveOptions.DisableDownlevelRevealedComments = false;
            saveOptions.IsExpImageToTempDir = false;
            saveOptions.ImageScalable = true;
            saveOptions.WidthScalable = false;
            saveOptions.ExportSingleTab = false;
            saveOptions.ExportImagesAsBase64 = false;
            saveOptions.ExportActiveWorksheetOnly = false;
            saveOptions.ExportPrintAreaOnly = false;
            saveOptions.ExportArea = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            saveOptions.ParseHtmlTagInCell = true;
            saveOptions.HtmlCrossStringType = HtmlCrossType.Default;
            saveOptions.HiddenColDisplayType = HtmlHiddenColDisplayType.Hidden;
            saveOptions.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden;
            saveOptions.Encoding = System.Text.Encoding.UTF8;
            saveOptions.SaveAsSingleFile = false;
            saveOptions.ShowAllSheets = true;
            saveOptions.ExportPageHeaders = true;
            saveOptions.ExportPageFooters = true;
            saveOptions.ExportHiddenWorksheet = true;
            saveOptions.PresentationPreference = false;
            saveOptions.CellCssPrefix = "cell_";
            saveOptions.TableCssId = "table_";
            saveOptions.IsFullPathLink = false;
            saveOptions.ExportWorksheetCSSSeparately = false;
            saveOptions.ExportSimilarBorderStyle = false;
            saveOptions.MergeEmptyTdForcely = false;
            saveOptions.MergeEmptyTdType = MergeEmptyTdType.Default;
            saveOptions.ExportCellCoordinate = false;
            saveOptions.ExportExtraHeadings = false;
            saveOptions.ExportHeadings = true;
            saveOptions.ExportRowColumnHeadings = true;
            saveOptions.ExportFormula = true;
            saveOptions.AddTooltipText = false;
            saveOptions.ExportGridLines = false;
            saveOptions.ExportBogusRowData = true;
            saveOptions.ExcludeUnusedStyles = true;
            saveOptions.ExportDocumentProperties = true;
            saveOptions.ExportWorksheetProperties = true;
            saveOptions.ExportWorkbookProperties = true;
            saveOptions.ExportFrameScriptsAndProperties = true;
            saveOptions.ExportDataOptions = HtmlExportDataOptions.All;
            saveOptions.LinkTargetType = HtmlLinkTargetType.Parent;
            saveOptions.IsIECompatible = false;
            saveOptions.FormatDataIgnoreColumnWidth = false;
            saveOptions.CalculateFormula = true;
            saveOptions.IsJsBrowserCompatible = true;
            saveOptions.IsMobileCompatible = false;
            saveOptions.CssStyles = "body { padding: 5px }";
            saveOptions.HideOverflowWrappedText = false;
            saveOptions.IsBorderCollapsed = true;
            saveOptions.ClearData = true;
            saveOptions.CachedFileFolder = "cache";
            saveOptions.ValidateMergedAreas = true;
            saveOptions.MergeAreas = true;
            saveOptions.SortNames = true;
            saveOptions.SortExternalNames = true;
            saveOptions.RefreshChartCache = true;
            saveOptions.WarningCallback = null;
            saveOptions.UpdateSmartArt = true;

            // حفظ المصنف إلى ملف HTML باستخدام الخيارات المحددة
            workbook.Save("EbookSaveOptionsExample.html", saveOptions);

            return;
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../../aspose.cells/htmlsaveoptions/)
* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


