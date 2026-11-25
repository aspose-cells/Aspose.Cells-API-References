---
title: "ThreeDFormat.ContourColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ThreeDFormat. Ottiene e imposta il colore del contorno su una forma"
type: docs
url: /it/net/aspose.cells.drawing/threedformat/contourcolor/
---
## ThreeDFormat.ContourColor property

Ottiene e imposta il colore del contorno su una forma.

```csharp
public CellsColor ContourColor { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyContourColorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma per dimostrare la formattazione 3D
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 200, 100, 0, 0);
            shape.Text = "3D ContourColor Demo";
            
            // Ottieni il ThreeDFormat della forma
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Configura le proprietà 3D di base
            threeDFormat.TopBevelType = BevelType.ArtDeco;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;
            threeDFormat.ContourWidth = 2;

            try
            {
                // Ottieni il valore corrente di ContourColor
                CellsColor contourColor = threeDFormat.ContourColor;
                Console.WriteLine($"Initial ContourColor - Type: {contourColor.Type}, ARGB: {contourColor.Argb}");

                // Crea un nuovo colore modificando quello esistente
                contourColor.Argb = System.Drawing.Color.Red.ToArgb();
                contourColor.Transparency = 0.5;
                threeDFormat.ContourColor = contourColor;

                // Visualizza il nuovo valore di ContourColor
                Console.WriteLine($"New ContourColor - Type: {threeDFormat.ContourColor.Type}, ARGB: {threeDFormat.ContourColor.Argb}");

                // Salva la cartella di lavoro per vedere gli effetti
                workbook.Save("ThreeDFormatContourColorDemo.xlsx");
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


