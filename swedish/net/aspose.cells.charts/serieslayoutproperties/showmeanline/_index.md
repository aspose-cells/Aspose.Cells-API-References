---
title: "SeriesLayoutProperties.ShowMeanLine"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SeriesLayoutProperties-egenskap. Anger om linjen som förbinder alla medelvärdespunkter ska visas"
type: docs
url: /sv/net/aspose.cells.charts/serieslayoutproperties/showmeanline/
---
## SeriesLayoutProperties.ShowMeanLine property

Anger om linjen som förbinder alla medelvärdespunkter ska visas.

```csharp
public bool ShowMeanLine { get; set; }
```

### Anmärkningar

Fungerar endast för BoxWhisker-diagram.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertyShowMeanLineDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för låddiagram
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(40);
            worksheet.Cells["A4"].PutValue(25);
            worksheet.Cells["A5"].PutValue(40);
            worksheet.Cells["A6"].PutValue(115);
            worksheet.Cells["A7"].PutValue(65.666);

            // Lägg till ett låddiagram
            int chartIndex = worksheet.Charts.Add(ChartType.BoxWhisker, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Lägg till serier i diagrammet
            chart.NSeries.Add("A1:A7", true);

            // Hämta den första serien
            Series series = chart.NSeries[0];

            // Kom åt layoutegenskaper
            SeriesLayoutProperties layout = series.LayoutProperties;

            // Demonstrera egenskapen ShowMeanLine
            Console.WriteLine("Default ShowMeanLine value: " + layout.ShowMeanLine);
            
            // Ställ in ShowMeanLine till true
            layout.ShowMeanLine = true;
            Console.WriteLine("After setting ShowMeanLine to true: " + layout.ShowMeanLine);

            // Spara arbetsboken
            workbook.Save("BoxWhiskerChart_ShowMeanLineDemo.xlsx");
        }
    }
}
```

### Se även

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


