---
title: "SeriesCollection.AddR1C1"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SeriesCollection-Methode. Fügt die Series-Sammlung zu einem Diagramm hinzu"
type: docs
url: /de/net/aspose.cells.charts/seriescollection/addr1c1/
---
## SeriesCollection.AddR1C1 method

Fügt die [`Series`](../../series/)-Sammlung zu einem Diagramm hinzu.

```csharp
public int AddR1C1(string area, bool isVertical)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Bereich | String | Gibt die Werte an, aus denen die Datenreihe geplottet wird |
| isVertical | Boolean | Gibt an, ob die Reihe aus einem Zellbereich zeilenweise oder spaltenweise geplottet werden soll. |

### Rückgabewert

Gibt den ersten Index der hinzugefügten ASeries in den NSeries zurück.

### Hinweise

Wenn Daten in zusammenhängenden Zellen festgelegt werden, verwenden Sie einen Doppelpunkt, um sie zu trennen. Beispiel: R[1]C[1]:R[3]C[2]. Wenn Daten in zusammenhängenden Zellen festgelegt werden, verwenden Sie ein Komma, um sie zu trennen. Beispiel: (R[1]C[1],R[3]C[2]).

### Beispiele

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

            // Beispieldaten
            wsData.Cells[0, 0].PutValue(1);
            wsData.Cells[1, 0].PutValue(2);
            wsData.Cells[0, 1].PutValue(3);
            wsData.Cells[1, 1].PutValue(4);

            Worksheet wsChart = workbook.Worksheets[workbook.Worksheets.Add(Aspose.Cells.SheetType.Chart)];
            wsChart.Name = "ChartSheet";

            int chartIndex = wsChart.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 0, 0, 15, 15);
            Aspose.Cells.Charts.Chart chart = wsChart.Charts[chartIndex];

            // Verwendung von AddR1C1 mit String- und Boolean-Parametern
            int seriesIndex = chart.NSeries.AddR1C1("ChartData!R1C2:R2C2", true);
            Aspose.Cells.Charts.Series series = chart.NSeries[seriesIndex];
            series.XValues = "ChartData!R1C1:R2C1";

            workbook.Save("SeriesCollectionAddR1C1Demo.xlsx", Aspose.Cells.SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


