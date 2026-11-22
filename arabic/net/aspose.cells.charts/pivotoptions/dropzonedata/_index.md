---
title: "PivotOptions.DropZoneData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotOptions. تحدد ما إذا كان التحكم لكل حقل PivotTable على محور بيانات PivotTable في PivotTable المصدر يظهر على المخطط عندما تكون الخاصية dropZonesVisible مضبوطة على true"
type: docs
url: /ar/net/aspose.cells.charts/pivotoptions/dropzonedata/
---
## PivotOptions.DropZoneData property

يحدد ما إذا كان عنصر التحكم لكل حقل PivotTable على محور البيانات في PivotTable المصدر يظهر على المخطط عندما تكون الخاصية dropZonesVisible مُعينة إلى true.

```csharp
public bool DropZoneData { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PivotOptionsPropertyDropZoneDataDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // بيانات عينة لجدول pivot
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Books");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Electronics");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Books");
            worksheet.Cells["B4"].PutValue(1500);

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "SalesPivot");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // إنشاء مخطط مرتبط بجدول pivot
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 7, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.PivotSource = "SalesPivot";

            // تكوين خيارات pivot مع تمكين DropZoneData
            PivotOptions pivotOptions = chart.PivotOptions;
            pivotOptions.DropZoneData = true;
            pivotOptions.DropZonesVisible = true;

            // حفظ النتيجة
            workbook.Save("PivotOptionsDropZoneDataDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


