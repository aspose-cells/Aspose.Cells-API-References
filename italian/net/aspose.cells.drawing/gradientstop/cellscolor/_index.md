---
title: "GradientStop.CellsColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà GradientStop. Ottiene il colore di questo punto di gradiente"
type: docs
url: /it/net/aspose.cells.drawing/gradientstop/cellscolor/
---
## GradientStop.CellsColor property

Ottiene il colore di questo punto di gradiente.

```csharp
public CellsColor CellsColor { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientStopPropertyCellsColorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Aggiungi una forma con riempimento gradiente
                Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 300);
                shape.Fill.FillType = FillType.Gradient;
                GradientFill gradientFill = shape.Fill.GradientFill;
                gradientFill.SetGradient(GradientFillType.Linear, 0, GradientDirectionType.FromUpperLeftCorner);

                // Crea colore per lo stop gradiente
                CellsColor color = workbook.CreateCellsColor();
                color.Color = Color.Blue;

                // Aggiungi stop gradiente
                gradientFill.GradientStops.Add(0, color, 30);

                // Accedi al punto di gradiente e visualizza le sue proprietà CellsColor
                GradientStop stop = gradientFill.GradientStops[0];
                CellsColor stopColor = stop.CellsColor;

                Console.WriteLine("Gradient Stop CellsColor Properties:");
                Console.WriteLine("Color Type: " + stopColor.Type);
                Console.WriteLine("RGB Color: " + stopColor.Color);
                Console.WriteLine("ARGB Value: " + stopColor.Argb);
                Console.WriteLine("Transparency: " + stopColor.Transparency);

                // Salva la cartella di lavoro
                workbook.Save("GradientStopCellsColorDemo.xlsx");
                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [GradientStop](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


