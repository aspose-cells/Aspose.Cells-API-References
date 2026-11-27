---
title: "ChartFrame.TextFont"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartFrame‑egenskap. Hämtar ett Font‑objekt för det angivna ChartFrame‑objektet"
type: docs
url: /sv/net/aspose.cells.charts/chartframe/textfont/
---
## ChartFrame.TextFont property

Hämtar ett [`Font`](../font/) objekt för det angivna ChartFrame‑objektet.

```csharp
[Obsolete("Use ChartFrame.Font property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual Font TextFont { get; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd i stället ChartFrame.Font‑egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med JANUARY 2012. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyTextFontDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ställ in diagramtitel och konfigurera teckensnitt
            chart.Title.Text = "Sample Chart";
            chart.Title.TextFont.Name = "Arial";
            chart.Title.TextFont.Size = 14;
            chart.Title.TextFont.IsBold = true;
            chart.Title.TextFont.Color = System.Drawing.Color.Blue;

            // Spara arbetsboken
            workbook.Save("ChartTitleFontDemo.xlsx");
        }
    }
}
```

### Se även

* class [Font](../../../aspose.cells/font/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


