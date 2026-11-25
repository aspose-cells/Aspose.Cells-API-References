---
title: "Shape.SetLockedProperty"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Shape. Imposta la proprietà bloccata"
type: docs
url: /it/net/aspose.cells.drawing/shape/setlockedproperty/
---
## Shape.SetLockedProperty method

Imposta la proprietà locked.

```csharp
public void SetLockedProperty(ShapeLockType type, bool value)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | ShapeLockType | Il tipo bloccato. |
| valore | Booleano | Il valore della proprietà. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodSetLockedPropertyWithShapeLockTypeBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma di esempio con tutti i parametri richiesti
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 50);

            // Dimostra l'uso di SetLockedProperty
            shape.SetLockedProperty(ShapeLockType.AdjustHandles, true);
            shape.SetLockedProperty(ShapeLockType.Selection, false);

            Console.WriteLine("Shape locked properties set successfully.");
        }
    }
}
```

### Vedi anche

* enum [ShapeLockType](../../shapelocktype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


