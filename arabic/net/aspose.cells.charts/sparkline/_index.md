---
title: "الفئة Sparkline"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Charts.Sparkline. تمثل الـ sparkline مخططًا صغيرًا أو رسمًا بيانيًا في خلية ورقة عمل يوفر تمثيلًا بصريًا للبيانات"
type: docs
url: /ar/net/aspose.cells.charts/sparkline/
---
## Sparkline class

تمثل المخططات الصغيرة (sparkline) مخططًا أو رسمًا صغيرًا في خلية ورقة العمل يوفر تمثيلًا بصريًا للبيانات.

```csharp
public class Sparkline
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Column](../../aspose.cells.charts/sparkline/column/) { get; } | يحصل على فهرس العمود للـ sparkline. |
| [DataRange](../../aspose.cells.charts/sparkline/datarange/) { get; set; } | يمثل نطاق البيانات للـ sparkline. |
| [Row](../../aspose.cells.charts/sparkline/row/) { get; } | يحصل على فهرس الصف للـ sparkline. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [ToImage](../../aspose.cells.charts/sparkline/toimage/#toimage)(ImageOrPrintOptions) | يحوّل الـ sparkline إلى صورة. |
| [ToImage](../../aspose.cells.charts/sparkline/toimage/#toimage_1)(Stream, ImageOrPrintOptions) | يحوّل الـ sparkline إلى صورة. |
| [ToImage](../../aspose.cells.charts/sparkline/toimage/#toimage_2)(string, ImageOrPrintOptions) | يحوّل الـ sparkline إلى صورة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SparklineDemo
    {
        public static void SparklineExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بعض البيانات إلى ورقة العمل
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // حدد CellArea للمخطط الخطي.
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // أضف مجموعة مخطط خطي إلى ورقة العمل.
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, sheet.Name + "!A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // إضافة sparkline إلى المجموعة
            idx = group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 5);
            Sparkline line = group.Sparklines[idx];

            // إخراج تفاصيل sparkline
            Console.WriteLine("Sparkline data range: " + line.DataRange + ", row: " + line.Row + ", column: " + line.Column);

            // حفظ الـ sparkline كصورة
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = Aspose.Cells.Drawing.ImageType.Png,
                HorizontalResolution = 300,
                VerticalResolution = 300
            };
            line.ToImage("output.png", options);

            // احفظ المصنف
            workbook.Save("SparklineExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


