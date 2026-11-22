---
title: "فئة Workbook"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Workbook. تمثل كائنًا أساسيًا لإنشاء جدول بيانات Excel"
type: docs
url: /ar/net/aspose.cells/workbook/
---
## Workbook class

يمثل كائنًا جذريًا لإنشاء جدول بيانات Excel.

```csharp
public class Workbook : IDisposable
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [Workbook](workbook/#constructor)() | يُنشئ مثيلًا جديدًا لفئة `Workbook`. |
| [Workbook](workbook/#constructor_1)(FileFormatType) | يُنشئ مثيلًا جديدًا لفئة `Workbook`. |
| [Workbook](workbook/#constructor_2)(LoadOptions) | يُنشئ مثيلًا جديدًا فارغًا لفئة `Workbook` مع خيارات |
| [Workbook](workbook/#constructor_3)(Stream) | يُنشئ مثيلًا جديدًا لفئة `Workbook` ويفتح تدفقًا. |
| [Workbook](workbook/#constructor_5)(string) | يُنشئ مثيلًا جديدًا لفئة `Workbook` ويفتح ملفًا. |
| [Workbook](workbook/#constructor_4)(Stream, LoadOptions) | يُهيئ نسخة جديدة من الفئة `Workbook` ويفتح الدفق. |
| [Workbook](workbook/#constructor_6)(string, LoadOptions) | يُنشئ مثيلًا جديدًا لفئة `Workbook` ويفتح ملفًا. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AbsolutePath](../../aspose.cells/workbook/absolutepath/) { get; set; } | يحصل على ويضبط المسار المطلق للملف. |
| [BuiltInDocumentProperties](../../aspose.cells/workbook/builtindocumentproperties/) { get; } | يعيد مجموعة [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) التي تمثل جميع خصائص المستند المدمجة في جدول البيانات. |
| [CellsDataTableFactory](../../aspose.cells/workbook/cellsdatatablefactory/) { get; } | يحصل على المصنع لبناء ICellsDataTable من الكائنات المخصصة |
| [Colors](../../aspose.cells/workbook/colors/) { get; } | يرجع الألوان في لوحة الألوان للجدول الإلكتروني. |
| [ContentTypeProperties](../../aspose.cells/workbook/contenttypeproperties/) { get; } | يحصل على قائمة كائنات [`ContentTypeProperty`](../../aspose.cells.properties/contenttypeproperty/) في المصنف. |
| [CountOfStylesInPool](../../aspose.cells/workbook/countofstylesinpool/) { get; } | يحصل على عدد الأنماط في مجموعة الأنماط. |
| [CustomDocumentProperties](../../aspose.cells/workbook/customdocumentproperties/) { get; } | يعيد مجموعة [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) التي تمثل جميع خصائص المستند المخصصة في جدول البيانات. |
| [CustomXmlParts](../../aspose.cells/workbook/customxmlparts/) { get; } | يمثل جزء تخزين بيانات XML مخصص (بيانات XML مخصصة داخل حزمة). |
| [DataConnections](../../aspose.cells/workbook/dataconnections/) { get; } | يحصل على مجموعة [`ExternalConnection`](../../aspose.cells.externalconnections/externalconnection/). |
| [DataMashup](../../aspose.cells/workbook/datamashup/) { get; } | يحصل على بيانات الدمج. |
| [DataModel](../../aspose.cells/workbook/datamodel/) { get; } | يحصل على نموذج البيانات في المصنف. |
| [DataSorter](../../aspose.cells/workbook/datasorter/) { get; } | يحصل على كائن DataSorter لفرز البيانات. |
| [DefaultStyle](../../aspose.cells/workbook/defaultstyle/) { get; set; } | يحصل على أو يضبط الكائن الافتراضي [`Style`](../style/) للمصنف. |
| [FileFormat](../../aspose.cells/workbook/fileformat/) { get; set; } | يحصل على ويضبط تنسيق الملف. |
| [FileName](../../aspose.cells/workbook/filename/) { get; set; } | يحصل على ويضبط اسم الملف الحالي. |
| [HasCustomFunction](../../aspose.cells/workbook/hascustomfunction/) { get; } | يكشف ما إذا كان هناك دالة مخصصة مستخدمة في هذا المصنف، مثل في صيغة الخلية أو في الأسماء المعرفة... |
| [HasMacro](../../aspose.cells/workbook/hasmacro/) { get; } | يشير إلى ما إذا كان هذا الجدول يحتوي على ماكرو/VBA. |
| [HasRevisions](../../aspose.cells/workbook/hasrevisions/) { get; } | يحصل على ما إذا كان المصنف يحتوي على أي تغييرات متتبعة |
| [InterruptMonitor](../../aspose.cells/workbook/interruptmonitor/) { get; set; } | يحصل على ويضبط مراقب المقاطعة. |
| [IsDigitallySigned](../../aspose.cells/workbook/isdigitallysigned/) { get; } | يشير إلى ما إذا كان هذا الجدول موقعًا رقمياً. |
| [IsLicensed](../../aspose.cells/workbook/islicensed/) { get; } | يشير إلى ما إذا تم ضبط الترخيص. |
| [IsWorkbookProtectedWithPassword](../../aspose.cells/workbook/isworkbookprotectedwithpassword/) { get; } | يشير إلى ما إذا كان الهيكل أو النافذة محميًا بكلمة مرور. |
| [RibbonXml](../../aspose.cells/workbook/ribbonxml/) { get; set; } | يحصل على ويضبط ملف XML الذي يحدد واجهة الشريط. |
| [Settings](../../aspose.cells/workbook/settings/) { get; } | يمثل إعدادات المصنف. |
| [Theme](../../aspose.cells/workbook/theme/) { get; } | يحصل على اسم السمة. |
| [VbaProject](../../aspose.cells/workbook/vbaproject/) { get; } | يحصل على [`VbaProject`](./vbaproject/) في جدول بيانات. |
| [Worksheets](../../aspose.cells/workbook/worksheets/) { get; } | يحصل على مجموعة [`WorksheetCollection`](../worksheetcollection/) في الجدول. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [AcceptAllRevisions](../../aspose.cells/workbook/acceptallrevisions/)() | يقبل جميع التغييرات المتتبعة في المصنف. |
| [AddDigitalSignature](../../aspose.cells/workbook/adddigitalsignature/)(DigitalSignatureCollection) | يضيف توقيعًا رقميًا إلى ملف جدول بيانات OOXML (Excel2007 وما بعده). |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula/#calculateformula)() | يحسب نتيجة الصيغ. |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula/#calculateformula_2)(bool) | يحسب نتيجة الصيغ. |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula/#calculateformula_1)(CalculationOptions) | يتم حساب الصيغ في هذا المصنف. |
| [ChangePalette](../../aspose.cells/workbook/changepalette/)(Color, int) | يغيّر لوحة الألوان لجدول البيانات في الفهرس المحدد. |
| [CloseAccessCache](../../aspose.cells/workbook/closeaccesscache/)(AccessCacheOptions) | يغلق الجلسة التي تستخدم الذاكرات المؤقتة للوصول إلى البيانات. |
| [Combine](../../aspose.cells/workbook/combine/)(Workbook) | يجمع كائن مصنف آخر. |
| [Copy](../../aspose.cells/workbook/copy/#copy)(Workbook) | ينسخ البيانات من كائن مصنف مصدر. |
| [Copy](../../aspose.cells/workbook/copy/#copy_1)(Workbook, CopyOptions) | ينسخ كائن مصنف آخر. |
| [CopyTheme](../../aspose.cells/workbook/copytheme/)(Workbook) | ينسخ السمة من مصنف آخر. |
| [CreateBuiltinStyle](../../aspose.cells/workbook/createbuiltinstyle/)(BuiltinStyleType) | ينشئ نمطًا مدمجًا حسب النوع المحدد. |
| [CreateCellsColor](../../aspose.cells/workbook/createcellscolor/)() | ينشئ كائن [`CellsColor`](../cellscolor/). |
| [CreateStyle](../../aspose.cells/workbook/createstyle/#createstyle)() | ينشئ نمطًا جديدًا. |
| [CreateStyle](../../aspose.cells/workbook/createstyle/#createstyle_1)(bool) | ينشئ نمطًا جديدًا. |
| [CustomTheme](../../aspose.cells/workbook/customtheme/)(string, Color[]) | يخصص السمة. |
| [Dispose](../../aspose.cells/workbook/dispose/)() | ينفّذ مهامًا معرفة من قبل التطبيق مرتبطة بتحرير أو إطلاق أو إعادة تعيين الموارد غير المُدارة. |
| [ExportXml](../../aspose.cells/workbook/exportxml/#exportxml)(string, Stream) | تصدير بيانات XML. |
| [ExportXml](../../aspose.cells/workbook/exportxml/#exportxml_1)(string, string) | تصدير بيانات XML المرتبطة بخريطة XML المحددة. |
| [GetDigitalSignature](../../aspose.cells/workbook/getdigitalsignature/)() | يحصل على التوقيع الرقمي من الملف. |
| [GetFonts](../../aspose.cells/workbook/getfonts/)() | يحصل على جميع الخطوط في مجموعة الأنماط. |
| [GetMatchingColor](../../aspose.cells/workbook/getmatchingcolor/)(Color) | ابحث عن أفضل لون مطابق في لوحة الألوان الحالية. |
| [GetNamedStyle](../../aspose.cells/workbook/getnamedstyle/)(string) | يحصل على النمط المسمى في مجموعة الأنماط. |
| [GetStyleInPool](../../aspose.cells/workbook/getstyleinpool/)(int) | يحصل على النمط في مجموعة الأنماط. سيتم جمع جميع الأنماط في المصنف في مجموعة. هناك فهرس إشارة بسيط فقط في الخلايا. |
| [GetThemeColor](../../aspose.cells/workbook/getthemecolor/)(ThemeColorType) | يحصل على لون السمة. |
| [HasExernalLinks](../../aspose.cells/workbook/hasexernallinks/)() | (**Obsolete.**) يشير إلى ما إذا كان هذا المصنف يحتوي على روابط خارجية إلى مصادر بيانات أخرى. |
| [ImportXml](../../aspose.cells/workbook/importxml/#importxml)(Stream, string, int, int) | يستورد/يحدّث ملف بيانات XML إلى المصنف. |
| [ImportXml](../../aspose.cells/workbook/importxml/#importxml_1)(string, string, int, int) | يستورد/يحدّث ملف بيانات XML إلى المصنف. |
| [IsColorInPalette](../../aspose.cells/workbook/iscolorinpalette/)(Color) | يتحقق مما إذا كان اللون موجودًا في لوحة ألوان جدول البيانات. |
| [MergeNamedStyles](../../aspose.cells/workbook/mergenamedstyles/)(Workbook) | يدمج الأنماط المسمّاة من ملف Excel الآخر. |
| [ParseFormulas](../../aspose.cells/workbook/parseformulas/)(bool) | يقوم بتحليل جميع الصيغ التي لم يتم تحليلها عندما تم تحميلها من ملف القالب أو تعيينها إلى خلية. |
| [Protect](../../aspose.cells/workbook/protect/)(ProtectionType, string) | يحمي مصنفًا. |
| [ProtectSharedWorkbook](../../aspose.cells/workbook/protectsharedworkbook/)(string) | يحمي مصنفًا مشتركًا. |
| [RefreshAll](../../aspose.cells/workbook/refreshall/)() | تحديث الأشكال المرتبطة، وجميع جداول المحور والرسوم البيانية مع مصدر المحور. |
| [RefreshDynamicArrayFormulas](../../aspose.cells/workbook/refreshdynamicarrayformulas/#refreshdynamicarrayformulas)(bool) | يقوم بتحديث صيغ المصفوفة الديناميكية (تنتشر إلى نطاق جديد من الخلايا المجاورة وفقًا للبيانات الحالية) لن يتم حساب الصيغ الأخرى في المصنف بشكل متكرر حتى إذا تم استخدامها بواسطة صيغ المصفوفة الديناميكية. |
| [RefreshDynamicArrayFormulas](../../aspose.cells/workbook/refreshdynamicarrayformulas/#refreshdynamicarrayformulas_1)(bool, CalculationOptions) | يقوم بتحديث صيغ المصفوفة الديناميكية (تنتشر إلى نطاق جديد من الخلايا المجاورة وفقًا للبيانات الحالية) |
| [RemoveDigitalSignature](../../aspose.cells/workbook/removedigitalsignature/)() | يزيل التوقيع الرقمي من هذه الورقة الإلكترونية. |
| [RemoveExternalLinks](../../aspose.cells/workbook/removeexternallinks/)() | (**Obsolete.**) يزيل جميع الروابط الخارجية في المصنف. |
| [RemoveMacro](../../aspose.cells/workbook/removemacro/)() | يزيل VBA/ماكرو من هذه الورقة الإلكترونية. |
| [RemovePersonalInformation](../../aspose.cells/workbook/removepersonalinformation/)() | يزيل المعلومات الشخصية. |
| [RemoveUnusedStyles](../../aspose.cells/workbook/removeunusedstyles/)() | إزالة جميع الأنماط غير المستخدمة. |
| [Replace](../../aspose.cells/workbook/replace/#replace)(bool, object) | يستبدل قيم الخلايا ببيانات جديدة. |
| [Replace](../../aspose.cells/workbook/replace/#replace_1)(int, object) | يستبدل قيم الخلايا ببيانات جديدة. |
| [Replace](../../aspose.cells/workbook/replace/#replace_6)(string, DataTable) | يستبدل قيم الخلايا ببيانات من DataTable. |
| [Replace](../../aspose.cells/workbook/replace/#replace_2)(string, double) | يستبدل قيمة خلية واحدة بقيمة مزدوجة جديدة. |
| [Replace](../../aspose.cells/workbook/replace/#replace_4)(string, int) | يستبدل قيمة خلية واحدة بعدد صحيح جديد. |
| [Replace](../../aspose.cells/workbook/replace/#replace_7)(string, string) | يستبدل قيمة خلية واحدة بسلسلة نصية جديدة. |
| [Replace](../../aspose.cells/workbook/replace/#replace_3)(string, double[], bool) | يستبدل قيم الخلايا بمصفوفة مزدوجة. |
| [Replace](../../aspose.cells/workbook/replace/#replace_5)(string, int[], bool) | يستبدل قيم الخلايا بمصفوفة أعداد صحيحة. |
| [Replace](../../aspose.cells/workbook/replace/#replace_8)(string, string, ReplaceOptions) | يستبدل قيمة خلية واحدة بسلسلة نصية جديدة. |
| [Replace](../../aspose.cells/workbook/replace/#replace_9)(string, string[], bool) | يستبدل قيمة خلية واحدة بمصفوفة سلاسل نصية جديدة. |
| [Save](../../aspose.cells/workbook/save/#save_2)(string) | احفظ المصنف على القرص. |
| [Save](../../aspose.cells/workbook/save/#save)(Stream, SaveFormat) | يحفظ المصنف إلى التدفق. |
| [Save](../../aspose.cells/workbook/save/#save_1)(Stream, SaveOptions) | يحفظ المصنف إلى التدفق. |
| [Save](../../aspose.cells/workbook/save/#save_3)(string, SaveFormat) | يحفظ المصنف على القرص. |
| [Save](../../aspose.cells/workbook/save/#save_4)(string, SaveOptions) | يحفظ المصنف على القرص. |
| [Save](../../aspose.cells/workbook/save/#save_5)(HttpResponse, string, ContentDisposition, SaveOptions) | ينشئ ورقة النتائج وينقلها إلى العميل ثم يفتحها في المتصفح أو MS Workbook. |
| [Save](../../aspose.cells/workbook/save/#save_6)(HttpResponse, string, ContentDisposition, SaveOptions, bool) | ينشئ ورقة النتائج وينقلها إلى العميل ثم يفتحها في المتصفح أو MS Workbook. |
| [SaveToStream](../../aspose.cells/workbook/savetostream/)() | يحفظ ملف Excel إلى كائن MemoryStream كملف Excel97-2003 xls ويعيده. |
| [SetDigitalSignature](../../aspose.cells/workbook/setdigitalsignature/)(DigitalSignatureCollection) | يحدد توقيعًا رقميًا لملف ورقة إلكترونية (Excel2007 وما بعده). |
| [SetEncryptionOptions](../../aspose.cells/workbook/setencryptionoptions/)(EncryptionType, int) | ضبط خيارات التشفير. |
| [SetThemeColor](../../aspose.cells/workbook/setthemecolor/)(ThemeColorType, Color) | يضبط لون السمة |
| [StartAccessCache](../../aspose.cells/workbook/startaccesscache/)(AccessCacheOptions) | يبدأ الجلسة التي تستخدم الذاكرة المؤقتة للوصول إلى البيانات. |
| [Unprotect](../../aspose.cells/workbook/unprotect/)(string) | يفك حماية مصنف. |
| [UnprotectSharedWorkbook](../../aspose.cells/workbook/unprotectsharedworkbook/)(string) | يفك حماية مصنف مشترك. |
| [UpdateCustomFunctionDefinition](../../aspose.cells/workbook/updatecustomfunctiondefinition/)(CustomFunctionDefinition) | يحدّث تعريف الدوال المخصصة. |
| [UpdateLinkedDataSource](../../aspose.cells/workbook/updatelinkeddatasource/)(Workbook[]) | إذا كان هذا المصنف يحتوي على روابط خارجية إلى مصدر بيانات آخر، سيحاول Aspose.Cells استرجاع أحدث البيانات من المصادر المعطاة. |

### ملاحظات

تشير فئة Workbook إلى جدول بيانات Excel. يمكن لكل جدول بيانات أن يحتوي على أوراق عمل متعددة. الميزة الأساسية للفئة هي فتح وحفظ ملفات Excel الأصلية. تحتوي الفئة على بعض الميزات المتقدمة مثل نسخ البيانات من Workbooks أخرى، دمج Workbooks، تحويل Excel إلى PDF، عرض Excel كصورة وحماية جدول بيانات Excel.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookDemo
    {
        public static void WorkbookExample()
        {
            // إنشاء نسخة جديدة من Workbook
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الافتراضية
            Worksheet worksheet = workbook.Worksheets[0];

            // ضبط بعض خصائص المصنف
            workbook.FileName = "ExampleWorkbook.xlsx";
            workbook.DefaultStyle.Font.Name = "Tahoma";

            // إضافة ورقة عمل جديدة
            int newSheetIndex = workbook.Worksheets.Add();
            Worksheet newWorksheet = workbook.Worksheets[newSheetIndex];
            newWorksheet.Name = "NewSheet";

            // إضافة بعض البيانات إلى ورقة العمل الجديدة
            newWorksheet.Cells["A1"].PutValue("Hello, Aspose.Cells!");

            // ضبط بعض خصائص المستند
            workbook.BuiltInDocumentProperties["Author"].Value = "John Smith";
            workbook.CustomDocumentProperties.Add("Checked by", "Jane");

            // حفظ المصنف إلى ملف
            workbook.Save("WorkbookExample.xlsx");

            // عرض بعض الخصائص
            Console.WriteLine("Workbook File Name: " + workbook.FileName);
            Console.WriteLine("Default Font: " + workbook.DefaultStyle.Font.Name);
            Console.WriteLine("Author: " + workbook.BuiltInDocumentProperties["Author"].Value);
            Console.WriteLine("Custom Property 'Checked by': " + workbook.CustomDocumentProperties["Checked by"].Value);

            // تحقق مما إذا كان المصنف مرخصًا
            Console.WriteLine("Is Licensed: " + workbook.IsLicensed);

            // تحقق مما إذا كان المصنف موقعًا رقميًا
            Console.WriteLine("Is Digitally Signed: " + workbook.IsDigitallySigned);

            // تحقق مما إذا كان المصنف يحتوي على ماكرو
            Console.WriteLine("Has Macros: " + workbook.HasMacro);

            // تحقق مما إذا كان المصنف يحتوي على أي تغييرات متتبعة
            Console.WriteLine("Has Revisions: " + workbook.HasRevisions);

            // تحقق من عدد الأنماط في مجموعة الأنماط
            Console.WriteLine("Number of Styles in Pool: " + workbook.CountOfStylesInPool);

            // تحقق من اسم السمة
            Console.WriteLine("Theme: " + workbook.Theme);

            // تحقق مما إذا كان المصنف محميًا بكلمة مرور
            Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);

            // تحقق مما إذا كان المصنف يحتوي على روابط خارجية
            Console.WriteLine("Has External Links: " + (workbook.Worksheets.ExternalLinks.Count > 0));

            // تخلص من المصنف
            workbook.Dispose();
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


