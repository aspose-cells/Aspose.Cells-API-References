---
title: "Class ChartPointCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.ChartPointCollection class. Representerar en samling som innehåller alla punkter i en serie"
type: docs
url: /sv/net/aspose.cells.charts/chartpointcollection/
---
## ChartPointCollection class

Representerar en samling som innehåller alla punkter i en serie.

```csharp
public class ChartPointCollection : IEnumerable
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Count](../../aspose.cells.charts/chartpointcollection/count/) { get; } | Hämtar antalet diagrampunkter. |
| [Item](../../aspose.cells.charts/chartpointcollection/item/) { get; } | Hämtar [`ChartPoint`](../chartpoint/) elementet på det angivna indexet i serien. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Clear](../../aspose.cells.charts/chartpointcollection/clear/)() | Ta bort alla inställningar för diagrampunkterna. |
| [GetEnumerator](../../aspose.cells.charts/chartpointcollection/getenumerator/)() | Returnerar en enumerator för hela `ChartPointCollection`. |
| [RemoveAt](../../aspose.cells.charts/chartpointcollection/removeat/)(int) | Tar bort punkt vid indexet i serien. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointCollectionDemo
    {
        public static void ChartPointCollectionExample()
        {
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();

            // Hämtning av referensen till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägger till exempelvärden i celler
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Lägger till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.PieExploded, 5, 0, 25, 10);

            // Åtkomst till instansen av det nyligen tillagda diagrammet
            Chart chart = worksheet.Charts[chartIndex];

            // Lägger till NSeries (diagramdatakälla) till diagrammet som sträcker sig från cellen "A1" till "B3"
            chart.NSeries.Add("A1:B3", true);

            // Visa datamärkningar
            chart.NSeries[0].DataLabels.ShowValue = true;

            // Åtkomst till ChartPointCollection
            ChartPointCollection points = chart.NSeries[0].Points;

            // Iterera genom punkterna i samlingen
            for (int i = 0; i < points.Count; i++)
            {
                // Hämta datapunkt
                ChartPoint point = points[i];
                
                // Ställ in pajexplosion
                point.Explosion = 15;
                
                // Ställ in kantfärg
                point.Border.Color = System.Drawing.Color.Red;
            }

            // Sparar Excel-filen
            workbook.Save("ChartPointCollectionExample.xlsx");
            workbook.Save("ChartPointCollectionExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


