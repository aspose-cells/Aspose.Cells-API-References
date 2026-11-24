---
title: "GroupShape.Ungroup"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GroupShape-Methode. Hebt die Gruppierung der Formelemente auf"
type: docs
url: /de/net/aspose.cells.drawing/groupshape/ungroup/
---
## GroupShape.Ungroup method

Löst die Gruppierung der Shape-Elemente auf.

```csharp
public void Ungroup()
```

### Hinweise

Wenn die Gruppenform von einer anderen Gruppenform gruppiert ist,nichts wird getan.

### Beispiele

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

            // Füge zwei Rechteckformen hinzu
            Shape shape1 = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 50);
            Shape shape2 = worksheet.Shapes.AddRectangle(0, 0, 3, 0, 100, 50);

            // Gruppiere Formen zu einem GroupShape
            GroupShape groupShape = worksheet.Shapes.Group(new Shape[] { shape1, shape2 });

            try
            {
                // Führe die Ungroup-Methode aus
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

### Siehe auch

* class [GroupShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


