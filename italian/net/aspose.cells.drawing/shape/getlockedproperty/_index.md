---
title: "Shape.GetLockedProperty"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Shape. Ottiene il valore della proprietà bloccata"
type: docs
url: /it/net/aspose.cells.drawing/shape/getlockedproperty/
---
## Shape.GetLockedProperty method

Ottiene il valore della proprietà locked.

```csharp
public bool GetLockedProperty(ShapeLockType type)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | ShapeLockType | Il tipo della proprietà bloccata della forma. |

### Valore di ritorno

Restituisce il valore della proprietà bloccata.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetLockedPropertyWithShapeLockTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma al foglio di lavoro
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // Imposta la proprietà bloccata per AdjustHandles
            shape.SetLockedProperty(ShapeLockType.AdjustHandles, true);

            // Verifica se AdjustHandles è bloccato
            int noAdjustHandles = 0;
            if (shape.GetLockedProperty(ShapeLockType.AdjustHandles))
                noAdjustHandles = 1;

            Console.WriteLine("AdjustHandles locked status: " + (noAdjustHandles == 1));
        }
    }
}
```

### Vedi anche

* enum [ShapeLockType](../../shapelocktype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


