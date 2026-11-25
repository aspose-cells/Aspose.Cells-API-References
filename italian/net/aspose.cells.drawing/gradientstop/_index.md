---
title: "Classe GradientStop"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.GradientStop class. Rappresenta il punto di gradiente"
type: docs
url: /it/net/aspose.cells.drawing/gradientstop/
---
## GradientStop class

Rappresenta il punto di arresto del gradiente.

```csharp
public class GradientStop
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CellsColor](../../aspose.cells.drawing/gradientstop/cellscolor/) { get; } | Ottiene il colore di questo punto di gradiente. |
| [Position](../../aspose.cells.drawing/gradientstop/position/) { get; set; } | La posizione dello stop. |
| [Transparency](../../aspose.cells.drawing/gradientstop/transparency/) { get; set; } | Restituisce o imposta il grado di trasparenza dell'area come valore da 0,0 (opaco) a 1,0 (trasparente). |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class DrawingClassGradientStopDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook per la dimostrazione
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

                // Accedi allo stop gradiente
                GradientStop stop = gradientFill.GradientStops[0];

                // Dimostra la funzionalità di base
                Console.WriteLine("GradientStop instance created successfully");
                Console.WriteLine("Position: " + stop.Position);
                Console.WriteLine("Transparency: " + stop.Transparency);
                Console.WriteLine("CellsColor Type: " + stop.CellsColor.Type);

                // Modifica proprietà
                stop.Position = 0.5;
                stop.Transparency = 0.7;

                Console.WriteLine("Modified Position: " + stop.Position);
                Console.WriteLine("Modified Transparency: " + stop.Transparency);

                // Salva la cartella di lavoro
                workbook.Save("GradientStopDemo.xlsx");
                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with GradientStop: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


