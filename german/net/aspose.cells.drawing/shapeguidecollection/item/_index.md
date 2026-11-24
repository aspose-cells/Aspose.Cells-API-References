---
title: "ShapeGuideCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeGuideCollection-Eigenschaft. Gibt einen Shape-Guide nach Index zurück"
type: docs
url: /de/net/aspose.cells.drawing/shapeguidecollection/item/
---
## ShapeGuideCollection indexer

Ruft einen Shape Guide nach Index ab

```csharp
public ShapeGuide this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index |  |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeGuideCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Form hinzu, die Anpassungsführungen verwendet
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.RightArrowCallout, 2, 0, 2, 0, 200, 150);

            // Greife über Geometry auf die Sammlung der Anpassungsführungen der Form zu
            ShapeGuideCollection shapeGuides = shape.Geometry.ShapeAdjustValues;

            // Füge neue Führungen zur Sammlung hinzu
            shapeGuides.Add("adj1", 25.5);
            shapeGuides.Add("adj2", 30);
            shapeGuides.Add("adj3", 25.5);
            shapeGuides.Add("adj4", 35);

            // Demonstriere das Auslesen von Führungswerten (Name-Eigenschaft in der bereitgestellten Definition nicht verfügbar)
            Console.WriteLine("First guide value: " + shapeGuides[0].Value);
            Console.WriteLine("Second guide value: " + shapeGuides[1].Value);
            Console.WriteLine("third guide value: " + shapeGuides[2].Value);
            Console.WriteLine("fourth guide value: " + shapeGuides[3].Value);

            // Speichere die geänderte Arbeitsmappe
            workbook.Save("ShapeGuideCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ShapeGuide](../../shapeguide/)
* class [ShapeGuideCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


