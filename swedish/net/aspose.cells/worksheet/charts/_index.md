---
title: "Worksheet.Charts"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Hämtar en Chart-samling"
type: docs
url: /sv/net/aspose.cells/worksheet/charts/
---
## Worksheet.Charts property

Hämtar en [`Chart`](../../../aspose.cells.charts/chart/) samling

```csharp
public ChartCollection Charts { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyChartsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för diagrammet
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);
            
            // Lägg till ett diagram i kalkylbladet
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Få åtkomst till första serien och ange fyllningsmönster
            Series series = chart.NSeries[0];
            series.Area.FillFormat.Pattern = FillPattern.Solid;
            
            // Spara arbetsboken
            workbook.Save("WorksheetPropertyChartsDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [ChartCollection](../../../aspose.cells.charts/chartcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


