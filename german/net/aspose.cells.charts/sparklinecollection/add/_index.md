---
title: "SparklineCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SparklineCollection-Methode. Fügt ein Sparkline hinzu"
type: docs
url: /de/net/aspose.cells.charts/sparklinecollection/add/
---
## SparklineCollection.Add method

Fügen Sie ein Sparkline hinzu.

```csharp
public int Add(string dataRange, int row, int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dataRange | String | Gibt den neuen Datenbereich des Sparkline an. |
| row | Int32 | Der Zeilenindex des Speicherorts. |
| column | Int32 | Der Spaltenindex des Speicherorts. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineCollectionMethodAddWithStringInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            for (int i = 0; i < 12; i++)
            {
                worksheet.Cells[4, 3 + i].PutValue(i + 1);
            }

            // Erstelle eine Sparkline-Gruppe
            int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line);
            SparklineGroup group = worksheet.SparklineGroups[groupIndex];

            // Füge ein Sparkline mit Datenbereich und Speicherort hinzu
            int sparklineIndex = group.Sparklines.Add("D5:O5", 4, 15);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [SparklineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


