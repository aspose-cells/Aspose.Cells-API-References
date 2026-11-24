---
title: "GroupShape.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GroupShape-Eigenschaft. Ruft die Kindform nach Index ab"
type: docs
url: /de/net/aspose.cells.drawing/groupshape/item/
---
## GroupShape indexer

Liest die untergeordnete Form nach Index.

```csharp
public Shape this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | der Index der Kindform. |

### Rückgabewert

gibt die Kindform zurück.

### Beispiele

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

            // Erstelle zwei Rechteckformen
            Shape shape1 = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 0, 0);
            Shape shape2 = worksheet.Shapes.AddRectangle(50, 50, 100, 100, 0, 0);

            // Gruppiere die Formen
            Shape[] shapesToGroup = new Shape[] { shape1, shape2 };
            GroupShape groupShape = worksheet.Shapes.Group(shapesToGroup);

            // Greife zu und zeige die Eigenschaften der ersten Form an
            Shape firstShape = groupShape[0];
            Console.WriteLine($"First shape initial name: {firstShape.Name}");
            Console.WriteLine($"First shape initial text: {firstShape.Text}");

            // Ändere die Eigenschaften der ersten Form über den Item-Zugriff
            firstShape.Name = "ModifiedRectangle1";
            firstShape.Text = "First Grouped Shape";

            // Greife direkt über den Indexer zu und ändere die zweite Form
            groupShape[1].Text = "Second Grouped Shape";

            // Überprüfe Änderungen
            Console.WriteLine($"\nFirst shape updated name: {groupShape[0].Name}");
            Console.WriteLine($"First shape updated text: {groupShape[0].Text}");
            Console.WriteLine($"Second shape updated text: {groupShape[1].Text}");

            // Modifizierte Arbeitsmappe speichern
            workbook.Save("GroupShapePropertyItemDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Shape](../../shape/)
* class [GroupShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


