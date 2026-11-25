---
title: "Enum RectangleAlignmentType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.RectangleAlignmentType enum. Rappresenta come posizionare due rettangoli l'uno rispetto all'altro"
type: docs
url: /it/net/aspose.cells.drawing/rectanglealignmenttype/
---
## RectangleAlignmentType enumeration

Rappresenta come posizionare due rettangoli l'uno rispetto all'altro.

```csharp
public enum RectangleAlignmentType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Bottom | `0` | Inferiore |
| BottomLeft | `1` | BottomLeft |
| BottomRight | `2` | BottomRight |
| Center | `3` | Center |
| Left | `4` | Left |
| Right | `5` | Right |
| Top | `6` | Top |
| TopLeft | `7` | TopLeft |
| TopRight | `8` | TopRight |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassRectangleAlignmentTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Aggiungi una forma rettangolare per dimostrare l'allineamento
                Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 0, 200, 100, 100);

                // Dimostra diversi tipi di allineamento
                Console.WriteLine("Available RectangleAlignmentType values:");
                Console.WriteLine("Bottom: " + RectangleAlignmentType.Bottom);
                Console.WriteLine("BottomLeft: " + RectangleAlignmentType.BottomLeft);
                Console.WriteLine("BottomRight: " + RectangleAlignmentType.BottomRight);
                Console.WriteLine("Center: " + RectangleAlignmentType.Center);
                Console.WriteLine("Left: " + RectangleAlignmentType.Left);
                Console.WriteLine("Right: " + RectangleAlignmentType.Right);
                Console.WriteLine("Top: " + RectangleAlignmentType.Top);
                Console.WriteLine("TopLeft: " + RectangleAlignmentType.TopLeft);
                Console.WriteLine("TopRight: " + RectangleAlignmentType.TopRight);

                // Imposta l'allineamento basandoti su uno dei valori enum
                rectangle.TextHorizontalAlignment = TextAlignmentType.Center;
                rectangle.TextVerticalAlignment = TextAlignmentType.Center;

                // Salva la cartella di lavoro
                workbook.Save("RectangleAlignmentTypeDemo.xlsx");
                Console.WriteLine("RectangleAlignmentType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating RectangleAlignmentType: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


