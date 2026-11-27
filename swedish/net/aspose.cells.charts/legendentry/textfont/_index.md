---
title: "LegendEntry.TextFont"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LegendEntry-egenskap. Hämtar ett Font-objekt för det angivna LegendEntry-objektet"
type: docs
url: /sv/net/aspose.cells.charts/legendentry/textfont/
---
## LegendEntry.TextFont property

Hämtar ett [`Font`](../font/) objekt för det angivna LegendEntry-objektet.

```csharp
[Obsolete("Use LegendEntry.Font property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual Font TextFont { get; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället LegendEntry.Font-egenskapen. Denna egenskap kommer att tas bort 12 månader senare sedan JANUARY 2012. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class LegendEntryPropertyTextFontDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["B1"].PutValue("Series 2");
            worksheet.Cells["B2"].PutValue(25);
            worksheet.Cells["B3"].PutValue(35);
            worksheet.Cells["B4"].PutValue(45);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("A2:A4", true);
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A1:B1";

            // Aktivera förklaring
            chart.ShowLegend = true;
            Legend legend = chart.Legend;

            // Åtkomst till första legendposten och ändra dess TextFont-egenskaper
            LegendEntry legendEntry = legend.LegendEntries[0];
            Aspose.Cells.Font font = legendEntry.TextFont;
            
            // Ställ in olika teckensnittsegenskaper
            font.Name = "Arial";
            font.Size = 12;
            font.Color = Color.Red;
            font.IsBold = true;
            font.IsItalic = true;
            font.Underline = FontUnderlineType.Single;

            // Spara arbetsboken
            workbook.Save("LegendEntryTextFontDemo.xlsx");
        }
    }
}
```

### Se även

* class [Font](../../../aspose.cells/font/)
* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


