---
title: "SeriesCollection.AddR1C1"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SeriesCollection-metod. Lägger till Series-samlingen i ett diagram"
type: docs
url: /sv/net/aspose.cells.charts/seriescollection/addr1c1/
---
## SeriesCollection.AddR1C1 method

Lägger till [`Series`](../../series/) samlingen i ett diagram.

```csharp
public int AddR1C1(string area, bool isVertical)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| område | String | Anger värden som data-serien ska plottas från |
| ärVertikal | Boolean | Anger om serien ska plottas från ett område med cellvärden radvis eller kolumnvis. |

### Returvärde

Returnerar det första indexet för den tillagda ASeries i NSeries.

### Anmärkningar

Om data anges på sammanhängande celler, använd kolon för att separera dem. Till exempel, R[1]C[1]:R[3]C[2]. Om data anges på sammanhängande celler, använd kommatecken för att separera dem. Till exempel, (R[1]C[1],R[3]C[2]).

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionMethodAddR1C1WithStringBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet wsData = workbook.Worksheets[0];
            wsData.Name = "ChartData";

            // Exempeldata
            wsData.Cells[0, 0].PutValue(1);
            wsData.Cells[1, 0].PutValue(2);
            wsData.Cells[0, 1].PutValue(3);
            wsData.Cells[1, 1].PutValue(4);

            Worksheet wsChart = workbook.Worksheets[workbook.Worksheets.Add(Aspose.Cells.SheetType.Chart)];
            wsChart.Name = "ChartSheet";

            int chartIndex = wsChart.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 0, 0, 15, 15);
            Aspose.Cells.Charts.Chart chart = wsChart.Charts[chartIndex];

            // Användning av AddR1C1 med String- och Boolean-parametrar
            int seriesIndex = chart.NSeries.AddR1C1("ChartData!R1C2:R2C2", true);
            Aspose.Cells.Charts.Series series = chart.NSeries[seriesIndex];
            series.XValues = "ChartData!R1C1:R2C1";

            workbook.Save("SeriesCollectionAddR1C1Demo.xlsx", Aspose.Cells.SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


