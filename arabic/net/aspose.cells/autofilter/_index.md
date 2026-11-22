---
title: "الفئة AutoFilter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.AutoFilter. تمثل التصفية التلقائية للورقة المحددة"
type: docs
url: /ar/net/aspose.cells/autofilter/
---
## AutoFilter class

يمثل الترشيح التلقائي للورقة المحددة.

```csharp
public class AutoFilter
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [FilterColumns](../../aspose.cells/autofilter/filtercolumns/) { get; } | يحصل على مجموعة أعمدة الفلتر. |
| [Range](../../aspose.cells/autofilter/range/) { get; set; } | يمثل النطاق الذي ينطبق عليه AutoFilter المحدد. |
| [ShowFilterButton](../../aspose.cells/autofilter/showfilterbutton/) { get; set; } | يشير إلى ما إذا كان زر AutoFilter لهذا العمود مرئيًا. |
| [Sorter](../../aspose.cells/autofilter/sorter/) { get; } | يحصل على مُرتّب البيانات. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [AddDateFilter](../../aspose.cells/autofilter/adddatefilter/)(int, DateTimeGroupingType, int, int, int, int, int, int) | يضيف مرشح تاريخ. |
| [AddFillColorFilter](../../aspose.cells/autofilter/addfillcolorfilter/)(int, BackgroundType, CellsColor, CellsColor) | يضيف مرشح لون تعبئة. |
| [AddFilter](../../aspose.cells/autofilter/addfilter/)(int, string) | يضيف مرشحًا لعمود الفلتر. |
| [AddFontColorFilter](../../aspose.cells/autofilter/addfontcolorfilter/)(int, CellsColor) | يضيف مرشح لون الخط. |
| [AddIconFilter](../../aspose.cells/autofilter/addiconfilter/)(int, IconSetType, int) | يضيف مرشح أيقونة. |
| [Custom](../../aspose.cells/autofilter/custom/#custom)(int, FilterOperatorType, object) | يفلتر قائمة بمعيار مخصص. |
| [Custom](../../aspose.cells/autofilter/custom/#custom_1)(int, FilterOperatorType, object, bool, FilterOperatorType, object) | يفلتر قائمة بمعايير مخصصة. |
| [DynamicFilter](../../aspose.cells/autofilter/dynamicfilter/)(int, DynamicFilterType) | يضيف مرشحًا ديناميكيًا. |
| [Filter](../../aspose.cells/autofilter/filter/)(int, string) | يفلتر قائمة بمعايير محددة. |
| [FilterTop10](../../aspose.cells/autofilter/filtertop10/)(int, bool, bool, int) | تصفية أعلى 10 عناصر في القائمة. |
| [GetCellArea](../../aspose.cells/autofilter/getcellarea/#getcellarea)() | يحصل على [`CellArea`](../cellarea/) حيث ينطبق هذا AutoFilter. |
| [GetCellArea](../../aspose.cells/autofilter/getcellarea/#getcellarea_1)(bool) | يحصل على [`CellArea`](../cellarea/) حيث ينطبق AutoFilter المحدد. |
| [MatchBlanks](../../aspose.cells/autofilter/matchblanks/)(int) | مطابقة جميع الخلايا الفارغة في القائمة. |
| [MatchNonBlanks](../../aspose.cells/autofilter/matchnonblanks/)(int) | مطابقة جميع الخلايا غير الفارغة في القائمة. |
| [Refresh](../../aspose.cells/autofilter/refresh/#refresh)() | تحديث الفلاتر التلقائية لإخفاء أو إظهار الصفوف. |
| [Refresh](../../aspose.cells/autofilter/refresh/#refresh_1)(bool) | يحصل على مؤشرات جميع الصفوف المخفية. |
| [RemoveDateFilter](../../aspose.cells/autofilter/removedatefilter/)(int, DateTimeGroupingType, int, int, int, int, int, int) | يزيل مرشح تاريخ. |
| [RemoveFilter](../../aspose.cells/autofilter/removefilter/#removefilter)(int) | يزيل الفلتر المحدد. |
| [RemoveFilter](../../aspose.cells/autofilter/removefilter/#removefilter_1)(int, string) | يزيل مرشحًا لعمود الفلتر. |
| [SetRange](../../aspose.cells/autofilter/setrange/)(int, int, int) | يحدد النطاق الذي ينطبق عليه AutoFilter المحدد. |
| [ShowAll](../../aspose.cells/autofilter/showall/)() | إظهار جميع الصفوف. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterDemo
    {
        public static void AutoFilterExample()
        {
            // إنشاء تدفق ملف يحتوي على ملف Excel الذي سيتم فتحه
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // الوصول إلى ورقة العمل الأولى في ملف Excel
            Worksheet worksheet = workbook.Worksheets[0];
            // إنشاء AutoFilter عن طريق تحديد نطاق الخلايا لصف العنوان
            worksheet.AutoFilter.Range = "A1:B8";
            // تصفية الأعمدة بالقيم المحددة
            worksheet.AutoFilter.Filter(0, "Bananas");
            worksheet.AutoFilter.Refresh();

            // حفظ ملف Excel المعدل.
            workbook.Save("AutoFilterExample.xlsx");
            workbook.Save("AutoFilterExample.pdf");

            // إنشاء كائن Workbook
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // الوصول إلى ورقة العمل الأولى في ملف Excel
            worksheet = workbook.Worksheets[0];

            // كود إضافي لعرض وظائف أخرى لـ AutoFilter
            // تحديد النطاق لـ AutoFilter
            worksheet.AutoFilter.Range = "A1:B8";
            // إضافة مرشح
            worksheet.AutoFilter.AddFilter(0, "Apples");
            // إضافة مرشح تاريخ
            worksheet.AutoFilter.AddDateFilter(1, DateTimeGroupingType.Year, 2022, 0, 0, 0, 0, 0);

            worksheet.AutoFilter.Refresh();
            // حفظ ملف Excel المعدل.
            workbook.Save("AutoFilterExample2.xlsx");
            workbook.Save("AutoFilterExample2.pdf");

            // إنشاء كائن Workbook
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // الوصول إلى ورقة العمل الأولى في ملف Excel
            worksheet = workbook.Worksheets[0];
                        
            // إضافة مرشح لون الخط
            CellsColor color = workbook.CreateCellsColor();
            color.Color = System.Drawing.Color.Red;

            worksheet.AutoFilter.AddFontColorFilter(0, color);

            worksheet.AutoFilter.Refresh();
            // حفظ ملف Excel المعدل.
            workbook.Save("AutoFilterExample3.xlsx");
            workbook.Save("AutoFilterExample3.pdf");

            // إنشاء كائن Workbook
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // الوصول إلى ورقة العمل الأولى في ملف Excel
            worksheet = workbook.Worksheets[0];

            // إضافة مرشح لون التعبئة
            CellsColor foregroundColor = workbook.CreateCellsColor();
            foregroundColor.Color = System.Drawing.Color.Red;
            CellsColor backgroundColor = workbook.CreateCellsColor();
            backgroundColor.Color = System.Drawing.Color.White;

            worksheet.AutoFilter.AddFillColorFilter(0, BackgroundType.Solid, foregroundColor, backgroundColor);

            worksheet.AutoFilter.Refresh();
            // حفظ ملف Excel المعدل.
            workbook.Save("AutoFilterExample4.xlsx");
            workbook.Save("AutoFilterExample4.pdf");

            // إنشاء كائن Workbook
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // الوصول إلى ورقة العمل الأولى في ملف Excel
            worksheet = workbook.Worksheets[0];

            // مطابقة الخلايا الفارغة
            worksheet.AutoFilter.MatchBlanks(0);

            worksheet.AutoFilter.Refresh();
            // حفظ ملف Excel المعدل.
            workbook.Save("AutoFilterExample5.xlsx");
            workbook.Save("AutoFilterExample5.pdf");

            // إنشاء كائن Workbook
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // الوصول إلى ورقة العمل الأولى في ملف Excel
            worksheet = workbook.Worksheets[0];

            // مطابقة الخلايا غير الفارغة
            worksheet.AutoFilter.MatchNonBlanks(0);

            worksheet.AutoFilter.Refresh();
            // حفظ ملف Excel المعدل.
            workbook.Save("AutoFilterExample6.xlsx");
            workbook.Save("AutoFilterExample6.pdf");

            // إنشاء كائن Workbook
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // الوصول إلى ورقة العمل الأولى في ملف Excel
            worksheet = workbook.Worksheets[0];

            // مرشح مخصص
            worksheet.AutoFilter.Custom(0, FilterOperatorType.Contains, "Test");

            worksheet.AutoFilter.Refresh();
            // حفظ ملف Excel المعدل.
            workbook.Save("AutoFilterExample7.xlsx");
            workbook.Save("AutoFilterExample7.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


