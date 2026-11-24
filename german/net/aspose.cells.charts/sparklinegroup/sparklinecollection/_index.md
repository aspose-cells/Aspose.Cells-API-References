---
title: "SparklineGroup.SparklineCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SparklineGroup-Eigenschaft. Gibt die Sammlung von Sparkline-Objekten zurück"
type: docs
url: /de/net/aspose.cells.charts/sparklinegroup/sparklinecollection/
---
## SparklineGroup.SparklineCollection property

Gibt die Sammlung von [`Sparkline`](../../sparkline/) Objekt zurück.

```csharp
[Obsolete("Use SparklineGroup.Sparklines property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public SparklineCollection SparklineCollection { get; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft SparklineGroup.Sparklines. Diese Eigenschaft wird 12 Monate später, seit November 2022, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben könnten.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineGroupPropertySparklineCollectionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für Sparklines hinzufügen
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["B1"].PutValue(20);
            worksheet.Cells["C1"].PutValue(15);
            worksheet.Cells["D1"].PutValue(30);

            try
            {
                // Ort für Sparklines festlegen
                CellArea location = new CellArea
                {
                    StartRow = 0,
                    EndRow = 0,
                    StartColumn = 4,
                    EndColumn = 4
                };

                // Fügt der Arbeitsmappe eine Sparkline-Gruppe hinzu
                int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, location);
                SparklineGroup sparklineGroup = worksheet.SparklineGroups[groupIndex];

                // Füge ein Sparkline zur Gruppe hinzu
                sparklineGroup.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);

                // Zugriff auf die SparklineCollection-Eigenschaft (schreibgeschützt)
                SparklineCollection sparklineCollection = sparklineGroup.SparklineCollection;

                // Informationen über die Sparkline-Sammlung anzeigen
                Console.WriteLine($"SparklineCollection contains {sparklineCollection.Count} sparklines");

                // Durch die Sparklines in der Sammlung iterieren
                for (int i = 0; i < sparklineCollection.Count; i++)
                {
                    Sparkline sparkline = sparklineCollection[i];
                    Console.WriteLine($"Sparkline {i + 1} location: Row {sparkline.Row}, Column {sparkline.Column}");
                }

                // Speichere die Arbeitsmappe
                workbook.Save("SparklineCollectionDemo.xlsx");
                Console.WriteLine("SparklineCollection demonstration completed successfully.");
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

* class [SparklineCollection](../../sparklinecollection/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


