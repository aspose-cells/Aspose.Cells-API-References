---
title: "ChartFrame.TextOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartFrame-Eigenschaft. Liest und schreibt die Optionen des Textes"
type: docs
url: /de/net/aspose.cells.charts/chartframe/textoptions/
---
## ChartFrame.TextOptions property

Ruft die Optionen des Textes ab und legt sie fest.

```csharp
public virtual TextOptions TextOptions { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyTextOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A2"].PutValue("カテゴリー1");
            sheet.Cells["A3"].PutValue("カテゴリー2");
            sheet.Cells["A4"].PutValue("カテゴリー3");
            sheet.Cells["B1"].PutValue("列 1");
            sheet.Cells["B2"].PutValue(4);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(50);
            sheet.Cells["C1"].PutValue("列 2");
            sheet.Cells["C2"].PutValue(50);
            sheet.Cells["C3"].PutValue(100);
            sheet.Cells["C4"].PutValue(150);

            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = sheet.Charts[chartIndex];
            chart.Title.Text = "マーケット";
            chart.Title.TextOptions.LanguageCode = CountryCode.Japan;
            chart.SetChartDataRange("A1:C4", true);

            workbook.Save("ChartTextOptionsOutput.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextOptions](../../../aspose.cells.drawing.texts/textoptions/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


