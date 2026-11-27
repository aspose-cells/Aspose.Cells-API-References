---
title: "GroupShape.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GroupShape-egenskap. Hämtar underformen efter index"
type: docs
url: /sv/net/aspose.cells.drawing/groupshape/item/
---
## GroupShape indexer

Hämtar underformen efter index.

```csharp
public Shape this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | index för underformen. |

### Returvärde

returnerar underformen.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class GroupShapePropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa två rektangelformer
            Shape shape1 = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 0, 0);
            Shape shape2 = worksheet.Shapes.AddRectangle(50, 50, 100, 100, 0, 0);

            // Gruppera formerna
            Shape[] shapesToGroup = new Shape[] { shape1, shape2 };
            GroupShape groupShape = worksheet.Shapes.Group(shapesToGroup);

            // Åtkomst och visa den första formens egenskaper
            Shape firstShape = groupShape[0];
            Console.WriteLine($"First shape initial name: {firstShape.Name}");
            Console.WriteLine($"First shape initial text: {firstShape.Text}");

            // Ändra den första formens egenskaper via Item-åtkomst
            firstShape.Name = "ModifiedRectangle1";
            firstShape.Text = "First Grouped Shape";

            // Åtkomst och ändra den andra formen direkt via indexerare
            groupShape[1].Text = "Second Grouped Shape";

            // Verifiera ändringar
            Console.WriteLine($"\nFirst shape updated name: {groupShape[0].Name}");
            Console.WriteLine($"First shape updated text: {groupShape[0].Text}");
            Console.WriteLine($"Second shape updated text: {groupShape[1].Text}");

            // Spara modifierad arbetsbok
            workbook.Save("GroupShapePropertyItemDemo.xlsx");
        }
    }
}
```

### Se även

* class [Shape](../../shape/)
* class [GroupShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


