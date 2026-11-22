---
title: "الفئة HtmlSaveOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.HtmlSaveOptions. تمثل الخيارات لحفظ ملف html"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/
---
## HtmlSaveOptions class

يمثل الخيارات لحفظ ملف HTML.

```csharp
public class HtmlSaveOptions : SaveOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions/#constructor)() | ينشئ خيارات لحفظ ملف html. |
| [HtmlSaveOptions](htmlsaveoptions/#constructor_1)(SaveFormat) | ينشئ خيارات لحفظ ملف htm. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AddGenericFont](../../aspose.cells/htmlsaveoptions/addgenericfont/) { get; set; } | يشير إلى ما إذا كان يجب إضافة خط عام إلى خاصية CSS font-family. القيمة الافتراضية هي true |
| [AddTooltipText](../../aspose.cells/htmlsaveoptions/addtooltiptext/) { get; set; } | يشير إلى ما إذا كان يتم إضافة نص تلميح عندما لا يمكن عرض البيانات بالكامل. القيمة الافتراضية هي false. |
| [AttachedFilesDirectory](../../aspose.cells/htmlsaveoptions/attachedfilesdirectory/) { get; set; } | الدليل الذي سيتم حفظ الملفات المرفقة فيه. يُستخدم فقط لحفظ تدفق html. |
| [AttachedFilesUrlPrefix](../../aspose.cells/htmlsaveoptions/attachedfilesurlprefix/) { get; set; } | حدد بادئة Url للملفات المرفقة مثل الصورة في ملف html. يُستخدم فقط لحفظ تدفق html. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة مؤقتة للبيانات. (موروث من [`SaveOptions`](../saveoptions/).) |
| [CalculateFormula](../../aspose.cells/htmlsaveoptions/calculateformula/) { get; set; } | يشير إلى ما إذا كان يجب حساب الصيغ قبل حفظ ملف html. |
| [CellCssPrefix](../../aspose.cells/htmlsaveoptions/cellcssprefix/) { get; set; } | يحصل على ويضبط بادئة اسم css، القيمة الافتراضية هي "". |
| [CellNameAttribute](../../aspose.cells/htmlsaveoptions/cellnameattribute/) { get; set; } | يحدد السمة التي تشير إلى CellName التي سيتم كتابتها. (مثال: إذا كانت القيمة "id"، فبالنسبة للخلية "A1" سيكون الناتج:&lt;td id='A1'&gt;). القيمة الافتراضية هي null. |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | ما إذا كان يتم فحص قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المتعلقة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32K. عندما تُدخل قيمة أطول من 32K، سيتم قطعها. (موروث من [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | اجعل دفتر العمل فارغًا بعد حفظ الملف. (موروث من [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | إذا كان صحيحًا ولم يكن الدليل موجودًا، سيتم إنشاء الدليل تلقائيًا قبل حفظ الملف. (موروث من [`SaveOptions`](../saveoptions/).) |
| [CssStyles](../../aspose.cells/htmlsaveoptions/cssstyles/) { get; set; } | يحصل على أو يضبط أنماط css الإضافية للمنسق. يعمل فقط عندما يكون [`SaveAsSingleFile`](./saveassinglefile/) True.  CssStyles="body { padding: 5px }"; |
| [DataBarRenderMode](../../aspose.cells/htmlsaveoptions/databarrendermode/) { get; set; } | يمثل وضع كيفية عرض DataBar عند تحويل ملفات Excel إلى ملفات html. القيمة الافتراضية هي BackgroundColor. |
| [DefaultFontName](../../aspose.cells/htmlsaveoptions/defaultfontname/) { get; set; } | حدد اسم الخط الافتراضي لتصدير html، سيُستخدم الخط الافتراضي عندما لا يكون خط النمط موجودًا، إذا كانت هذه الخاصية null، سيستخدم Aspose.Cells خطًا عالميًا يملك نفس عائلة الخط الأصلي، القيمة الافتراضية هي null. |
| [DisableCss](../../aspose.cells/htmlsaveoptions/disablecss/) { get; set; } | يشير إلى ما إذا كانت الأنماط المضمنة فقط تُطبق، دون الاعتماد على CSS. القيمة الافتراضية هي false. |
| [DisableDownlevelRevealedComments](../../aspose.cells/htmlsaveoptions/disabledownlevelrevealedcomments/) { get; set; } | يشير إلى ما إذا كان يتم تعطيل التعليقات الشرطية المكشوفة للمتصفحات القديمة عند تصدير الملف إلى html، القيمة الافتراضية هي false. |
| [EmbeddedFontType](../../aspose.cells/htmlsaveoptions/embeddedfonttype/) { get; set; } | يحصل على أو يضبط نوع تضمين ملف الخط في ملف html. القيمة الافتراضية هي None والتي تشير إلى عدم تضمين أي خط في html. |
| [EnableCssCustomProperties](../../aspose.cells/htmlsaveoptions/enablecsscustomproperties/) { get; set; } | حسّن مخرجات html باستخدام خصائص CSS المخصصة. على سبيل المثال، في السيناريو الذي توجد فيه تكرارات متعددة لصورة base64 واحدة، مع الخاصية المخصصة يحتاج بيانات الصورة أن تُحفظ مرة واحدة فقط وبالتالي يمكن تحسين أداء html الناتج. القيمة الافتراضية هي false. |
| [EncodeEntityAsCode](../../aspose.cells/htmlsaveoptions/encodeentityascode/) { get; set; } | يشير إلى ما إذا كانت كيانات أحرف html تُستبدل بالرمز العشري. (مثال: "&amp;nbsp;" تُستبدل بـ "&amp;#160;"). القيمة الافتراضية هي false. |
| [Encoding](../../aspose.cells/htmlsaveoptions/encoding/) { get; set; } | إذا لم يتم تعيينه، استخدم Encoding.UTF8 كنوع الترميز الافتراضي. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | يشير إلى ما إذا كان يتم تشفير خصائص المستند عند الحفظ كملف .xls. القيمة الافتراضية هي true. (موروث من [`SaveOptions`](../saveoptions/).) |
| [ExcludeUnusedStyles](../../aspose.cells/htmlsaveoptions/excludeunusedstyles/) { get; set; } | يشير إلى ما إذا كان يتم استبعاد الأنماط غير المستخدمة. بالنسبة لملفات html المولدة، استبعاد الأنماط غير المستخدمة يمكن أن يقلل حجم الملف دون التأثير على التأثيرات البصرية. لذا القيمة الافتراضية لهذه الخاصية هي true. إذا كان المستخدم يحتاج إلى الاحتفاظ بجميع الأنماط في المصنف للـ html المولد (مثل السيناريو الذي يحتاج فيه المستخدم لاستعادة المصنف من الـ html المولد لاحقًا)، يرجى تعيين هذه الخاصية إلى false. |
| [ExportActiveWorksheetOnly](../../aspose.cells/htmlsaveoptions/exportactiveworksheetonly/) { get; set; } | يشير إلى ما إذا كان يتم تصدير ورقة العمل النشطة فقط إلى ملف html. إذا كان true فستُصدر ورقة العمل النشطة فقط إلى ملف html؛ إذا كان false فسيتم تصدير المصنف بالكامل إلى ملف html. القيمة الافتراضية هي false. |
| [ExportArea](../../aspose.cells/htmlsaveoptions/exportarea/) { get; set; } | يحصل على أو يضبط CellArea المُصدَّر لورقة العمل النشطة الحالية. إذا قمت بتعيين هذه السمة، سيتم حذف منطقة الطباعة لورقة العمل النشطة الحالية. سيتم تصدير المنطقة المحددة فقط عند حفظ الملف إلى html. |
| [ExportBogusRowData](../../aspose.cells/htmlsaveoptions/exportbogusrowdata/) { get; set; } | تشير إلى ما إذا كان يتم تصدير بيانات الصف السفلي الزائفة. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html أو mht إلى Excel، يرجى الحفاظ على القيمة الافتراضية. |
| [ExportCellCoordinate](../../aspose.cells/htmlsaveoptions/exportcellcoordinate/) { get; set; } | تشير إلى ما إذا كان يتم تصدير إحداثيات Excel للخلايا غير الفارغة عند حفظ الملف إلى html. القيمة الافتراضية هي false. إذا كنت تريد استيراد ملف html الناتج إلى Excel، يرجى الحفاظ على القيمة الافتراضية. |
| [ExportCommentsType](../../aspose.cells/htmlsaveoptions/exportcommentstype/) { get; set; } | يمثل نوع تصدير التعليقات إلى ملفات html. |
| [ExportDataOptions](../../aspose.cells/htmlsaveoptions/exportdataoptions/) { get; set; } | تشير إلى قاعدة تصدير بيانات ملف html. القيمة الافتراضية هي All. |
| [ExportDocumentProperties](../../aspose.cells/htmlsaveoptions/exportdocumentproperties/) { get; set; } | تشير إلى ما إذا كان يتم تصدير خصائص المستند. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html أو mht إلى Excel، يرجى الحفاظ على القيمة الافتراضية. |
| [ExportExtraHeadings](../../aspose.cells/htmlsaveoptions/exportextraheadings/) { get; set; } | تشير إلى ما إذا كان يتم تصدير عناوين إضافية عندما يكون طول النص أطول من الحد الأقصى لعرض العمود. القيمة الافتراضية هي false. إذا كنت تريد استيراد ملف html إلى Excel، يرجى الحفاظ على القيمة الافتراضية. |
| [ExportFormula](../../aspose.cells/htmlsaveoptions/exportformula/) { get; set; } | تشير إلى ما إذا كان يتم تصدير الصيغ عند حفظ الملف إلى html. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html الناتج إلى Excel، يرجى الحفاظ على القيمة الافتراضية. |
| [ExportFrameScriptsAndProperties](../../aspose.cells/htmlsaveoptions/exportframescriptsandproperties/) { get; set; } | تشير إلى ما إذا كان يتم تصدير سكريبتات الإطار وخصائص المستند. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html أو mht إلى Excel، يرجى الحفاظ على القيمة الافتراضية. |
| [ExportGridLines](../../aspose.cells/htmlsaveoptions/exportgridlines/) { get; set; } | تشير إلى ما إذا كان يتم تصدير خطوط الشبكة. القيمة الافتراضية هي false. |
| [ExportHeadings](../../aspose.cells/htmlsaveoptions/exportheadings/) { get; set; } | (**Obsolete.**) تشير إلى ما إذا كان يتم تصدير رؤوس الصفوف والأعمدة للورقة عند الحفظ إلى ملفات HTML. |
| [ExportHiddenWorksheet](../../aspose.cells/htmlsaveoptions/exporthiddenworksheet/) { get; set; } | تشير إلى ما إذا كان يتم تصدير محتوى ورقة العمل المخفي. القيمة الافتراضية هي true. |
| [ExportImagesAsBase64](../../aspose.cells/htmlsaveoptions/exportimagesasbase64/) { get; set; } | يحدد ما إذا كانت الصور تُحفظ بصيغة Base64 إلى HTML أو MHTML أو EPUB. |
| [ExportNamedRangeAnchors](../../aspose.cells/htmlsaveoptions/exportnamedrangeanchors/) { get; set; } | تشير إلى ما إذا كان يتم تصدير عناصر الربط للنطاقات المسماة عند الحفظ كـ HTML. القيمة الافتراضية هي true. |
| [ExportObjectListener](../../aspose.cells/htmlsaveoptions/exportobjectlistener/) { get; set; } | (**Obsolete.**) يحصل على أو يضبط ExportObjectListener لتصدير الكائنات. |
| [ExportPageFooters](../../aspose.cells/htmlsaveoptions/exportpagefooters/) { get; set; } | تشير إلى ما إذا كان يتم تصدير رؤوس الصفحات. |
| [ExportPageHeaders](../../aspose.cells/htmlsaveoptions/exportpageheaders/) { get; set; } | تشير إلى ما إذا كان يتم تصدير رؤوس الصفحات. |
| [ExportPrintAreaOnly](../../aspose.cells/htmlsaveoptions/exportprintareaonly/) { get; set; } | تشير إلى ما إذا كان يتم تصدير منطقة الطباعة فقط إلى ملف html. القيمة الافتراضية هي false. |
| [ExportRowColumnHeadings](../../aspose.cells/htmlsaveoptions/exportrowcolumnheadings/) { get; set; } | تشير إلى ما إذا كان يتم تصدير رؤوس الصفوف والأعمدة للورقة عند الحفظ إلى ملفات HTML. |
| [ExportSimilarBorderStyle](../../aspose.cells/htmlsaveoptions/exportsimilarborderstyle/) { get; set; } | تشير إلى ما إذا كان يتم تصدير نمط الحدود المشابه عندما لا يدعم المتصفحات نمط الحدود. إذا كنت تريد استيراد ملف html أو mht إلى Excel، يرجى الحفاظ على القيمة الافتراضية. القيمة الافتراضية هي false. |
| [ExportSingleTab](../../aspose.cells/htmlsaveoptions/exportsingletab/) { get; set; } | تشير إلى ما إذا كان يتم تصدير علامة التبويب الوحيدة عندما يحتوي الملف على ورقة عمل واحدة فقط. القيمة الافتراضية هي false. |
| [ExportWorkbookProperties](../../aspose.cells/htmlsaveoptions/exportworkbookproperties/) { get; set; } | تشير إلى ما إذا كان يتم تصدير خصائص دفتر العمل. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html أو mht إلى Excel، يرجى الحفاظ على القيمة الافتراضية. |
| [ExportWorksheetCSSSeparately](../../aspose.cells/htmlsaveoptions/exportworksheetcssseparately/) { get; set; } | تشير إلى ما إذا كان يتم تصدير CSS لورقة العمل بشكل منفصل. القيمة الافتراضية هي false. |
| [ExportWorksheetProperties](../../aspose.cells/htmlsaveoptions/exportworksheetproperties/) { get; set; } | تشير إلى ما إذا كان يتم تصدير خصائص ورقة العمل. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html أو mht إلى Excel، يرجى الحفاظ على القيمة الافتراضية. |
| [FilePathProvider](../../aspose.cells/htmlsaveoptions/filepathprovider/) { get; set; } | يحصل على أو يضبط IFilePathProvider لتصدير Worksheet إلى html بشكل منفصل. |
| [FormatDataIgnoreColumnWidth](../../aspose.cells/htmlsaveoptions/formatdataignorecolumnwidth/) { get; set; } | تشير إلى ما إذا كان يتم عرض جميع البيانات المنسقة للخلية عندما يتجاوز العمود. إذا كان true يتم تجاهل عرض العمود وسيتم تصدير جميع بيانات الخلية. إذا كان false سيتم تصدير البيانات كما في Excel. القيمة الافتراضية هي false. |
| [HiddenColDisplayType](../../aspose.cells/htmlsaveoptions/hiddencoldisplaytype/) { get; set; } | العمود المخفي (عرض هذا العمود هو 0) في Excel، قبل حفظه بصيغة html، إذا كان HtmlHiddenColDisplayType هو \"Remove\"، فلن يتم إخراج العمود المخفي، إذا كانت القيمة \"Hidden\"، سيتم إخراج العمود لكنه سيبقى مخفيًا، القيمة الافتراضية هي \"Hidden\". |
| [HiddenRowDisplayType](../../aspose.cells/htmlsaveoptions/hiddenrowdisplaytype/) { get; set; } | صف مخفي (ارتفاع هذا الصف هو 0) في Excel، قبل حفظه بصيغة html، إذا كان HtmlHiddenRowDisplayType هو "Remove"، فلن يتم إخراج الصف المخفي، إذا كانت القيمة "Hidden"، سيتم إخراج الصف ولكنه مخفي، القيمة الافتراضية هي "Hidden" |
| [HideOverflowWrappedText](../../aspose.cells/htmlsaveoptions/hideoverflowwrappedtext/) { get; set; } | يشير إلى ما إذا كان سيتم إخفاء النص المتجاوز عندما يتم تعيين تنسيق الخلية إلى التفاف النص. القيمة الافتراضية هي false |
| [HtmlCrossStringType](../../aspose.cells/htmlsaveoptions/htmlcrossstringtype/) { get; set; } | يشير إلى ما إذا كان سيتم عرض سلسلة عبر الخلايا بنفس طريقة MS Excel عند حفظ ملف Excel بصيغة html. بشكل افتراضي القيمة هي Default، لذا بالنسبة لسلاسل عبر الخلايا، هناك فرق بسيط بين ملفات html التي تم إنشاؤها بواسطة Aspose.Cells و MS Excel. لكن الأداء لإنشاء ملفات html الكبيرة، ضبط القيمة إلى Cross سيكون أسرع عدة مرات مقارنةً بضبطها إلى Default أو Fit2Cell. |
| [HtmlVersion](../../aspose.cells/htmlsaveoptions/htmlversion/) { get; set; } | يحدد إصدار معيار HTML الذي يجب استخدامه عند حفظ الصيغة HTML. القيمة الافتراضية هي HtmlVersion.Default. |
| [IgnoreInvisibleShapes](../../aspose.cells/htmlsaveoptions/ignoreinvisibleshapes/) { get; set; } | يشير إلى ما إذا كان سيتم تصدير الأشكال غير المرئية |
| [ImageOptions](../../aspose.cells/htmlsaveoptions/imageoptions/) { get; } | احصل على كائن ImageOrPrintOptions قبل التصدير |
| [ImageScalable](../../aspose.cells/htmlsaveoptions/imagescalable/) { get; set; } | يشير إلى ما إذا كان سيتم استخدام وحدة قابلة للتوسع لوصف عرض الصورة عند استخدام وحدة قابلة للتوسع لوصف عرض العمود. القيمة الافتراضية هي true. |
| [IsBorderCollapsed](../../aspose.cells/htmlsaveoptions/isbordercollapsed/) { get; set; } | يشير إلى ما إذا كانت حدود الجدول مدمجة. القيمة الافتراضية هي true. |
| [IsExpImageToTempDir](../../aspose.cells/htmlsaveoptions/isexpimagetotempdir/) { get; set; } | يشير إلى ما إذا كان سيتم تصدير ملفات الصور إلى دليل مؤقت. فقط لحفظ إلى تدفق html. |
| [IsExportComments](../../aspose.cells/htmlsaveoptions/isexportcomments/) { get; set; } | يشير إلى ما إذا كان سيتم تصدير التعليقات عند حفظ الملف إلى html، القيمة الافتراضية هي false. |
| [IsFullPathLink](../../aspose.cells/htmlsaveoptions/isfullpathlink/) { get; set; } | يشير إلى ما إذا كان سيتم استخدام رابط المسار الكامل في sheet00x.htm،filelist.xml و tabstrip.htm. القيمة الافتراضية هي false. |
| [IsIECompatible](../../aspose.cells/htmlsaveoptions/isiecompatible/) { get; set; } | يشير إلى ما إذا كان HTML الناتج متوافقًا مع متصفح IE. القيمة الافتراضية هي false |
| [IsJsBrowserCompatible](../../aspose.cells/htmlsaveoptions/isjsbrowsercompatible/) { get; set; } | يشير إلى ما إذا كان JavaScript متوافقًا مع المتصفحات التي لا تدعم JavaScript. القيمة الافتراضية هي true. |
| [IsMobileCompatible](../../aspose.cells/htmlsaveoptions/ismobilecompatible/) { get; set; } | يشير إلى ما إذا كان HTML الناتج متوافقًا مع الأجهزة المحمولة. القيمة الافتراضية هي false. |
| [LayoutMode](../../aspose.cells/htmlsaveoptions/layoutmode/) { get; set; } | يحصل أو يضبط وضع التخطيط عند الحفظ إلى HTML. القيمة الافتراضية هي Normal |
| [LinkTargetType](../../aspose.cells/htmlsaveoptions/linktargettype/) { get; set; } | يشير إلى نوع خاصية target في رابط `<a>`. القيمة الافتراضية هي HtmlLinkTargetType.Parent. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | يشير إلى ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق قبل حفظ الملف. (موروث من [`SaveOptions`](../saveoptions/).) |
| [MergeEmptyTdForcely](../../aspose.cells/htmlsaveoptions/mergeemptytdforcely/) { get; set; } | (**Obsolete.**) يشير إلى ما إذا كان سيتم دمج عنصر TD فارغ بالقوة عند تصدير الملف إلى html. سيقل حجم ملف html بشكل كبير بعد ضبط القيمة إلى true. القيمة الافتراضية هي false. إذا كنت تريد استيراد ملف html إلى Excel أو تصدير خطوط شبكة مثالية عند حفظ الملف إلى html، يرجى الحفاظ على القيمة الافتراضية. |
| [MergeEmptyTdType](../../aspose.cells/htmlsaveoptions/mergeemptytdtype/) { get; set; } | الخيار لدمج الخلايا الفارغة المتجاورة (عناصر td الفارغة). القيمة الافتراضية هي MergeEmptyTdType.Default. |
| [OfficeMathOutputMode](../../aspose.cells/htmlsaveoptions/officemathoutputmode/) { get; set; } | يشير إلى كيفية تصدير كائنات OfficeMath إلى HTML، القيمة الافتراضية هي Image. |
| [PageTitle](../../aspose.cells/htmlsaveoptions/pagetitle/) { get; set; } | عنوان صفحة html. فقط لحفظ إلى تدفق html. |
| [ParseHtmlTagInCell](../../aspose.cells/htmlsaveoptions/parsehtmltagincell/) { get; set; } | يشير إلى ما إذا كان يجب تحليل علامة html (مثل `<div></div>`) في الخلية كقيمة خلية أو الحفاظ عليها كما هي. القيمة الافتراضية هي true. |
| [PresentationPreference](../../aspose.cells/htmlsaveoptions/presentationpreference/) { get; set; } | يشير إلى ما إذا كان ملف html أو mht هو تفضيل العرض. القيمة الافتراضية هي false. إذا كنت تريد الحصول على عرض أكثر جمالًا، يرجى ضبط القيمة إلى true. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | يشير إلى ما إذا كان يتم تخزين أحدث بيانات المخطط مؤقتًا. (موروث من [`SaveOptions`](../saveoptions/).) |
| [SaveAsSingleFile](../../aspose.cells/htmlsaveoptions/saveassinglefile/) { get; set; } | يشير إلى ما إذا كان سيتم حفظ html كملف واحد. القيمة الافتراضية هي false. |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | يحصل على تنسيق حفظ الملف. (موروث من [`SaveOptions`](../saveoptions/).) |
| [SheetSet](../../aspose.cells/htmlsaveoptions/sheetset/) { get; set; } | يحصل أو يضبط الأوراق التي سيتم عرضها. الافتراضي هو جميع الأوراق المرئية في المصنف: [`Visible`](../../aspose.cells.rendering/sheetset/visible/). |
| [ShowAllSheets](../../aspose.cells/htmlsaveoptions/showallsheets/) { get; set; } | يشير إلى ما إذا كان سيتم عرض جميع الأوراق عند الحفظ كملف html واحد. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | يشير إلى ما إذا كان يتم فرز الأسماء المعرفة الخارجية قبل حفظ الملف. (موروث من [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | يشير إلى ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف. (موروث من [`SaveOptions`](../saveoptions/).) |
| [SpaceMode](../../aspose.cells/htmlsaveoptions/spacemode/) { get; set; } | يشير إلى كيفية عرض المسافات في مخرجات HTML. يتم تطبيق هذا الخيار حالياً فقط على الصيغ الرقمية (مثل صيغة المحاسبة). القيمة الافتراضية هي Css. |
| [StreamProvider](../../aspose.cells/htmlsaveoptions/streamprovider/) { get; set; } | يحصل أو يعيّن IStreamProvider لتصدير الكائنات. |
| [TableCssId](../../aspose.cells/htmlsaveoptions/tablecssid/) { get; set; } | يحصل ويعيّن بادئة اسم نوع CSS مثل tr, col, td وغيرها، والتي تُضمّن في عنصر الجدول الذي يحتوي على السمة TableCssId المحددة. القيمة الافتراضية هي "". |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | يشير إلى ما إذا كان يتم تحديث إعدادات Smart Art. القيمة الافتراضية هي false. (موروث من [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | يشير إلى ما إذا كان يتم التحقق من صحة الخلايا المدمجة قبل حفظ الملف. (موروث من [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | يحصل أو يعيّن رد الاتصال التحذيري.(موروث من [`SaveOptions`](../saveoptions/).) |
| [WidthScalable](../../aspose.cells/htmlsaveoptions/widthscalable/) { get; set; } | يشير إلى ما إذا كان يتم تصدير عرض العمود بوحدة المقياس إلى HTML. القيمة الافتراضية هي false. |
| [WorksheetScalable](../../aspose.cells/htmlsaveoptions/worksheetscalable/) { get; set; } | يشير إلى ما إذا كان يتم تكبير أو تصغير HTML عبر مستوى تكبير ورقة العمل عند حفظ الملف إلى HTML، القيمة الافتراضية هي false. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlSaveOptionsDemo
    {
        public static void HtmlSaveOptionsExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // إنشاء نسخة من HtmlSaveOptions
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                IgnoreInvisibleShapes = true,
                PageTitle = "Sample HTML Page",
                AttachedFilesDirectory = "attached_files",
                AttachedFilesUrlPrefix = "http://example.com/files/",
                DefaultFontName = "Arial",
                AddGenericFont = true,
                WorksheetScalable = false,
                IsExportComments = false,
                ExportCommentsType = PrintCommentsType.PrintNoComments,
                DisableDownlevelRevealedComments = false,
                IsExpImageToTempDir = false,
                ImageScalable = true,
                WidthScalable = false,
                ExportSingleTab = false,
                ExportImagesAsBase64 = false,
                ExportActiveWorksheetOnly = false,
                ExportPrintAreaOnly = false,
                ExportArea = new CellArea { StartRow = 0, EndRow = 1, StartColumn = 0, EndColumn = 1 },
                ParseHtmlTagInCell = true,
                HtmlCrossStringType = HtmlCrossType.Default,
                HiddenColDisplayType = HtmlHiddenColDisplayType.Hidden,
                HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden,
                Encoding = System.Text.Encoding.UTF8,
                SaveAsSingleFile = false,
                ShowAllSheets = false,
                ExportPageHeaders = false,
                ExportPageFooters = false,
                ExportHiddenWorksheet = true,
                PresentationPreference = false,
                CellCssPrefix = "",
                TableCssId = "",
                IsFullPathLink = false,
                ExportWorksheetCSSSeparately = false,
                ExportSimilarBorderStyle = false,
                MergeEmptyTdForcely = false,
                MergeEmptyTdType = MergeEmptyTdType.Default,
                ExportCellCoordinate = false,
                ExportExtraHeadings = false,
                ExportHeadings = false,
                ExportRowColumnHeadings = false,
                ExportFormula = true,
                AddTooltipText = false,
                ExportGridLines = false,
                ExportBogusRowData = true,
                ExcludeUnusedStyles = true,
                ExportDocumentProperties = true,
                ExportWorksheetProperties = true,
                ExportWorkbookProperties = true,
                ExportFrameScriptsAndProperties = true,
                ExportDataOptions = HtmlExportDataOptions.All,
                LinkTargetType = HtmlLinkTargetType.Parent,
                IsIECompatible = false,
                FormatDataIgnoreColumnWidth = false,
                CalculateFormula = true,
                IsJsBrowserCompatible = true,
                IsMobileCompatible = false,
                CssStyles = "body { padding: 5px }",
                HideOverflowWrappedText = false,
                IsBorderCollapsed = true,
                ClearData = false,
                CachedFileFolder = "cache",
                ValidateMergedAreas = true,
                MergeAreas = true,
                SortNames = true,
                SortExternalNames = true,
                RefreshChartCache = true,
                UpdateSmartArt = false
            };

            // حفظ المصنف كملف HTML
            workbook.Save("HtmlSaveOptionsExample.html", saveOptions);

            return;
        }
    }
}
```

### انظر أيضًا

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


