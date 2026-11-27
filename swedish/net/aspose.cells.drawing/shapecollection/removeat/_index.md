---
title: "ShapeCollection.RemoveAt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-metod. Ta bort formen"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/removeat/
---
## ShapeCollection.RemoveAt method

Ta bort formen.

```csharp
public void RemoveAt(int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | Indexet för formen. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hämta samlingen av former
            ShapeCollection shapes = worksheet.Shapes;

            // Lägg till den första rektangelformen
            shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            
            // Lägg till den andra rektangelformen
            shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // Ta bort den första formen vid index 0
            shapes.RemoveAt(0);

            // Spara arbetsboken
            workbook.Save("ShapeCollectionRemoveAtDemo.xlsx");
        }
    }
}
```

### Se även

* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


