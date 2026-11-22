---
title: "الفئة PivotOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Charts.PivotOptions. تمثل نوعًا مركبًا يحدد عناصر التحكم المحورية التي تظهر على المخطط"
type: docs
url: /ar/net/aspose.cells.charts/pivotoptions/
---
## PivotOptions class

يمثل نوعًا مركبًا يحدد عناصر التحكم المحورية التي تظهر على المخطط

```csharp
public class PivotOptions
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [DropZoneCategories](../../aspose.cells.charts/pivotoptions/dropzonecategories/) { get; set; } | يحدد ما إذا كان عنصر التحكم لكل حقل PivotTable على محور الصفوف في PivotTable المصدر يظهر على المخطط عندما تكون الخاصية dropZonesVisible مُعينة إلى true. |
| [DropZoneData](../../aspose.cells.charts/pivotoptions/dropzonedata/) { get; set; } | يحدد ما إذا كان عنصر التحكم لكل حقل PivotTable على محور البيانات في PivotTable المصدر يظهر على المخطط عندما تكون الخاصية dropZonesVisible مُعينة إلى true. |
| [DropZoneFilter](../../aspose.cells.charts/pivotoptions/dropzonefilter/) { get; set; } | يحدد ما إذا كان عنصر التحكم لكل حقل PivotTable على محور الصفحات في PivotTable المصدر يظهر على المخطط عندما تكون الخاصية dropZonesVisible مُعينة إلى true. |
| [DropZoneSeries](../../aspose.cells.charts/pivotoptions/dropzoneseries/) { get; set; } | يحدد ما إذا كان عنصر التحكم لكل حقل PivotTable على محور الأعمدة في PivotTable المصدر يظهر على المخطط عندما تكون الخاصية dropZonesVisible مُعينة إلى true. |
| [DropZonesVisible](../../aspose.cells.charts/pivotoptions/dropzonesvisible/) { get; set; } | يحدد ما إذا كان يمكن لأي عناصر تحكم محورية الظهور على المخطط المحوري. |
| [ShowExpandCollapseFieldButtons](../../aspose.cells.charts/pivotoptions/showexpandcollapsefieldbuttons/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كان يجب إظهار أزرار توسيع أو طي الحقول |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotOptionsDemo
    {
        public static void PivotOptionsExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات لجدول المحور
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B5"].PutValue(40);

            // إضافة جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("=A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 7, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.PivotSource = "PivotTable1";

            // الوصول إلى PivotOptions للمخطط
            PivotOptions pivotOptions = chart.PivotOptions;

            // تعيين خصائص PivotOptions
            pivotOptions.DropZoneFilter = true;
            pivotOptions.DropZoneCategories = true;
            pivotOptions.DropZoneData = true;
            pivotOptions.DropZoneSeries = true;
            pivotOptions.DropZonesVisible = true;

            // احفظ المصنف
            workbook.Save("PivotOptionsExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


