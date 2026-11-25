---
title: "Shape.ToFrontOrBack"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Shape. Porta la forma in primo piano o la invia sullo sfondo"
type: docs
url: /it/net/aspose.cells.drawing/shape/tofrontorback/
---
## Shape.ToFrontOrBack method

Porta la forma in primo piano o invia la forma sullo sfondo.

```csharp
public void ToFrontOrBack(int orders)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ordini | Int32 | Se è inferiore a zero, imposta la forma sullo sfondo. Se è superiore a zero, porta la forma in primo piano. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodToFrontOrBackWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi due forme per dimostrare lo z-order
            Aspose.Cells.Drawing.Shape shape1 = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);
            Aspose.Cells.Drawing.Shape shape2 = worksheet.Shapes.AddRectangle(50, 50, 100, 100, 0, 0);

            // Sposta shape2 di 2 posizioni in avanti nello z-order
            shape2.ToFrontOrBack(2);

            // Sposta shape1 di 1 posizione indietro nello z-order
            shape1.ToFrontOrBack(-1);
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


