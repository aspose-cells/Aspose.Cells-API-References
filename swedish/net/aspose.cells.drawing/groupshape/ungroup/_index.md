---
title: "GroupShape.Ungroup"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GroupShape-metod. Avgrupperar formobjekten"
type: docs
url: /sv/net/aspose.cells.drawing/groupshape/ungroup/
---
## GroupShape.Ungroup method

Avgrupperar formobjekten.

```csharp
public void Ungroup()
```

### Anmärkningar

Om gruppformen är grupperad av en annan gruppform, görs inget.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class GroupShapeMethodUngroupDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till två rektangelformer
            Shape shape1 = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 50);
            Shape shape2 = worksheet.Shapes.AddRectangle(0, 0, 3, 0, 100, 50);

            // Gruppera former till en GroupShape
            GroupShape groupShape = worksheet.Shapes.Group(new Shape[] { shape1, shape2 });

            try
            {
                // Utför Ungroup-metoden
                groupShape.Ungroup();
                Console.WriteLine("Shapes ungrouped successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during ungrouping: {ex.Message}");
            }

            workbook.Save("GroupShapeUngroupDemo.xlsx");
        }
    }
}
```

### Se även

* class [GroupShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


