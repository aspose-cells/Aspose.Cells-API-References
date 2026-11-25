---
title: "GroupShape.Ungroup"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "GroupShape method. Sgropa gli elementi della forma"
type: docs
url: /it/net/aspose.cells.drawing/groupshape/ungroup/
---
## GroupShape.Ungroup method

Separa gli elementi della forma.

```csharp
public void Ungroup()
```

### Osservazioni

Se la forma di gruppo è raggruppata da un'altra forma di gruppo, non verrà eseguita alcuna operazione.

### Esempi

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

            // Aggiungi due forme rettangolari
            Shape shape1 = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 50);
            Shape shape2 = worksheet.Shapes.AddRectangle(0, 0, 3, 0, 100, 50);

            // Raggruppa le forme in un GroupShape
            GroupShape groupShape = worksheet.Shapes.Group(new Shape[] { shape1, shape2 });

            try
            {
                // Esegui il metodo Ungroup
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

### Vedi anche

* class [GroupShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


