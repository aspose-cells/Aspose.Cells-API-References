---
title: "Chart.SubTitle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Chart-egenskap. Hämtar diagrammets undertitel. Gäller endast ODS-filer"
type: docs
url: /sv/net/aspose.cells.charts/chart/subtitle/
---
## Chart.SubTitle property

Hämtar diagrammets undertitel. Gäller endast ODS‑filer.

```csharp
public Title SubTitle { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertySubTitleDemo
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

            // Lägg till ett diagram och ange dess dataintervall
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ange huvudrubriken
            chart.Title.Text = "Main Chart Title";

            // Ange undertiteln
            chart.SubTitle.Text = "Chart Subtitle";
            chart.SubTitle.Font.Size = 12;
            chart.SubTitle.Font.IsBold = true;

            // Spara arbetsboken
            workbook.Save("ChartWithSubtitle.xlsx");
        }
    }
}
```

### Se även

* class [Title](../../title/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


