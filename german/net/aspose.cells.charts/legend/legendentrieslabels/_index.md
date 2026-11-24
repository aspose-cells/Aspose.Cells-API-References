---
title: "Legend.LegendEntriesLabels"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Legend-Eigenschaft. Gibt die Beschriftungen der Legendeneinträge zurück, nachdem die Chart.Calculate-Methode aufgerufen wurde."
type: docs
url: /de/net/aspose.cells.charts/legend/legendentrieslabels/
---
## Legend.LegendEntriesLabels property

Gibt die Beschriftungen der Legendeneinträge zurück, nachdem die Methode Chart.Calculate() aufgerufen wurde.

```csharp
[Obsolete("Use Legend.GetLegendLabels method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList LegendEntriesLabels { get; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode Legend.GetLegendLabels. Diese Eigenschaft wird 12 Monate später, seit November 2023, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class LegendPropertyLegendEntriesLabelsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Diagramm berechnen, um sicherzustellen, dass Legendeneinträge erzeugt werden
            chart.Calculate();

            // Legende abrufen
            Legend legend = chart.Legend;

            // Legendeneintragsbeschriftungen anzeigen (unter Verwendung der Eigenschaft)
            Console.WriteLine("Legend Entries Labels:");
            foreach (string label in legend.LegendEntriesLabels)
            {
                Console.WriteLine(label);
            }

            // Speichere die Arbeitsmappe
            workbook.Save("LegendEntriesLabelsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


