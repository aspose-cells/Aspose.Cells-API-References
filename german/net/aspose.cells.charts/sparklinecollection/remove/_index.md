---
title: "SparklineCollection.Remove"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SparklineCollection-Methode. Entfernt das Sparkline"
type: docs
url: /de/net/aspose.cells.charts/sparklinecollection/remove/
---
## SparklineCollection.Remove method

Entfernt das Sparkline

```csharp
[Obsolete("Use SparklineCollection.RemoveSparkline(Sparkline) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void Remove(object o)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | Object |  |

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode RemoveSparkline(). Diese Methode wird 6 Monate nach Dezember 2025 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineCollectionMethodRemoveWithObjectDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten in das Arbeitsblatt ein
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);


            // Definieren Sie den CellArea, in dem die Sparklines hinzugefügt werden
            CellArea cellArea = new CellArea { StartColumn = 4, EndColumn = 4, StartRow = 0, EndRow = 0 };

            // Fügen Sie eine neue SparklineGroup zum Arbeitsblatt hinzu
            int sparklineGroupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, cellArea);
            SparklineGroup sparklineGroup = worksheet.SparklineGroups[sparklineGroupIndex];

            SparklineCollection sparklineCollection = sparklineGroup.Sparklines;

            // Fügen Sie Sparklines zur SparklineGroup hinzu
            sparklineCollection.Add("A1:D1", 0, 5);

            Console.WriteLine("Sparkline count: " + sparklineCollection.Count);

            // Legen Sie verschiedene Eigenschaften für die SparklineGroup fest
            sparklineGroup.ShowHighPoint = true;
            sparklineGroup.ShowLowPoint = true;

            // Legen Sie Farben für hohe und niedrige Punkte fest
            CellsColor highPointColor = workbook.CreateCellsColor();
            highPointColor.Color = System.Drawing.Color.Green;
            sparklineGroup.HighPointColor = highPointColor;

            CellsColor lowPointColor = workbook.CreateCellsColor();
            lowPointColor.Color = System.Drawing.Color.Red;
            sparklineGroup.LowPointColor = lowPointColor;

            // Legen Sie die Serienfarbe und die Linienstärke fest
            CellsColor seriesColor = workbook.CreateCellsColor();
            seriesColor.Color = System.Drawing.Color.Orange;
            sparklineGroup.SeriesColor = seriesColor;
            sparklineGroup.LineWeight = 1.0;


            // Erhalte das erste Sparkline zum Entfernen
            Sparkline sparklineToRemove = sparklineCollection[0];

            // Rufe die Remove-Methode mit dem Sparkline-Objekt auf
            sparklineCollection.Remove(sparklineToRemove);

            Console.WriteLine("Sparkline removed successfully");


            Console.WriteLine("after deleted---Sparkline count: " + sparklineCollection.Count);
            // Speichere die Arbeitsmappe
            workbook.Save("SparklineRemoveDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SparklineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


