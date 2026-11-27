---
title: "DataLabels.ShowLegendKey"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataLabels-egenskap. Representerar ett specificerat diagramdataetikett-legendnyckelns visningsbeteende. Sant om legendnyckeln för dataetiketten är synlig"
type: docs
url: /sv/net/aspose.cells.charts/datalabels/showlegendkey/
---
## DataLabels.ShowLegendKey property

Representerar ett specificerat diagrammets visningsbeteende för datamärkets legendnyckel. Sant om legendnyckeln för datamärket är synlig.

```csharp
public bool ShowLegendKey { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowLegendKeyDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
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
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Hämta dataetiketter
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            
            // Ställ in ShowLegendKey till sant
            dataLabels.ShowLegendKey = true;
            Console.WriteLine("ShowLegendKey set to: " + dataLabels.ShowLegendKey);

            // Spara arbetsboken
            workbook.Save("DataLabelsShowLegendKeyDemo.xlsx");
        }
    }
}
```

### Se även

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


