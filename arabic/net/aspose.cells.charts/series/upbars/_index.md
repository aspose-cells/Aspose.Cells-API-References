---
title: "Series.UpBars"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Series. تُرجع كائن DropBars الذي يمثل أشرطة الصعود في مخطط خطي. ينطبق فقط على المخططات الخطية"
type: docs
url: /ar/net/aspose.cells.charts/series/upbars/
---
## Series.UpBars property

يعيد كائن DropBars الذي يمثل الأشرطة الصاعدة في مخطط الخط. ينطبق فقط على مخططات الخط.

```csharp
public DropBars UpBars { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesPropertyUpBarsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // بيانات عينة لمخطط خطي مع أشرطة الصعود/الهبوط
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // تمكين وتخصيص أشرطة الصعود
            chart.NSeries[0].HasUpDownBars = true;
            DropBars upBars = chart.NSeries[0].UpBars;
            upBars.Area.ForegroundColor = Color.LightGreen;
            upBars.Border.Color = Color.Green;

            workbook.Save("UpBarsExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DropBars](../../dropbars/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


