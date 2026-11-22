---
title: "Title.OverLay"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Title. تمثل عنوانًا مركزيًا فوق المخطط دون تغيير حجم المخطط"
type: docs
url: /ar/net/aspose.cells.charts/title/overlay/
---
## Title.OverLay property

يمثل عنوانًا مركزيًا فوق المخطط دون تغيير حجم المخطط.

```csharp
public bool OverLay { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TitlePropertyOverLayDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            Cells cells = sheet.Cells;
            cells[0, 1].PutValue("Income");
            cells[1, 0].PutValue("Company A");
            cells[2, 0].PutValue("Company B");
            cells[3, 0].PutValue("Company C");
            cells[1, 1].PutValue(10000);
            cells[2, 1].PutValue(20000);
            cells[3, 1].PutValue(30000);

            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 9, 9, 21, 15);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];

            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            chart.Title.Text = "Income Analysis";
            chart.Title.OverLay = true; // Demonstrating OverLay property
            
            workbook.Save("TitleOverlayDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


