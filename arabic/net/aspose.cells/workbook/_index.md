---
title: Workbook
second_title: Aspose.Cells لمرجع .NET API
description: يمثل كائنًا جذرًا لإنشاء جدول بيانات Excel.
type: docs
weight: 6480
url: /ar/net/aspose.cells/workbook/
---
## Workbook class

يمثل كائنًا جذرًا لإنشاء جدول بيانات Excel.

```csharp
public class Workbook : IDisposable
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [Workbook](workbook#constructor)() | يقوم بتهيئة مثيل جديد لملف[`Workbook`](../workbook) فئة . |
| [Workbook](workbook#constructor_1)(FileFormatType) | يقوم بتهيئة مثيل جديد لملف[`Workbook`](../workbook) فئة . |
| [Workbook](workbook#constructor_2)(Stream) | يقوم بتهيئة مثيل جديد لملف[`Workbook`](../workbook) فئة وافتح دفق. |
| [Workbook](workbook#constructor_4)(string) | يقوم بتهيئة مثيل جديد لملف[`Workbook`](../workbook) فئة وافتح ملفًا. |
| [Workbook](workbook#constructor_3)(Stream, LoadOptions) | يقوم بتهيئة مثيل جديد لملف[`Workbook`](../workbook) فئة ودفق مفتوح. |
| [Workbook](workbook#constructor_5)(string, LoadOptions) | يقوم بتهيئة مثيل جديد لملف[`Workbook`](../workbook) فئة وافتح ملفًا. |

## الخصائص

| اسم | وصف |
| --- | --- |
| [AbsolutePath](../../aspose.cells/workbook/absolutepath) { get; set; } | الحصول على المسار المطلق للملف وتعيينه. |
| [BuiltInDocumentProperties](../../aspose.cells/workbook/builtindocumentproperties) { get; } | إرجاع أ[`DocumentProperty`](../../aspose.cells.properties/documentproperty)مجموعة تمثل جميع خصائص المستند المضمنة في جدول البيانات. |
| [CellsDataTableFactory](../../aspose.cells/workbook/cellsdatatablefactory) { get; } | الحصول على المصنع لبناء ICellsDataTable من كائنات مخصصة |
| [Colors](../../aspose.cells/workbook/colors) { get; } | إرجاع الألوان في اللوحة لجدول البيانات. |
| [ContentTypeProperties](../../aspose.cells/workbook/contenttypeproperties) { get; } | يحصل على قائمة[`ContentTypeProperty`](../../aspose.cells.properties/contenttypeproperty) كائنات في المصنف. |
| [CountOfStylesInPool](../../aspose.cells/workbook/countofstylesinpool) { get; } | الحصول على عدد الأنماط في تجمع الأنماط . |
| [CustomDocumentProperties](../../aspose.cells/workbook/customdocumentproperties) { get; } | إرجاع أ[`DocumentProperty`](../../aspose.cells.properties/documentproperty) المجموعة التي تمثل جميع خصائص المستند المخصصة لجدول البيانات. |
| [CustomXmlParts](../../aspose.cells/workbook/customxmlparts) { get; } | يمثل جزء تخزين بيانات XML مخصص (بيانات XML مخصصة داخل حزمة). |
| [DataConnections](../../aspose.cells/workbook/dataconnections) { get; } | يحصل على ملف[`ExternalConnection`](../../aspose.cells.externalconnections/externalconnection) جمع . |
| [DataMashup](../../aspose.cells/workbook/datamashup) { get; } | الحصول على بيانات Mashup . |
| [DataSorter](../../aspose.cells/workbook/datasorter) { get; } | يحصل على كائن DataSorter لفرز البيانات. |
| [DefaultStyle](../../aspose.cells/workbook/defaultstyle) { get; set; } | الحصول على الإعداد الافتراضي أو تعيينه[`Style`](../style) كائن من المصنف . |
| [FileFormat](../../aspose.cells/workbook/fileformat) { get; set; } | الحصول على تنسيق الملف وتعيينه. |
| [FileName](../../aspose.cells/workbook/filename) { get; set; } | الحصول على اسم الملف الحالي وتعيينه. |
| [HasMacro](../../aspose.cells/workbook/hasmacro) { get; } | يشير إلى ما إذا كان جدول البيانات هذا يحتوي على ماكرو / VBA. |
| [HasRevisions](../../aspose.cells/workbook/hasrevisions) { get; } | يتم الحصول على ما إذا كان المصنف يحتوي على أي تغييرات متعقبة |
| [InterruptMonitor](../../aspose.cells/workbook/interruptmonitor) { get; set; } | الحصول على شاشة المقاطعة وتعيينها. |
| [IsDigitallySigned](../../aspose.cells/workbook/isdigitallysigned) { get; } | يشير إلى ما إذا كان جدول البيانات هذا موقعًا رقميًا. |
| [IsLicensed](../../aspose.cells/workbook/islicensed) { get; } | يشير إلى ما إذا تم تعيين الترخيص . |
| [IsWorkbookProtectedWithPassword](../../aspose.cells/workbook/isworkbookprotectedwithpassword) { get; } | يشير إلى ما إذا كانت البنية أو النافذة محمية بكلمة مرور. |
| [RibbonXml](../../aspose.cells/workbook/ribbonxml) { get; set; } | الحصول على ملف XML الذي يحدد واجهة مستخدم الشريط وتعيينه. |
| [Settings](../../aspose.cells/workbook/settings) { get; } | يمثل إعدادات المصنف. |
| [Theme](../../aspose.cells/workbook/theme) { get; } | يحصل على اسم المظهر. |
| [VbaProject](../../aspose.cells/workbook/vbaproject) { get; } | يحصل على ملف[`VbaProject`](./vbaproject) في جدول بيانات . |
| [Worksheets](../../aspose.cells/workbook/worksheets) { get; } | يحصل على ملف[`WorksheetCollection`](../worksheetcollection) جمع في جدول البيانات. |

## طُرق

| اسم | وصف |
| --- | --- |
| [AcceptAllRevisions](../../aspose.cells/workbook/acceptallrevisions)() | يقبل كافة التغييرات المتعقبة في المصنف. |
| [AddDigitalSignature](../../aspose.cells/workbook/adddigitalsignature)(DigitalSignatureCollection) | إضافة توقيع رقمي إلى ملف جدول بيانات OOXML (Excel2007 والإصدارات الأحدث). |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula#calculateformula)() | حساب نتيجة الصيغ . |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula#calculateformula_2)(bool) | حساب نتيجة الصيغ . |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula#calculateformula_1)(CalculationOptions) | حساب الصيغ في هذا المصنف. |
| [ChangePalette](../../aspose.cells/workbook/changepalette)(Color, int) | يغير لوحة جدول البيانات في الفهرس المحدد. |
| [CloseAccessCache](../../aspose.cells/workbook/closeaccesscache)(AccessCacheOptions) | إغلاق الجلسة التي تستخدم ذاكرات التخزين المؤقت للوصول إلى البيانات. |
| [Combine](../../aspose.cells/workbook/combine)(Workbook) | يجمع بين كائن مصنف آخر. |
| [Copy](../../aspose.cells/workbook/copy#copy)(Workbook) | نسخ البيانات من كائن مصنف مصدر . |
| [Copy](../../aspose.cells/workbook/copy#copy_1)(Workbook, CopyOptions) | نسخ البيانات من كائن مصنف مصدر . |
| [CopyTheme](../../aspose.cells/workbook/copytheme)(Workbook) | نسخ النسق من مصنف آخر . |
| [CreateBuiltinStyle](../../aspose.cells/workbook/createbuiltinstyle)(BuiltinStyleType) | ينشئ نمطًا مدمجًا حسب النوع المحدد. |
| [CreateCellsColor](../../aspose.cells/workbook/createcellscolor)() | ينشئ ملف[`CellsColor`](../cellscolor) الكائن . |
| [CreateStyle](../../aspose.cells/workbook/createstyle)() | ينشئ نمطًا جديدًا . |
| [CustomTheme](../../aspose.cells/workbook/customtheme)(string, Color[]) | جمارك الموضوع . |
| [Dispose](../../aspose.cells/workbook/dispose)() | يؤدي مهام محددة بواسطة التطبيق مرتبطة بتحرير الموارد غير المُدارة أو تحريرها أو إعادة تعيينها. |
| [ExportXml](../../aspose.cells/workbook/exportxml#exportxml)(string, Stream) | تصدير بيانات XML . |
| [ExportXml](../../aspose.cells/workbook/exportxml#exportxml_1)(string, string) | تصدير بيانات XML المرتبطة بخريطة XML المحددة. |
| [GetDigitalSignature](../../aspose.cells/workbook/getdigitalsignature)() | الحصول على توقيع رقمي من ملف . |
| [GetFonts](../../aspose.cells/workbook/getfonts)() | يحصل على كل الخطوط في تجمع الأنماط . |
| [GetMatchingColor](../../aspose.cells/workbook/getmatchingcolor)(Color) | البحث عن أفضل الألوان المطابقة في لوحة الألوان الحالية. |
| [GetNamedStyle](../../aspose.cells/workbook/getnamedstyle)(string) | الحصول على النمط المسمى في تجمع الأنماط . |
| [GetStyleInPool](../../aspose.cells/workbook/getstyleinpool)(int) | الحصول على النمط في تجمع الأنماط. سيتم تجميع كافة الأنماط الموجودة في المصنف في مجموعة . لا يوجد سوى فهرس مرجعي بسيط في الخلايا . |
| [GetThemeColor](../../aspose.cells/workbook/getthemecolor)(ThemeColorType) | الحصول على لون المظهر. |
| [ImportXml](../../aspose.cells/workbook/importxml#importxml)(Stream, string, int, int) | يستورد / يحدّث ملف بيانات XML في المصنف. |
| [ImportXml](../../aspose.cells/workbook/importxml#importxml_1)(string, string, int, int) | يستورد / يحدّث ملف بيانات XML في المصنف. |
| [IsColorInPalette](../../aspose.cells/workbook/iscolorinpalette)(Color) | للتحقق مما إذا كان اللون موجودًا في لوحة جدول البيانات. |
| [ParseFormulas](../../aspose.cells/workbook/parseformulas)(bool) | يوزع جميع الصيغ التي لم يتم تحليلها عند تحميلها من ملف قالب أو تعيينها إلى خلية. |
| [Protect](../../aspose.cells/workbook/protect)(ProtectionType, string) | حماية مصنف. |
| [ProtectSharedWorkbook](../../aspose.cells/workbook/protectsharedworkbook)(string) | حماية مصنف مشترك . |
| [RefreshDynamicArrayFormulas](../../aspose.cells/workbook/refreshdynamicarrayformulas)(bool) | تحديث صيغ الصفيف الديناميكية (الانسكاب في نطاق جديد من الخلايا المجاورة وفقًا للبيانات الحالية) |
| [RemoveDigitalSignature](../../aspose.cells/workbook/removedigitalsignature)() | يزيل التوقيع الرقمي من جدول البيانات هذا. |
| [RemoveMacro](../../aspose.cells/workbook/removemacro)() | يزيل VBA / الماكرو من جدول البيانات هذا. |
| [RemovePersonalInformation](../../aspose.cells/workbook/removepersonalinformation)() | إزالة المعلومات الشخصية . |
| [RemoveUnusedStyles](../../aspose.cells/workbook/removeunusedstyles)() | قم بإزالة كافة الأنماط غير المستخدمة. |
| [Replace](../../aspose.cells/workbook/replace#replace)(bool, object) | يستبدل قيم الخلايا ببيانات جديدة. |
| [Replace](../../aspose.cells/workbook/replace#replace_1)(int, object) | يستبدل قيم الخلايا ببيانات جديدة. |
| [Replace](../../aspose.cells/workbook/replace#replace_6)(string, DataTable) | يستبدل قيم الخلايا ببيانات من ملفDataTable . |
| [Replace](../../aspose.cells/workbook/replace#replace_2)(string, double) | يستبدل قيمة الخلية بمزدوج جديد. |
| [Replace](../../aspose.cells/workbook/replace#replace_4)(string, int) | يستبدل قيمة الخلية بعدد صحيح جديد. |
| [Replace](../../aspose.cells/workbook/replace#replace_7)(string, string) | يستبدل قيمة الخلية بسلسلة جديدة. |
| [Replace](../../aspose.cells/workbook/replace#replace_3)(string, double[], bool) | يستبدل قيم الخلايا بمصفوفة مزدوجة. |
| [Replace](../../aspose.cells/workbook/replace#replace_5)(string, int[], bool) | يستبدل قيم الخلايا بمصفوفة عدد صحيح. |
| [Replace](../../aspose.cells/workbook/replace#replace_8)(string, string, ReplaceOptions) | يستبدل قيمة الخلية بسلسلة جديدة. |
| [Replace](../../aspose.cells/workbook/replace#replace_9)(string, string[], bool) | يستبدل قيمة الخلية بمصفوفة سلسلة جديدة. |
| [Save](../../aspose.cells/workbook/save#save_2)(string) | احفظ المصنف على القرص. |
| [Save](../../aspose.cells/workbook/save#save)(Stream, SaveFormat) | يحفظ المصنف في الدفق . |
| [Save](../../aspose.cells/workbook/save#save_1)(Stream, SaveOptions) | يحفظ المصنف في الدفق . |
| [Save](../../aspose.cells/workbook/save#save_3)(string, SaveFormat) | يحفظ المصنف على القرص . |
| [Save](../../aspose.cells/workbook/save#save_4)(string, SaveOptions) | يحفظ المصنف على القرص . |
| [Save](../../aspose.cells/workbook/save#save_5)(HttpResponse, string, ContentDisposition, SaveOptions) | يقوم بإنشاء جدول البيانات الناتج ونقله إلى العميل ثم فتحه في المتصفح أو MS Workbook . |
| [Save](../../aspose.cells/workbook/save#save_6)(HttpResponse, string, ContentDisposition, SaveOptions, bool) | يقوم بإنشاء جدول البيانات الناتج ونقله إلى العميل ثم فتحه في المتصفح أو MS Workbook . |
| [SaveToStream](../../aspose.cells/workbook/savetostream)() | يحفظ ملف Excel في كائن MemoryStream وإعادته. |
| [SetDigitalSignature](../../aspose.cells/workbook/setdigitalsignature)(DigitalSignatureCollection) | تعيين التوقيع الرقمي إلى ملف جدول بيانات (Excel2007 والإصدارات الأحدث). |
| [SetEncryptionOptions](../../aspose.cells/workbook/setencryptionoptions)(EncryptionType, int) | تعيين خيارات التشفير . |
| [SetThemeColor](../../aspose.cells/workbook/setthemecolor)(ThemeColorType, Color) | يحدد لون السمة |
| [StartAccessCache](../../aspose.cells/workbook/startaccesscache)(AccessCacheOptions) | يبدأ الجلسة التي تستخدم ذاكرات التخزين المؤقت للوصول إلى البيانات. |
| [Unprotect](../../aspose.cells/workbook/unprotect)(string) | إلغاء حماية مصنف . |
| [UnprotectSharedWorkbook](../../aspose.cells/workbook/unprotectsharedworkbook)(string) | إلغاء حماية مصنف مشترك. |
| [UpdateLinkedDataSource](../../aspose.cells/workbook/updatelinkeddatasource)(Workbook[]) | إذا كان هذا المصنف يحتوي على ارتباطات خارجية بمصدر بيانات آخر ، فسيحاول Aspose.Cells استرداد أحدث البيانات. |

### ملاحظات

تشير فئة المصنف إلى جدول بيانات Excel. يمكن أن يحتوي كل جدول بيانات على أوراق عمل متعددة. الميزة الأساسية للفصل هي فتح ملفات Excel الأصلية وحفظها. يحتوي الفصل على بعض الميزات المتقدمة مثل نسخ البيانات من مصنفات أخرى ، والجمع بين مصنفين وحماية جدول بيانات Excel .

### أمثلة

يقوم المثال التالي بتحميل مصنف من ملف باسم designer.xls ويجعل أشرطة التمرير الأفقية والعمودية غير مرئية للمصنف. ثم يستبدل قيمتي سلسلة بقيمة عدد صحيح وقيمة سلسلة على التوالي داخل جدول البيانات وأخيرًا يرسل الملف المحدث إلى متصفح العميل.

```csharp
[C#]

// فتح ملف المصمم
string designerFile = "designer.xls";
Workbook workbook = new Workbook(designerFile);

// تعيين أشرطة التمرير
workbook.Settings.IsHScrollBarVisible = false;
workbook.Settings.IsVScrollBarVisible = false;

// استبدل سلسلة العنصر النائب بقيم جديدة
int newInt = 100;
workbook.Replace("OldInt", newInt);

string newString = "Hello!";
workbook.Replace("OldString", newString);
workbook.Save("result.xls");

[Visual Basic]

'افتح ملف المصمم
Dim designerFile as String = "\designer.xls"
Dim workbook as Workbook = new Workbook(designerFile)

'تعيين أشرطة التمرير
workbook.IsHScrollBarVisible = False
workbook.IsVScrollBarVisible = False

'استبدل سلسلة العنصر النائب بقيم جديدة
Dim newInt as Integer = 100
workbook.Replace("OldInt", newInt)

Dim newString as String = "Hello!"
workbook.Replace("OldString", newString)
workbook.Save("result.xls")    
```

### أنظر أيضا

* مساحة الاسم [Aspose.Cells](../../aspose.cells)
* المجسم [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
