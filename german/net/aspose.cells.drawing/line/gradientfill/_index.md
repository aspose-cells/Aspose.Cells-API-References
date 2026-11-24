---
title: "Line.GradientFill"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Line-Eigenschaft. Stellt den Farbverlauf dar"
type: docs
url: /de/net/aspose.cells.drawing/line/gradientfill/
---
## Line.GradientFill property

Stellt einen Farbverlauf dar.

```csharp
public GradientFill GradientFill { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;

    public class LinePropertyGradientFillDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten für ein Diagramm hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Ein Säulendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Ermitteln Sie den ersten Punkt der ersten Serie
            Series series = chart.NSeries[0];
            ChartPoint point = series.Points[0];

            try
            {
                // Greifen Sie auf das Line-Objekt (Rand) des Punktes zu
                Line line = point.Border;

                // Lesen Sie die GradientFill-Eigenschaft (schreibgeschützt)
                GradientFill gradient = line.GradientFill;

                // Aktuelle Details zum Farbverlauf anzeigen
                Console.WriteLine("Current GradientFill:");
                Console.WriteLine($"  FillType       = {gradient.FillType}");
                Console.WriteLine($"  DirectionType = {gradient.DirectionType}");
                Console.WriteLine($"  Angle          = {gradient.Angle}");

                // Ändern Sie den Farbverlauf mithilfe der bereitgestellten Methoden
                // Verwenden Sie einen Cast zu einem Standard‑Enum‑Wert, um das Verweisen auf ein nicht vorhandenes Element zu vermeiden
                gradient.SetGradient(GradientFillType.Linear, 45.0, (GradientDirectionType)0);
                Console.WriteLine("GradientFill after SetGradient:");
                Console.WriteLine($"  Angle = {gradient.Angle}");

                // Speichere die Arbeitsmappe
                workbook.Save("LinePropertyGradientFillDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [GradientFill](../../gradientfill/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


