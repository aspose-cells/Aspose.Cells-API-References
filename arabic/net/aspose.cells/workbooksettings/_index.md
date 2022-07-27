---
title: WorkbookSettings
second_title: Aspose.Cells لمرجع .NET API
description: يمثل كافة إعدادات المصنف.
type: docs
weight: 6500
url: /ar/net/aspose.cells/workbooksettings/
---
## WorkbookSettings class

يمثل كافة إعدادات المصنف.

```csharp
public class WorkbookSettings : IDisposable
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [Author](../../aspose.cells/workbooksettings/author) { get; set; } | الحصول على كاتب الملف وتعيينه. |
| [AutoCompressPictures](../../aspose.cells/workbooksettings/autocompresspictures) { get; set; } | يحدد قيمة منطقية تشير إلى التطبيق الذي تم ضغطه تلقائيًا في المصنف. |
| [AutoRecover](../../aspose.cells/workbooksettings/autorecover) { get; set; } | يشير إلى ما إذا كان الملف علامة للاسترداد التلقائي. |
| [BuildVersion](../../aspose.cells/workbooksettings/buildversion) { get; set; } | يحدد الإصدار العام المتزايد للتطبيق. |
| [CheckCompatibility](../../aspose.cells/workbooksettings/checkcompatibility) { get; set; } | يشير إلى ما إذا كان التحقق من التوافق مع الإصدارات السابقة عند حفظ المصنف. |
| [CheckCustomNumberFormat](../../aspose.cells/workbooksettings/checkcustomnumberformat) { get; set; } | يشير إلى ما إذا كان التحقق من تنسيق الأرقام المخصص عند تعيين Style.Custom. |
| [CheckExcelRestriction](../../aspose.cells/workbooksettings/checkexcelrestriction) { get; set; } | ما إذا كان التحقق من تقييد ملف Excel عند قيام المستخدم بتعديل الكائنات ذات الصلة بالخلايا. على سبيل المثال ، لا يسمح Excel بإدخال قيمة سلسلة أطول من 32 كيلو بايت . عند إدخال قيمة أطول من 32 كيلو بايت مثل عن طريق Cell.PutValue (سلسلة) ، إذا كان هذا الخاصية صحيحة ، ستحصل على استثناء . إذا كانت هذه الخاصية خاطئة ، فسنقبل قيمة سلسلة الإدخال كقيمة للخلية بحيث يمكنك لاحقًا إخراج قيمة السلسلة الكاملة لتنسيقات الملفات الأخرى مثل CSV. ومع ذلك ، إذا لقد قمت بتعيين مثل هذا النوع من القيمة غير الصالحة لتنسيق ملف Excel ، يجب ألا تحفظ المصنف بتنسيق ملف excel لاحقًا. وإلا فقد يكون هناك خطأ غير متوقع لملف Excel الذي تم إنشاؤه. |
| [Compliance](../../aspose.cells/workbooksettings/compliance) { get; set; } | يحدد إصدار OOXML لوثيقة الإخراج. القيمة الافتراضية هي Ecma376_2006. |
| [CrashSave](../../aspose.cells/workbooksettings/crashsave) { get; set; } | يشير إلى ما إذا كان التطبيق قد حفظ ملف المصنف آخر مرة بعد التعطل. |
| [CultureInfo](../../aspose.cells/workbooksettings/cultureinfo) { get; set; } | الحصول على أو تعيين معلومات ثقافة النظام. |
| [DataExtractLoad](../../aspose.cells/workbooksettings/dataextractload) { get; set; } | يشير إلى ما إذا كان التطبيق قد فتح المصنف آخر مرة لاستعادة البيانات. |
| [Date1904](../../aspose.cells/workbooksettings/date1904) { get; set; } | الحصول على أو تعيين قيمة تمثل ما إذا كان المصنف يستخدم نظام التاريخ 1904. |
| [DisplayDrawingObjects](../../aspose.cells/workbooksettings/displaydrawingobjects) { get; set; } | يشير إلى ما إذا كان سيتم إظهار الكائنات في المصنف وكيفية إظهارها. |
| [EnableMacros](../../aspose.cells/workbooksettings/enablemacros) { get; set; } | تمكين وحدات الماكرو ؛ |
| [FirstVisibleTab](../../aspose.cells/workbooksettings/firstvisibletab) { get; set; } | الحصول على أول علامة تبويب مرئية لورقة العمل أو تعيينها. |
| [FormulaSettings](../../aspose.cells/workbooksettings/formulasettings) { get; } | الحصول على إعدادات الميزات المتعلقة بالصيغة. |
| [GlobalizationSettings](../../aspose.cells/workbooksettings/globalizationsettings) { get; set; } | الحصول على إعدادات العولمة وتعيينها. |
| [HidePivotFieldList](../../aspose.cells/workbooksettings/hidepivotfieldlist) { get; set; } | الحصول على وتحديد ما إذا كان سيتم إخفاء قائمة الحقول لجدول PivotTable. |
| [IsDefaultEncrypted](../../aspose.cells/workbooksettings/isdefaultencrypted) { get; set; } | يشير إلى ما إذا كان تشفير المصنف بكلمة مرور افتراضية إذا تم تأمين البنية و Windows للمصنف. |
| [IsEncrypted](../../aspose.cells/workbooksettings/isencrypted) { get; } | يحصل على قيمة تشير إلى ما إذا كانت كلمة المرور مطلوبة لفتح هذا المصنف. |
| [IsHidden](../../aspose.cells/workbooksettings/ishidden) { get; set; } | يشير إلى ما إذا كان هذا المصنف مخفيًا. |
| [IsHScrollBarVisible](../../aspose.cells/workbooksettings/ishscrollbarvisible) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان جدول البيانات الذي تم إنشاؤه سيحتوي على شريط تمرير أفقي. |
| [IsMinimized](../../aspose.cells/workbooksettings/isminimized) { get; set; } | يمثل ما إذا كان سيتم فتح جدول البيانات الذي تم إنشاؤه بأدنى حد. |
| [IsProtected](../../aspose.cells/workbooksettings/isprotected) { get; } | الحصول على قيمة تشير إلى ما إذا كانت بنية أو نافذة المصنف محمية. |
| [IsVScrollBarVisible](../../aspose.cells/workbooksettings/isvscrollbarvisible) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان جدول البيانات الذي تم إنشاؤه سيحتوي على شريط تمرير عمودي. |
| [LanguageCode](../../aspose.cells/workbooksettings/languagecode) { get; set; } | الحصول على أو تعيين لغة واجهة المستخدم لإصدار المصنف بناءً على كود البلد الذي حفظ الملف. |
| [MaxColumn](../../aspose.cells/workbooksettings/maxcolumn) { get; } | الحصول على فهرس العمود الأقصى ، على أساس الصفر . |
| [MaxRow](../../aspose.cells/workbooksettings/maxrow) { get; } | يحصل على فهرس الصف الأقصى ، على أساس الصفر . |
| [MaxRowsOfSharedFormula](../../aspose.cells/workbooksettings/maxrowsofsharedformula) { get; set; } | الحصول على الحد الأقصى لعدد الصف الخاص بالصيغة المشتركة وتعيينه. |
| [MemorySetting](../../aspose.cells/workbooksettings/memorysetting) { get; set; } | الحصول على أو تعيين خيارات استخدام الذاكرة. سيتم اتخاذ الخيار الجديد كخيار افتراضي لأوراق العمل المنشأة حديثًا ولكنه لا يسري على أوراق العمل الحالية. |
| [NumberDecimalSeparator](../../aspose.cells/workbooksettings/numberdecimalseparator) { get; set; } | الحصول على أو تعيين الفاصل العشري لتنسيق / تحليل القيم الرقمية. الافتراضي هو الفاصل العشري للمنطقة الحالية. |
| [NumberGroupSeparator](../../aspose.cells/workbooksettings/numbergroupseparator) { get; set; } | الحصول على أو تعيين الحرف الذي يفصل بين مجموعات الأرقام على يسار العلامة العشرية في القيم الرقمية. الافتراضي هو فاصل المجموعة للمنطقة الحالية. |
| [PaperSize](../../aspose.cells/workbooksettings/papersize) { get; set; } | الحصول على حجم ورق الطباعة الافتراضي وتعيينه. |
| [Password](../../aspose.cells/workbooksettings/password) { get; set; } | يمثل كلمة مرور تشفير ملف المصنف. |
| [ProtectionType](../../aspose.cells/workbooksettings/protectiontype) { get; } | يحصل على نوع الحماية للمصنف. |
| [QuotePrefixToStyle](../../aspose.cells/workbooksettings/quoteprefixtostyle) { get; set; } | يشير إلى ما إذا كان الإعداد[`QuotePrefix`](../style/quoteprefix) الخاصية عند إدخال قيمة السلسلة (التي تبدأ بعلامة اقتباس مفردة) في الخلية |
| [Region](../../aspose.cells/workbooksettings/region) { get; set; } | الحصول على الإعدادات الإقليمية للمصنف أو تعيينها. |
| [RemovePersonalInformation](../../aspose.cells/workbooksettings/removepersonalinformation) { get; set; } | صواب إذا كان من الممكن إزالة المعلومات الشخصية من المصنف المحدد. |
| [RepairLoad](../../aspose.cells/workbooksettings/repairload) { get; set; } | يشير إلى ما إذا كان التطبيق قد فتح المصنف آخر مرة في الوضع الآمن أو وضع الإصلاح. |
| [ResourceProvider](../../aspose.cells/workbooksettings/resourceprovider) { get; set; } | الحصول على موفر التدفق للمورد الخارجي وتعيينه ، مثل تحميل بيانات الصورة لصورة من النوع "LinkToFile" . |
| [Shared](../../aspose.cells/workbooksettings/shared) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان المصنف مشتركًا أم لا. |
| [SheetTabBarWidth](../../aspose.cells/workbooksettings/sheettabbarwidth) { get; set; } | عرض شريط علامة تبويب ورقة العمل (في 1/1000 من عرض النافذة) . |
| [ShowTabs](../../aspose.cells/workbooksettings/showtabs) { get; set; } | الحصول على قيمة أو تعيينها سواء كانت علامات تبويب المصنف معروضة. |
| [SignificantDigits](../../aspose.cells/workbooksettings/significantdigits) { get; set; } | الحصول على عدد الأرقام المهمة وتعيينه . القيمة الافتراضية هي[`SignificantDigits`](../cellshelper/significantdigits) . |
| [UpdateAdjacentCellsBorder](../../aspose.cells/workbooksettings/updateadjacentcellsborder) { get; set; } | يشير إلى ما إذا كان سيتم تحديث حدود الخلايا المجاورة. |
| [UpdateLinksType](../../aspose.cells/workbooksettings/updatelinkstype) { get; set; } | الحصول على كيفية تحديث الروابط الخارجية عند فتح المصنف وتعيينه. |
| [WarningCallback](../../aspose.cells/workbooksettings/warningcallback) { get; set; } | الحصول على رد اتصال التحذير أو تعيينه . |
| [WindowHeight](../../aspose.cells/workbooksettings/windowheight) { get; set; } | ارتفاع النافذة بوحدة النقطة . |
| [WindowHeightCM](../../aspose.cells/workbooksettings/windowheightcm) { get; set; } | ارتفاع النافذة بوحدة السنتيمتر . |
| [WindowHeightInch](../../aspose.cells/workbooksettings/windowheightinch) { get; set; } | ارتفاع النافذة بوحدة البوصة . |
| [WindowLeft](../../aspose.cells/workbooksettings/windowleft) { get; set; } | المسافة من الحافة اليسرى لمنطقة العميل إلى الحافة اليسرى من النافذة ، بوحدة النقطة . |
| [WindowLeftCM](../../aspose.cells/workbooksettings/windowleftcm) { get; set; } | المسافة من الحافة اليسرى لمنطقة العميل إلى الحافة اليسرى للنافذة. بوحدة السنتيمتر . |
| [WindowLeftInch](../../aspose.cells/workbooksettings/windowleftinch) { get; set; } | المسافة من الحافة اليسرى لمنطقة العميل إلى الحافة اليسرى للنافذة. بوحدة بوصة . |
| [WindowTop](../../aspose.cells/workbooksettings/windowtop) { get; set; } | المسافة من الحافة العلوية لمنطقة العميل إلى الحافة العلوية للنافذة ، بوحدة النقطة . |
| [WindowTopCM](../../aspose.cells/workbooksettings/windowtopcm) { get; set; } | المسافة من الحافة العلوية لمنطقة العميل إلى الحافة العلوية للنافذة ، بوحدة سنتيمتر. |
| [WindowTopInch](../../aspose.cells/workbooksettings/windowtopinch) { get; set; } | المسافة من الحافة العلوية لمنطقة العميل إلى الحافة العلوية للنافذة ، بوحدة بوصة . |
| [WindowWidth](../../aspose.cells/workbooksettings/windowwidth) { get; set; } | عرض النافذة بوحدة النقطة . |
| [WindowWidthCM](../../aspose.cells/workbooksettings/windowwidthcm) { get; set; } | عرض النافذة بوحدة السنتيمتر . |
| [WindowWidthInch](../../aspose.cells/workbooksettings/windowwidthinch) { get; set; } | عرض النافذة بوحدة البوصة . |
| [WriteProtection](../../aspose.cells/workbooksettings/writeprotection) { get; } | يوفر الوصول إلى خيارات الحماية ضد الكتابة في المصنف. |

## طُرق

| اسم | وصف |
| --- | --- |
| [Dispose](../../aspose.cells/workbooksettings/dispose)() | إصدارات الموارد . |
| [GetThemeFont](../../aspose.cells/workbooksettings/getthemefont)(FontSchemeType) | الحصول على اسم خط النسق الافتراضي. |
| [SetPageOrientationType](../../aspose.cells/workbooksettings/setpageorientationtype)(PageOrientationType) | حدد نوع اتجاه الطباعة لكامل المصنف. |

### أمثلة

```csharp
[C#]

Workbook workbook = new Workbook();

WorkbookSettings settings = workbook.Settings;

// قم بعملك

[Visual Basic]
Dim workbook as Workbook = new Workbook()

Dim settings as WorkbookSettings = workbook.Settings

'قم بعملك
```

### أنظر أيضا

* مساحة الاسم [Aspose.Cells](../../aspose.cells)
* المجسم [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
