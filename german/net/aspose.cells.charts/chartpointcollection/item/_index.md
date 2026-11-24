---
title: "ChartPointCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartPointCollection-Eigenschaft. Gibt das ChartPoint-Element am angegebenen Index in der Serie zurück"
type: docs
url: /de/net/aspose.cells.charts/chartpointcollection/item/
---
## ChartPointCollection indexer

Gibt das [`ChartPoint`](../../chartpoint/) Element am angegebenen Index in der Serie zurück.

```csharp
public ChartPoint this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der Index des Diagrammpunkts in der Serie. |

### Rückgabewert

Das ChartPoint-Objekt.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPointCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Beispieldaten zum Diagramm hinzufügen
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Füge ein Diagramm hinzu
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Greifen Sie mit der Item-Eigenschaft auf einen bestimmten Diagrammpunkt zu
            ChartPoint point = chart.NSeries[0].Points[1];
            
            // Ändern Sie das Füllmuster des Punktes
            point.Area.FillFormat.Pattern = FillPattern.LightHorizontal;

            // Speichere die Arbeitsmappe
            workbook.Save("ChartPointCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartPoint](../../chartpoint/)
* class [ChartPointCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


