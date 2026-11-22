---
title: "الفئة CellsHelper"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.CellsHelper. توفر وظائف مساعدة"
type: docs
url: /ar/net/aspose.cells/cellshelper/
---
## CellsHelper class

يوفر وظائف مساعدة.

```csharp
public class CellsHelper
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| static [AltStartPath](../../aspose.cells/cellshelper/altstartpath/) { get; set; } | يحصل أو يعيّن مسار بدء التشغيل البديل، الذي يُشار إليه من قبل بعض مراجع الصيغ الخارجية. |
| static [CustomImplementationFactory](../../aspose.cells/cellshelper/customimplementationfactory/) { get; set; } | يحصل أو يعيّن المصنع لإنشاء مثيلات بتنفيذ خاص. |
| static [DPI](../../aspose.cells/cellshelper/dpi/) { get; set; } | يحصل على DPI للجهاز. |
| static [IsCloudPlatform](../../aspose.cells/cellshelper/iscloudplatform/) { get; set; } | يرجى تعيين هذه الخاصية إلى True عند التشغيل على منصة سحابة، مثل: Azure، AWSLambda، إلخ، |
| static [LibraryPath](../../aspose.cells/cellshelper/librarypath/) { get; set; } | يحصل أو يعيّن مسار المكتبة الذي يُشار إليه من قبل بعض مراجع الصيغ الخارجية. |
| static [SignificantDigits](../../aspose.cells/cellshelper/significantdigits/) { get; set; } | (**Obsolete.**) يحصل ويعيّن عدد الأرقام ذات الدقة. القيمة الافتراضية هي 17. |
| static [SignificantDigitsType](../../aspose.cells/cellshelper/significantdigitstype/) { get; set; } | يحصل ويعيّن النوع الافتراضي للأرقام ذات الدقة لإخراج القيم الرقمية. القيمة الافتراضية هي G17. |
| static [StartupPath](../../aspose.cells/cellshelper/startuppath/) { get; set; } | يحصل أو يعيّن مسار بدء التشغيل، الذي يُشار إليه من قبل بعض مراجع الصيغ الخارجية. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| static [AddAddInFunction](../../aspose.cells/cellshelper/addaddinfunction/)(string, int, int, ParameterType[], ParameterType) | (**Obsolete.**) أضف وظيفة الإضافة. |
| static [CellIndexToName](../../aspose.cells/cellshelper/cellindextoname/)(int, int) | يحصل على اسم الخلية وفقًا لمؤشرات الصف والعمود. |
| static [CellNameToIndex](../../aspose.cells/cellshelper/cellnametoindex/)(string, out int, out int) | يحصل على مؤشرات الصف والعمود للخلية وفقًا لاسمها. |
| static [ColumnIndexToName](../../aspose.cells/cellshelper/columnindextoname/)(int) | يحصل على اسم العمود وفقًا لمؤشر العمود. |
| static [ColumnNameToIndex](../../aspose.cells/cellshelper/columnnametoindex/)(string) | يحصل على مؤشر العمود وفقًا لاسم العمود. |
| static [ConvertA1FormulaToR1C1](../../aspose.cells/cellshelper/converta1formulator1c1/)(string, int, int) | (**Obsolete.**) يحوّل صيغة A1 للخلية إلى صيغة r1c1. |
| static [ConvertR1C1FormulaToA1](../../aspose.cells/cellshelper/convertr1c1formulatoa1/)(string, int, int) | (**Obsolete.**) يحوّل صيغة r1c1 للخلية إلى صيغة A1. |
| static [CreateSafeSheetName](../../aspose.cells/cellshelper/createsafesheetname/#createsafesheetname)(string) | يتحقق من اسم الورقة المُعطى وينشئ اسمًا صالحًا عند الحاجة. إذا كان اسم الورقة المُعطى يتوافق مع قواعد أسماء أوراق Excel، يتم إرجاعه. وإلا سيتم قص السلسلة إذا تجاوز طولها الحد المسموح وسيتم استبدال الأحرف غير الصالحة بـ ' ', ثم إرجاع قيمة السلسلة المعاد بناؤها. |
| static [CreateSafeSheetName](../../aspose.cells/cellshelper/createsafesheetname/#createsafesheetname_1)(string, char) | يتحقق من اسم الورقة المُعطى وينشئ اسمًا صالحًا عند الحاجة. إذا كان اسم الورقة المُعطى يتوافق مع قواعد أسماء أوراق Excel، يتم إرجاعه. وإلا سيتم قص السلسلة إذا تجاوز طولها الحد المسموح وسيتم استبدال الأحرف غير الصالحة بالحرف المُعطى، ثم إرجاع قيمة السلسلة المعاد بناؤها. |
| static [GetCacheFolder](../../aspose.cells/cellshelper/getcachefolder/)() | يحصل على المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة تخزين مؤقت للبيانات. |
| static [GetDateTimeFromDouble](../../aspose.cells/cellshelper/getdatetimefromdouble/)(double, bool) | حوّل القيمة المزدوجة إلى قيمة تاريخ ووقت. |
| static [GetDoubleFromDateTime](../../aspose.cells/cellshelper/getdoublefromdatetime/)(DateTime, bool) | حوّل التاريخ والوقت إلى قيمة مزدوجة. |
| static [GetTextWidth](../../aspose.cells/cellshelper/gettextwidth/)(string, Font, double) | احصل على عرض النص بوحدة النقاط. |
| static [GetUsedColors](../../aspose.cells/cellshelper/getusedcolors/)(Workbook) | يحصل على جميع الألوان المستخدمة في دفتر العمل. |
| static [GetVersion](../../aspose.cells/cellshelper/getversion/)() | احصل على نسخة الإصدار. |
| static [MergeFiles](../../aspose.cells/cellshelper/mergefiles/)(string[], string, string) | يدمج بعض ملفات xls الكبيرة إلى ملف xls واحد. |
| static [NeedQuoteInFormula](../../aspose.cells/cellshelper/needquoteinformula/)(string) | يحدد ما إذا كان يجب إغلاق اسم الورقة بين علامات اقتباس مفردة |
| static [RowIndexToName](../../aspose.cells/cellshelper/rowindextoname/)(int) | يحصل على اسم الصف وفقًا لمؤشر الصف. |
| static [RowNameToIndex](../../aspose.cells/cellshelper/rownametoindex/)(string) | يحصل على مؤشر الصف وفقًا لاسم الصف. |
| static [SetCacheFolder](../../aspose.cells/cellshelper/setcachefolder/)(string) | يضبط المجلد للملفات المؤقتة التي قد تُستخدم كذاكرة تخزين مؤقت للبيانات. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperDemo
    {
        public static void CellsHelperExample()
        {
            // ضبط خصائص CellsHelper
            CellsHelper.SignificantDigits = 15;
            CellsHelper.DPI = 96.0;
            CellsHelper.StartupPath = "C:\\Program Files\\Aspose\\Cells";
            CellsHelper.AltStartPath = "D:\\Aspose\\Cells";
            CellsHelper.LibraryPath = "E:\\Aspose\\Cells\\Library";
            CellsHelper.IsCloudPlatform = true;

            // افتراض أن CustomImplementationFactory معرفة ومُنشأة مسبقًا في مكان آخر
            CellsHelper.CustomImplementationFactory = new CustomImplementationFactory();

            // عرض استخدام خصائص CellsHelper
            Console.WriteLine("Significant Digits: " + CellsHelper.SignificantDigits);
            Console.WriteLine("DPI: " + CellsHelper.DPI);
            Console.WriteLine("Startup Path: " + CellsHelper.StartupPath);
            Console.WriteLine("Alternate Startup Path: " + CellsHelper.AltStartPath);
            Console.WriteLine("Library Path: " + CellsHelper.LibraryPath);
            Console.WriteLine("Is Cloud Platform: " + CellsHelper.IsCloudPlatform);

            // مثال على استخدام CustomImplementationFactory
            var memoryStream = CellsHelper.CustomImplementationFactory.CreateMemoryStream();
            Console.WriteLine("MemoryStream created with CustomImplementationFactory: " + (memoryStream != null));

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


