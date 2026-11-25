---
title: "Classe Fill"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.Fill class. Rappresenta il formato di riempimento della forma"
type: docs
url: /it/net/aspose.cells.drawing/fill/
---
## Fill class

Rappresenta il formato di riempimento della forma.

```csharp
public abstract class Fill
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | / |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Ottiene il codice hash. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class DrawingClassFillDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 150);
            // Imposta il tipo di riempimento su solido e modifica il colore
            rectangle.Fill.FillType = FillType.Solid;
            rectangle.Fill.SolidFill.Color = Color.LightBlue;

            Shape oval = worksheet.Shapes.AddOval(2, 0, 0, 0, 100, 150);
            // Usa il metodo di riempimento gradiente direttamente su FillFormat
            oval.Fill.SetTwoColorGradient(Color.DarkBlue, Color.SkyBlue, GradientStyleType.Vertical, 0);

            workbook.Save("DrawingClassFillDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


