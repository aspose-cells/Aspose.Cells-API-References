---
title: "Enum GradientFillType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.GradientFillType enum. Rappresenta tutti i tipi di riempimento gradiente"
type: docs
url: /it/net/aspose.cells.drawing/gradientfilltype/
---
## GradientFillType enumeration

Rappresenta tutti i tipi di riempimento gradiente.

```csharp
public enum GradientFillType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Linear | `0` | Lineare |
| Radial | `1` | Radiale |
| Rectangle | `2` | Rettangolo |
| Path | `3` | Percorso |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassGradientFillTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una forma per dimostrare il riempimento gradiente
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 5, 5, 20);

            // Ottieni il formato di riempimento
            FillFormat fillFormat = shape.Fill;

            // Imposta il tipo di riempimento gradiente e le proprietà
            fillFormat.SetTwoColorGradient(System.Drawing.Color.Blue, System.Drawing.Color.LightBlue, GradientStyleType.Horizontal, 1);
            fillFormat.GradientFill.SetGradient(GradientFillType.Linear, 45, GradientDirectionType.FromUpperLeftCorner);

            // Restituisci il tipo di direzione del gradiente
            Console.WriteLine("Gradient Direction Type: " + fillFormat.GradientFill.DirectionType);

            // Salva la cartella di lavoro
            workbook.Save("GradientFillTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


