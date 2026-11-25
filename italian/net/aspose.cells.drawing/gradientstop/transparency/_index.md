---
title: "GradientStop.Transparency"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà GradientStop. Restituisce o imposta il grado di trasparenza dell'area come valore da 0,0 opaco a 1,0 trasparente"
type: docs
url: /it/net/aspose.cells.drawing/gradientstop/transparency/
---
## GradientStop.Transparency property

Restituisce o imposta il grado di trasparenza dell'area come valore da 0,0 (opaco) a 1,0 (trasparente).

```csharp
public double Transparency { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientStopPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma con riempimento gradiente
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 300);
            shape.Fill.FillType = FillType.Gradient;
            GradientFill gradientFill = shape.Fill.GradientFill;
            gradientFill.SetGradient(GradientFillType.Linear, 0, GradientDirectionType.FromUpperLeftCorner);

            // Crea colore per lo stop gradiente
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Blue;

            // Aggiungi un punto di gradiente con trasparenza iniziale
            gradientFill.GradientStops.Add(0, color, 30);

            // Accedi allo stop gradiente
            GradientStop stop = gradientFill.GradientStops[0];

            // Visualizza e modifica la trasparenza
            Console.WriteLine("Initial Transparency: " + stop.Transparency);
            stop.Transparency = 0.7;
            Console.WriteLine("Modified Transparency: " + stop.Transparency);

            // Aggiungi un altro punto per confronto visivo
            CellsColor color2 = workbook.CreateCellsColor();
            color2.Color = Color.Green;
            gradientFill.GradientStops.Add(1, color2, 30);

            // Salva la cartella di lavoro
            workbook.Save("GradientStopTransparencyDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [GradientStop](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


