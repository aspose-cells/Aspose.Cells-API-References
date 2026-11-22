---
title: "SaveOptions.RefreshChartCache"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SaveOptions. تشير إلى ما إذا كان يجب تخزين أحدث بيانات المخطط في الذاكرة"
type: docs
url: /ar/net/aspose.cells/saveoptions/refreshchartcache/
---
## SaveOptions.RefreshChartCache property

يشير إلى ما إذا كان سيتم تخزين أحدث بيانات المخطط مؤقتًا.

```csharp
public bool RefreshChartCache { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyRefreshChartCacheDemo
    {
        public static void Run()
        {
            // إنشاء مصنف تجريبي مع مخطط
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // إنشاء خيارات حفظ PDF مع تمكين RefreshChartCache
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.RefreshChartCache = true;

            // حفظ المصنف مع خيار RefreshChartCache
            workbook.Save("output.pdf", pdfSaveOptions);

            Console.WriteLine("Workbook saved with chart cache refreshed.");
        }
    }
}
```

### انظر أيضًا

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


