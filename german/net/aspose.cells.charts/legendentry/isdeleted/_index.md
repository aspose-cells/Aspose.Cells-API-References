---
title: "LegendEntry.IsDeleted"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LegendEntry-Eigenschaft. Gibt an, ob der Legendeintrag gelöscht ist, und legt dies fest"
type: docs
url: /de/net/aspose.cells.charts/legendentry/isdeleted/
---
## LegendEntry.IsDeleted property

Liest und setzt, ob der Legendeneintrag gelöscht ist.

```csharp
public bool IsDeleted { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendEntryPropertyIsDeletedDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Den ersten Legendeintrag abrufen
            LegendEntry legendEntry = chart.Legend.LegendEntries[0];

            // IsDeleted-Eigenschaft demonstrieren
            Console.WriteLine("Legend entry initially deleted? " + legendEntry.IsDeleted);
            
            // Den Legendeintrag löschen
            legendEntry.IsDeleted = true;
            Console.WriteLine("Legend entry after deletion? " + legendEntry.IsDeleted);

            // Den Legendeintrag wiederherstellen
            legendEntry.IsDeleted = false;
            Console.WriteLine("Legend entry after restoration? " + legendEntry.IsDeleted);

            // Speichere die Arbeitsmappe
            workbook.Save("LegendEntryIsDeletedDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


