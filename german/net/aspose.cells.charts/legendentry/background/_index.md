---
title: "LegendEntry.Background"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LegendEntry-Eigenschaft. Ruft den Anzeigemodus des Hintergrunds ab und legt ihn fest"
type: docs
url: /de/net/aspose.cells.charts/legendentry/background/
---
## LegendEntry.Background property

Liest und setzt den Anzeigemodus des Hintergrunds

```csharp
[Obsolete("Use LegendEntry.BackgroundMode property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public BackgroundMode Background { get; set; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die LegendEntry.BackgroundMode-Eigenschaft. Diese Eigenschaft wird 12 Monate nach JANUAR 2012 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class LegendEntryPropertyBackgroundDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Den ersten Legendeintrag abrufen
                LegendEntry legendEntry = chart.Legend.LegendEntries[0];

                // Den aktuellen Wert der Background-Eigenschaft anzeigen
                Console.WriteLine("Current Background value: " + legendEntry.Background);

                // Einen neuen Background-Wert festlegen (da er nicht schreibgeschützt ist)
                legendEntry.Background = BackgroundMode.Opaque;
                Console.WriteLine("Background after setting to Opaque: " + legendEntry.Background);

                // Einen weiteren Background-Wert festlegen
                legendEntry.Background = BackgroundMode.Transparent;
                Console.WriteLine("Background after setting to Transparent: " + legendEntry.Background);

                // Speichere die Arbeitsmappe
                workbook.Save("LegendEntryBackgroundDemo.xlsx");
                Console.WriteLine("Background property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* enum [BackgroundMode](../../backgroundmode/)
* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


