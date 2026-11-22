---
title: "SparklineGroup.ShowMarkers"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SparklineGroup. تشير إلى ما إذا كان يُبرز كل نقطة في كل خط سباركلين داخل مجموعة السباركلين"
type: docs
url: /ar/net/aspose.cells.charts/sparklinegroup/showmarkers/
---
## SparklineGroup.ShowMarkers property

يشير إلى ما إذا كان يجب تمييز كل نقطة في كل مخطط خطي في مجموعة المخططات الخطية.

```csharp
public bool ShowMarkers { get; set; }
```

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyShowMarkersDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // تحديد موقع السباركلين
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // أضف مجموعة سباركلين
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // إضافة سباركلين
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // تكوين مظهر السباركلين
            CellsColor seriesColor = workbook.CreateCellsColor();
            seriesColor.Color = Color.Orange;
            group.SeriesColor = seriesColor;

            group.ShowMarkers = true;
            
            CellsColor markersColor = workbook.CreateCellsColor();
            markersColor.Color = Color.Black;
            group.MarkersColor = markersColor;

            // احفظ المصنف
            workbook.Save("SparklineWithMarkers.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


