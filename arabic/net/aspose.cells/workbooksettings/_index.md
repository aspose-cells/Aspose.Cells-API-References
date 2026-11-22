---
title: "الفئة WorkbookSettings"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.WorkbookSettings. تمثل جميع إعدادات دفتر العمل"
type: docs
url: /ar/net/aspose.cells/workbooksettings/
---
## WorkbookSettings class

يمثل جميع إعدادات المصنف.

```csharp
public class WorkbookSettings : IDisposable
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Author](../../aspose.cells/workbooksettings/author/) { get; set; } | يحصل على مؤلف الملف ويضبطه. |
| [AutoCompressPictures](../../aspose.cells/workbooksettings/autocompresspictures/) { get; set; } | يحدد قيمة منطقية تشير إلى أن التطبيق يضغط الصور تلقائيًا في دفتر العمل. |
| [AutoRecover](../../aspose.cells/workbooksettings/autorecover/) { get; set; } | يشير إلى ما إذا كان الملف معلمًا للاستعادة التلقائية. |
| [BuildVersion](../../aspose.cells/workbooksettings/buildversion/) { get; set; } | يحدد الإصدار العام المتزايد للتطبيق. |
| [CheckCompatibility](../../aspose.cells/workbooksettings/checkcompatibility/) { get; set; } | يشير إلى ما إذا كان يتم فحص التوافق مع الإصدارات السابقة عند حفظ المصنف. |
| [CheckCustomNumberFormat](../../aspose.cells/workbooksettings/checkcustomnumberformat/) { get; set; } | يشير إلى ما إذا كان يتم فحص تنسيق الأرقام المخصص عند تعيين Style.Custom. |
| [CheckExcelRestriction](../../aspose.cells/workbooksettings/checkexcelrestriction/) { get; set; } | ما إذا كان يتم فحص قيود ملف Excel عندما يقوم المستخدم بتعديل الكائنات المتعلقة بالخلايا. على سبيل المثال، لا يسمح Excel بإدخال قيمة نصية أطول من 32 كيلوبايت. عندما تُدخل قيمة أطول من 32 كيلوبايت مثلًا باستخدام Cell.PutValue(string)، إذا كانت هذه الخاصية true، ستحصل على استثناء. إذا كانت false، سنقبل قيمة النص المدخلة كقيمة الخلية بحيث يمكنك لاحقًا إخراج القيمة النصية الكاملة إلى صيغ ملفات أخرى مثل CSV. ومع ذلك، إذا قمت بتعيين قيمة غير صالحة لتنسيق ملف Excel، يجب ألا تحفظ المصنف بتنسيق Excel لاحقًا. وإلا قد يحدث خطأ غير متوقع في ملف Excel المُنشأ. |
| [Compliance](../../aspose.cells/workbooksettings/compliance/) { get; set; } | يحدد إصدار OOXML للمستند الناتج. القيمة الافتراضية هي Ecma376_2006. |
| [CrashSave](../../aspose.cells/workbooksettings/crashsave/) { get; set; } | يشير إلى ما إذا كان التطبيق قد حفظ ملف المصنف آخر مرة بعد تعطل. |
| [CultureInfo](../../aspose.cells/workbooksettings/cultureinfo/) { get; set; } | يحصل أو يعيّن معلومات الثقافة للنظام. |
| [DataExtractLoad](../../aspose.cells/workbooksettings/dataextractload/) { get; set; } | يشير إلى ما إذا كان التطبيق قد فتح المصنف آخر مرة لاستعادة البيانات. |
| [Date1904](../../aspose.cells/workbooksettings/date1904/) { get; set; } | يحصل أو يعيّن قيمة تمثل ما إذا كان المصنف يستخدم نظام التاريخ 1904. |
| [DefaultImageResolution](../../aspose.cells/workbooksettings/defaultimageresolution/) { get; set; } | يحصل ويعيّن الدقة الافتراضية للصورة. |
| [DefaultStyleSettings](../../aspose.cells/workbooksettings/defaultstylesettings/) { get; } | يحصل على الإعدادات للقيم الافتراضية للخصائص المتعلقة بالنمط لهذا المصنف. |
| [DiscardImageEditData](../../aspose.cells/workbooksettings/discardimageeditdata/) { get; set; } | يشير إلى ما إذا كان يتم تجاهل بيانات تحرير الصورة. |
| [DisplayDrawingObjects](../../aspose.cells/workbooksettings/displaydrawingobjects/) { get; set; } | يشير إلى ما إذا كان وكيفية عرض الكائنات في المصنف. |
| [EnableMacros](../../aspose.cells/workbooksettings/enablemacros/) { get; set; } | تمكين الماكرو؛ |
| [FirstVisibleTab](../../aspose.cells/workbooksettings/firstvisibletab/) { get; set; } | يحصل أو يعيّن أول تبويب ورقة عمل مرئي. |
| [FormulaSettings](../../aspose.cells/workbooksettings/formulasettings/) { get; } | يحصل على الإعدادات للميزات المتعلقة بالمعادلات. |
| [GlobalizationSettings](../../aspose.cells/workbooksettings/globalizationsettings/) { get; set; } | يحصل ويعيّن إعدادات العولمة. |
| [HidePivotFieldList](../../aspose.cells/workbooksettings/hidepivotfieldlist/) { get; set; } | يحصل ويعيّن ما إذا كان يتم إخفاء قائمة الحقول لجدول PivotTable. |
| [IsDefaultEncrypted](../../aspose.cells/workbooksettings/isdefaultencrypted/) { get; set; } | يشير إلى ما إذا كان يتم تشفير المصنف باستخدام كلمة مرور افتراضية إذا تم قفل بنية المصنف والنوافذ. |
| [IsEncrypted](../../aspose.cells/workbooksettings/isencrypted/) { get; } | يحصل على قيمة تشير إلى ما إذا كانت كلمة المرور مطلوبة لفتح هذا المصنف. |
| [IsHidden](../../aspose.cells/workbooksettings/ishidden/) { get; set; } | يشير إلى ما إذا كان هذا المصنف مخفيًا. |
| [IsHScrollBarVisible](../../aspose.cells/workbooksettings/ishscrollbarvisible/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان الجدول الإلكتروني المُنشأ سيحتوي على شريط تمرير أفقي. |
| [IsMinimized](../../aspose.cells/workbooksettings/isminimized/) { get; set; } | يمثل ما إذا كان الجدول الإلكتروني المُنشأ سيفتح مصغّرًا. |
| [IsProtected](../../aspose.cells/workbooksettings/isprotected/) { get; } | يحصل على قيمة تشير إلى ما إذا كانت بنية أو نافذة المصنف محمية. |
| [IsVScrollBarVisible](../../aspose.cells/workbooksettings/isvscrollbarvisible/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كان جدول البيانات المُولد سيحتوي على شريط تمرير عمودي. |
| [LanguageCode](../../aspose.cells/workbooksettings/languagecode/) { get; set; } | يحصل أو يضبط لغة واجهة المستخدم لإصدار Workbook بناءً على رمز البلد (CountryCode) الذي حفظ الملف. |
| [MaxColumn](../../aspose.cells/workbooksettings/maxcolumn/) { get; } | يحصل على أقصى فهرس للعمود، يبدأ من الصفر. |
| [MaxRow](../../aspose.cells/workbooksettings/maxrow/) { get; } | يحصل على أقصى فهرس للصف، يبدأ من الصفر. |
| [MaxRowsOfSharedFormula](../../aspose.cells/workbooksettings/maxrowsofsharedformula/) { get; set; } | يحصل أو يضبط أقصى رقم للصف للمعادلة المشتركة. |
| [MaxUniqueItemsPerField](../../aspose.cells/workbooksettings/maxuniqueitemsperfield/) { get; set; } | يحصل أو يضبط حد العناصر الفريدة لكل حقل |
| [MemorySetting](../../aspose.cells/workbooksettings/memorysetting/) { get; set; } | يحصل أو يضبط خيارات استخدام الذاكرة. سيتم اعتبار الخيار الجديد كخيار افتراضي للأوراق العمل التي تم إنشاؤها حديثًا لكنه لا يؤثر على الأوراق الموجودة. |
| [NumberDecimalSeparator](../../aspose.cells/workbooksettings/numberdecimalseparator/) { get; set; } | يحصل أو يضبط الفاصل العشري لتنسيق/تحليل القيم الرقمية. الافتراضي هو الفاصل العشري للمنطقة الحالية. |
| [NumberGroupSeparator](../../aspose.cells/workbooksettings/numbergroupseparator/) { get; set; } | يحصل أو يضبط الحرف الذي يفصل مجموعات الأرقام إلى يسار الفاصل العشري في القيم الرقمية. الافتراضي هو فاصل المجموعات للمنطقة الحالية. |
| [PaperSize](../../aspose.cells/workbooksettings/papersize/) { get; set; } | يحصل أو يضبط حجم ورق الطباعة الافتراضي. |
| [Password](../../aspose.cells/workbooksettings/password/) { get; set; } | يمثل كلمة مرور تشفير ملف Workbook. |
| [PropertiesFollowChartPoint](../../aspose.cells/workbooksettings/propertiesfollowchartpoint/) { get; set; } | يشير إلى ما إذا كانت خصائص نقاط البيانات وتسميات البيانات في جميع المخططات في هذا المصنف تتبع مرجعها. |
| [ProtectionType](../../aspose.cells/workbooksettings/protectiontype/) { get; } | يحصل على نوع الحماية للمصنف. |
| [QuotePrefixToStyle](../../aspose.cells/workbooksettings/quoteprefixtostyle/) { get; set; } | يشير إلى ما إذا كان ضبط خاصية [`QuotePrefix`](../style/quoteprefix/) عند إدخال قيمة النص (التي تبدأ بعلامة اقتباس مفردة) إلى الخلية |
| [Region](../../aspose.cells/workbooksettings/region/) { get; set; } | يحصل أو يضبط الإعدادات الإقليمية للمصنف. |
| [RemovePersonalInformation](../../aspose.cells/workbooksettings/removepersonalinformation/) { get; set; } | صحيح إذا كان يمكن إزالة المعلومات الشخصية من المصنف المحدد. |
| [RepairLoad](../../aspose.cells/workbooksettings/repairload/) { get; set; } | يشير إلى ما إذا كان التطبيق قد فتح المصنف آخر مرة في وضع الأمان أو الإصلاح. |
| [ResourceProvider](../../aspose.cells/workbooksettings/resourceprovider/) { get; set; } | يحصل أو يضبط موفر الدفق للموارد الخارجية، مثل تحميل بيانات الصورة للصور من النوع "LinkToFile". |
| [ShapeDisplayType](../../aspose.cells/workbooksettings/shapedisplaytype/) { get; set; } | يحصل أو يضبط طريقة عرض التطبيق للأشكال في هذا المصنف |
| [Shared](../../aspose.cells/workbooksettings/shared/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كان Workbook مشتركًا. |
| [SheetTabBarWidth](../../aspose.cells/workbooksettings/sheettabbarwidth/) { get; set; } | عرض شريط علامات تبويب ورقة العمل (بـ 1/1000 من عرض النافذة). |
| [ShowTabs](../../aspose.cells/workbooksettings/showtabs/) { get; set; } | يحصل أو يضبط قيمة ما إذا كانت علامات تبويب Workbook معروضة. |
| [SignificantDigits](../../aspose.cells/workbooksettings/significantdigits/) { get; set; } | (**Obsolete.**) يحصل أو يضبط عدد الأرقام المهمة. القيمة الافتراضية هي [`SignificantDigits`](../cellshelper/significantdigits/). |
| [SignificantDigitsType](../../aspose.cells/workbooksettings/significantdigitstype/) { get; set; } | يحصل أو يضبط نوع الأرقام المهمة لإخراج القيم الرقمية في هذا المصنف. القيمة الافتراضية هي [`SignificantDigitsType`](../cellshelper/significantdigitstype/). |
| [SmartTagOptions](../../aspose.cells/workbooksettings/smarttagoptions/) { get; } | يحصل على خيارات العلامة الذكية. |
| [StreamProvider](../../aspose.cells/workbooksettings/streamprovider/) { get; set; } | (**Obsolete.**) يحصل ويضبط موفر الدفق للموارد الخارجية. |
| [UpdateAdjacentCellsBorder](../../aspose.cells/workbooksettings/updateadjacentcellsborder/) { get; set; } | يشير إلى ما إذا كان يتم تحديث حد الخلايا المجاورة. |
| [UpdateLinksType](../../aspose.cells/workbooksettings/updatelinkstype/) { get; set; } | يحصل ويضبط كيفية تحديث الروابط الخارجية عند فتح دفتر العمل. |
| [WarningCallback](../../aspose.cells/workbooksettings/warningcallback/) { get; set; } | يحصل أو يضبط رد النداء التحذيري. |
| [WindowHeight](../../aspose.cells/workbooksettings/windowheight/) { get; set; } | ارتفاع النافذة، بوحدة النقطة. |
| [WindowHeightCM](../../aspose.cells/workbooksettings/windowheightcm/) { get; set; } | ارتفاع النافذة، بوحدة السنتيمتر. |
| [WindowHeightInch](../../aspose.cells/workbooksettings/windowheightinch/) { get; set; } | ارتفاع النافذة، بوحدة البوصة. |
| [WindowLeft](../../aspose.cells/workbooksettings/windowleft/) { get; set; } | المسافة من الحافة اليسرى لمنطقة العميل إلى الحافة اليسرى للنافذة، بوحدة النقطة. |
| [WindowLeftCM](../../aspose.cells/workbooksettings/windowleftcm/) { get; set; } | المسافة من الحافة اليسرى لمنطقة العميل إلى الحافة اليسرى للنافذة. بوحدة السنتيمتر. |
| [WindowLeftInch](../../aspose.cells/workbooksettings/windowleftinch/) { get; set; } | المسافة من الحافة اليسرى لمنطقة العميل إلى الحافة اليسرى للنافذة. بوحدة البوصة. |
| [WindowTop](../../aspose.cells/workbooksettings/windowtop/) { get; set; } | المسافة من الحافة العليا لمنطقة العميل إلى الحافة العليا للنافذة، بوحدة النقطة. |
| [WindowTopCM](../../aspose.cells/workbooksettings/windowtopcm/) { get; set; } | المسافة من الحافة العليا لمنطقة العميل إلى الحافة العليا للنافذة، بوحدة السنتيمتر. |
| [WindowTopInch](../../aspose.cells/workbooksettings/windowtopinch/) { get; set; } | المسافة من الحافة العليا لمنطقة العميل إلى الحافة العليا للنافذة، بوحدة البوصة. |
| [WindowWidth](../../aspose.cells/workbooksettings/windowwidth/) { get; set; } | عرض النافذة، بوحدة النقطة. |
| [WindowWidthCM](../../aspose.cells/workbooksettings/windowwidthcm/) { get; set; } | عرض النافذة، بوحدة السنتيمتر. |
| [WindowWidthInch](../../aspose.cells/workbooksettings/windowwidthinch/) { get; set; } | عرض النافذة، بوحدة البوصة. |
| [WpsCompatibility](../../aspose.cells/workbooksettings/wpscompatibility/) { get; set; } | يشير إلى ما إذا كان متوافقًا مع WPS. |
| [WriteProtection](../../aspose.cells/workbooksettings/writeprotection/) { get; } | يوفر الوصول إلى خيارات حماية الكتابة لدفتر العمل. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Dispose](../../aspose.cells/workbooksettings/dispose/)() | يطلق الموارد. |
| [GetThemeFont](../../aspose.cells/workbooksettings/getthemefont/)(FontSchemeType) | يحصل على اسم خط السمة الافتراضي. |
| [SetPageOrientationType](../../aspose.cells/workbooksettings/setpageorientationtype/)(PageOrientationType) | ضبط نوع اتجاه الطباعة لكامل دفتر العمل. |

### أمثلة

```csharp
using Aspose.Cells;
using System;
using System.Globalization;

public class WorkbookSettingsDemo
{
    public static void RunDemo()
    {
        // إنشاء دفتر عمل جديد
        Workbook workbook = new Workbook();
        Worksheet sheet = workbook.Worksheets[0];

        // أضف بعض البيانات التجريبية
        sheet.Cells["A1"].PutValue("Sample Data");
        sheet.Cells["A2"].PutValue(123);
        sheet.Cells["A3"].PutValue(DateTime.Now);

        // الوصول إلى WorkbookSettings
        WorkbookSettings settings = workbook.Settings;

        // ضبط إعدادات مختلفة
        settings.Author = "John Doe";
        settings.CheckCustomNumberFormat = true;
        settings.EnableMacros = false;
        settings.Date1904 = false;
        settings.DisplayDrawingObjects = DisplayDrawingObjects.DisplayShapes;
        settings.SheetTabBarWidth = 1000;
        settings.ShowTabs = true;
        settings.FirstVisibleTab = 0;
        settings.IsHScrollBarVisible = true;
        settings.IsVScrollBarVisible = true;
        settings.Shared = false;
        settings.LanguageCode = CountryCode.USA;
        settings.Region = CountryCode.USA;
        settings.CultureInfo = new CultureInfo("en-US");
        settings.GlobalizationSettings = new GlobalizationSettings();
        settings.NumberDecimalSeparator = '.';
        settings.NumberGroupSeparator = ',';
        settings.Password = "password123";
        settings.IsDefaultEncrypted = false;
        settings.IsMinimized = false;
        settings.IsHidden = false;
        settings.AutoCompressPictures = true;
        settings.RemovePersonalInformation = false;
        settings.HidePivotFieldList = false;
        settings.UpdateLinksType = UpdateLinksType.UserSet;
        settings.WindowLeft = 0;
        settings.WindowLeftInch = 0;
        settings.WindowLeftCM = 0;
        settings.WindowTop = 0;
        settings.WindowTopInch = 0;
        settings.WindowTopCM = 0;
        settings.WindowWidth = 800;
        settings.WindowWidthInch = 8;
        settings.WindowWidthCM = 20.32;
        settings.WindowHeight = 600;
        settings.WindowHeightInch = 6;
        settings.WindowHeightCM = 15.24;
        settings.UpdateAdjacentCellsBorder = true;
        settings.SignificantDigits = 15;
        settings.CheckCompatibility = true;
        settings.CheckExcelRestriction = true;
        settings.AutoRecover = true;
        settings.CrashSave = false;
        settings.DataExtractLoad = false;
        settings.RepairLoad = false;
        settings.BuildVersion = "1.0.0";
        settings.MemorySetting = MemorySetting.Normal;
        settings.PaperSize = PaperSizeType.PaperA4;
        settings.WarningCallback = null;
        settings.MaxRowsOfSharedFormula = 1048576;
        settings.Compliance = OoxmlCompliance.Ecma376_2006;
        settings.QuotePrefixToStyle = false;

        // احفظ المصنف
        workbook.Save("WorkbookSettingsDemo.xlsx");
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


