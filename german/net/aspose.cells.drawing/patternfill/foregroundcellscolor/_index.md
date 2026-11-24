---
title: "PatternFill.ForegroundCellsColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PatternFill-Eigenschaft. Gibt das Vordergrund‑CellsColor‑Objekt zurück oder legt es fest"
type: docs
url: /de/net/aspose.cells.drawing/patternfill/foregroundcellscolor/
---
## PatternFill.ForegroundCellsColor property

Gibt das Vordergrund‑[`CellsColor`](../../../aspose.cells/cellscolor/)‑Objekt zurück oder legt es fest.

```csharp
public CellsColor ForegroundCellsColor { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class PatternFillPropertyForegroundCellsColorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie eine Rechteckform hinzu, um die Musterfüllung zu demonstrieren
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);

            try
            {
                // Setzen Sie den Fülltyp auf Muster
                shape.Fill.FillType = FillType.Pattern;

                // Holen Sie die PatternFill-Instanz
                PatternFill patternFill = shape.Fill.PatternFill;

                // Legen Sie den Mustertyp und die Farben fest
                patternFill.Pattern = FillPattern.WideDownwardDiagonal;
                patternFill.ForegroundColor = Color.Red;
                patternFill.BackgroundColor = Color.Yellow;

                // Erstelle ein CellsColor-Objekt für den Vordergrund mithilfe der Color-Eigenschaft
                // Da CellsColor keinen öffentlichen Konstruktor hat, verwenden wir das vorhandene ForegroundCellsColor
                // und ändern seine Eigenschaften direkt
                patternFill.ForegroundCellsColor.Color = Color.Blue;
                patternFill.ForegroundCellsColor.Argb = Color.Blue.ToArgb();

                // Zeige die Eigenschaften von ForegroundCellsColor an
                Console.WriteLine("ForegroundCellsColor Type: " + patternFill.ForegroundCellsColor.Type);
                Console.WriteLine("ForegroundCellsColor Color: " + patternFill.ForegroundCellsColor.Color);
                Console.WriteLine("ForegroundCellsColor ARGB: " + patternFill.ForegroundCellsColor.Argb);

                // Speichere die Arbeitsmappe
                workbook.Save("ForegroundCellsColorDemo.xlsx");
                Console.WriteLine("ForegroundCellsColor demonstration completed successfully.");
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

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


