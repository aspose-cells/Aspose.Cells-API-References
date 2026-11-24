---
title: "LegendEntryCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LegendEntryCollection-Eigenschaft. Gibt das LegendEntry-Element am angegebenen Index zurück"
type: docs
url: /de/net/aspose.cells.charts/legendentrycollection/item/
---
## LegendEntryCollection indexer

Gibt das [`LegendEntry`](../../legendentry/) Element am angegebenen Index zurück.

```csharp
public LegendEntry this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der nullbasierte Index des Elements. |

### Rückgabewert

Das Element am angegebenen Index.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendEntryCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["B1"].PutValue("Category 2");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(40);

            // Ein Diagramm erstellen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("A2:B3", true);
            chart.NSeries.CategoryData = "A1:B1";

            // Zugriff auf Legendeinträge
            LegendEntryCollection legendEntries = chart.Legend.LegendEntries;
            
            // Demonstriere die Verwendung der Item-Eigenschaft
            for (int i = 0; i < legendEntries.Count; i++)
            {
                LegendEntry entry = legendEntries[i];
                Console.WriteLine($"Legend Entry {i}:");
                Console.WriteLine($"- Font: {entry.Font.Name}");
                Console.WriteLine($"- Auto Scale Font: {entry.AutoScaleFont}");
            }

            // Ersten Legendeneintrag ändern
            if (legendEntries.Count > 0)
            {
                legendEntries[0].Font.Name = "Arial";
                legendEntries[0].Font.Size = 12;
                legendEntries[0].AutoScaleFont = false;
            }
        }
    }
}
```

### Siehe auch

* class [LegendEntry](../../legendentry/)
* class [LegendEntryCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


