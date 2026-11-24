---
title: "ChartCollection.RemoveAt"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartCollection-Methode. Entfernt ein Diagramm am bestimmten Index"
type: docs
url: /de/net/aspose.cells.charts/chartcollection/removeat/
---
## ChartCollection.RemoveAt method

Entfernt ein Diagramm am bestimmten Index.

```csharp
public void RemoveAt(int index)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | Int32 | Der Diagramm-Index. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(20);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Anzahl der Anfangsdiagramme anzeigen
            Console.WriteLine("Initial chart count: " + sheet.Charts.Count);

            // Diagramm bei Index 0 entfernen
            sheet.Charts.RemoveAt(0);

            // Diagrammanzahl nach dem Entfernen anzeigen
            Console.WriteLine("Chart count after removal: " + sheet.Charts.Count);
        }
    }
}
```

### Siehe auch

* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


