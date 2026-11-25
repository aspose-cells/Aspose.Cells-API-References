---
title: "ThreeDFormat.ExtrusionColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ThreeDFormat. Ottiene il colore di estrusione su una forma"
type: docs
url: /it/net/aspose.cells.drawing/threedformat/extrusioncolor/
---
## ThreeDFormat.ExtrusionColor property

Ottiene il colore di estrusione su una forma.

```csharp
public CellsColor ExtrusionColor { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyExtrusionColorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma per dimostrare la formattazione 3D
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 0, 0, 200, 100);
            shape.Text = "3D ExtrusionColor Demo";
            
            // Ottieni il ThreeDFormat della forma
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Configura le proprietà 3D di base per rendere visibile l'estrusione
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.Material = PresetMaterialType.Plastic;

            try
            {
                // Ottieni e visualizza il valore di ExtrusionColor
                CellsColor extrusionColor = threeDFormat.ExtrusionColor;
                Console.WriteLine("ExtrusionColor properties:");
                Console.WriteLine($"Type: {extrusionColor.Type}");
                Console.WriteLine($"Color (RGB): {extrusionColor.Color}");
                Console.WriteLine($"Transparency: {extrusionColor.Transparency}");

                // Salva la cartella di lavoro per vedere gli effetti 3D
                workbook.Save("ThreeDFormatExtrusionColorDemo.xlsx");
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
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


