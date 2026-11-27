---
title: "ChartArea.Height"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartArea-egenskap. Hämtar eller anger det vertikala offsetet från dess nedre högra hörnrad i enheter av 1/4000 av diagramområdet"
type: docs
url: /sv/net/aspose.cells.charts/chartarea/height/
---
## ChartArea.Height property

Hämtar eller anger det vertikala offsetet från dess nedre‑högra hörnrad, i enheter av 1/4000 av diagramområdet.

```csharp
[Obsolete("Use ChartArea.HeightRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Height { get; set; }
```

### Anmärkningar

OBS: Den här medlemmen är nu föråldrad. Använd istället ChartArea.HeightRatioToChart‑egenskap. Height = HeightRatioToChart * 4000. Denna egenskap kommer att tas bort 12 månader senare, från och med februari 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartAreaPropertyHeightDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Åtkomst till diagramområdet
            ChartArea chartArea = chart.ChartArea;

            // Demonstrera Height-egenskapen
            Console.WriteLine("Original Chart Area Height: " + chartArea.Height);
            
            // Ändra höjden
            chartArea.Height = 500;
            Console.WriteLine("Modified Chart Area Height: " + chartArea.Height);

            // Spara arbetsboken
            workbook.Save("ChartAreaHeightDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


