---
title: "Title.Y"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Title property. Gibt die y-Koordinate der oberen linken Ecke in Einheiten von 1/4000 des Diagrammbereichs zurück oder legt sie fest."
type: docs
url: /de/net/aspose.cells.charts/title/y/
---
## Title.Y property

Gibt die y-Koordinate der oberen linken Ecke in Einheiten von 1/4000 des Diagrammbereichs zurück oder legt sie fest.

```csharp
[Obsolete("Use Title.YRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Y { get; set; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die Title.YRatioToChart-Eigenschaft. Y = YRatioToChart * 4000; Diese Eigenschaft wird 12 Monate später, seit Februar 2025, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erfahren haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TitlePropertyYDemo
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
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Diagrammtitel festlegen
            chart.Title.Text = "Sample Chart";
            chart.Title.Y = 1000; // Demonstrating Y property - position in 1/4000 units
            
            // Diagramm berechnen, um sicherzustellen, dass das Layout aktualisiert wird
            chart.Calculate();

            // Fügen Sie eine Form hinzu, die mit der Y-Position des Titels ausgerichtet ist
            Shape shape = chart.Shapes.AddShapeInChart(MsoDrawingType.Rectangle, PlacementType.Move,
                2000, 
                chart.Title.Y, // Using the title's Y property
                3000, 
                chart.Title.Y + 500);
            shape.Fill.SolidFill.Color = Color.Blue;

            // Speichere die Arbeitsmappe
            workbook.Save("TitlePropertyYDemo_Output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


