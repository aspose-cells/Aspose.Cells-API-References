---
title: "Chart.Move"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Chart-Methode. Verschiebt das Diagramm an einen angegebenen Ort"
type: docs
url: /de/net/aspose.cells.charts/chart/move/
---
## Chart.Move method

Verschiebt das Diagramm an einen angegebenen Ort.

```csharp
public void Move(int topRow, int leftColumn, int bottomRow, int rightColumn)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| leftColumn | Int32 | Index der oberen linken Spalte. |
| topRow | Int32 | Index der oberen linken Zeile. |
| rightColumn | Int32 | Index der unteren rechten Spalte |
| bottomRow | Int32 | Index der unteren rechten Zeile |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartMethodMoveWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Ursprüngliche Diagrammposition
                Console.WriteLine($"Original position - topRow: {chart.ChartObject.UpperLeftRow}, leftColumn: {chart.ChartObject.UpperLeftColumn}");

                // Verschieben Sie das Diagramm in die neue Position (Zeilen 10-20, Spalten 2-8)
                chart.Move(10, 2, 20, 8);

                // Neue Position anzeigen
                Console.WriteLine($"New position - topRow: {chart.ChartObject.UpperLeftRow}, leftColumn: {chart.ChartObject.UpperLeftColumn}");

                // Speichere die Arbeitsmappe
                workbook.Save("ChartMoveDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Move method: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


