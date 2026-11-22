---
title: "PivotOptions.DropZoneFilter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotOptions. تحدد ما إذا كان التحكم لكل حقل PivotTable على محور صفحة PivotTable في PivotTable المصدر يظهر على المخطط عندما تكون الخاصية dropZonesVisible مضبوطة على true"
type: docs
url: /ar/net/aspose.cells.charts/pivotoptions/dropzonefilter/
---
## PivotOptions.DropZoneFilter property

يحدد ما إذا كان عنصر التحكم لكل حقل PivotTable على محور الصفحات في PivotTable المصدر يظهر على المخطط عندما تكون الخاصية dropZonesVisible مُعينة إلى true.

```csharp
public bool DropZoneFilter { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PivotOptionsPropertyDropZoneFilterDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // بيانات عينة
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

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("=A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // إنشاء مخطط مرتبط بpivot
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 7, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.PivotSource = "PivotTable1";

            // تكوين خيارات pivot باستخدام DropZoneFilter
            PivotOptions pivotOptions = chart.PivotOptions;
            pivotOptions.DropZoneFilter = true;
            pivotOptions.DropZonesVisible = true;

            workbook.Save("PivotOptionsDropZoneFilterDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


