---
title: "Chart.Calculate"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Chart metod. Beräknar de anpassade positionerna för plotområdet och axlarna om deras positioner är automatiskt tilldelade"
type: docs
url: /sv/net/aspose.cells.charts/chart/calculate/
---
## Calculate() {#calculate}

Beräknar de anpassade positionerna för plotområdet och axlarna om deras positioner tilldelas automatiskt.

```csharp
public void Calculate()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodCalculateDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Beräkna diagrammet innan du sparar
            chart.Calculate();

            // Spara arbetsboken med diagrammet
            workbook.Save("ChartCalculateDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Calculate(ChartCalculateOptions) {#calculate_1}

Beräknar den anpassade positionen för plotområdet och axlarna om deras positioner tilldelas automatiskt, med Diagramberäkningsalternativ.

```csharp
public void Calculate(ChartCalculateOptions calculateOptions)
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodCalculateWithChartCalculateOptionsDemo
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
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(150);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Aktivera datamärkningar
            chart.NSeries[0].DataLabels.ShowValue = true;

            // Skapa beräkningsalternativ och ställ in för att uppdatera alla punkter
            ChartCalculateOptions calculateOptions = new ChartCalculateOptions();
            calculateOptions.UpdateAllPoints = true;

            // Beräkna diagram med alternativ
            chart.Calculate(calculateOptions);

            // Skriv ut dataetiketttexterna
            ChartPointCollection points = chart.NSeries[0].Points;
            Console.WriteLine("DataLabel Text for Point 0: " + points[0].DataLabels.Text);
            Console.WriteLine("DataLabel Text for Point 1: " + points[1].DataLabels.Text);
            Console.WriteLine("DataLabel Text for Point 2: " + points[2].DataLabels.Text);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [ChartCalculateOptions](../../chartcalculateoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


