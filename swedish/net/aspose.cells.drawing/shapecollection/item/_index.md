---
title: "ShapeCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-egenskap. Hämtar Shape-objektet på det specifika indexet i listan"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/item/
---
## ShapeCollection indexer (1 of 2)

Hämtar [`Shape`](../../shape/) objektet på det specifika indexet i listan.

```csharp
public Shape this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Indexet. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till några former i kalkylbladet med korrekta parametrar
            worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
            worksheet.Shapes.AddOval(2, 0, 150, 100, 100, 100);
            worksheet.Shapes.AddLine(3, 0, 300, 100, 100, 100);

            // Hämta shape-samlingen
            ShapeCollection shapes = worksheet.Shapes;

            // Demonstrera Item-egenskapen genom att hämta den första formen
            Shape firstShape = shapes[0];
            Console.WriteLine("First shape type: " + firstShape.Type);

            // Demonstrera Item-egenskapen genom att hämta formen med ID
            Shape shapeById = shapes[2];
            Console.WriteLine("Shape with ID 2 type: " + shapeById.Type);
        }
    }
}
```

### Se även

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## ShapeCollection indexer (2 of 2)

Hämtar [`Shape`](../../shape/)-objektet med namnet på formen.

```csharp
public Shape this[string name] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| namn | Namnet på formen. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till former i kalkylbladet
            ShapeCollection shapes = worksheet.Shapes;
            shapes.AddRectangle(2, 0, 2, 0, 130, 130);
            shapes.AddOval(5, 0, 2, 0, 130, 130);
            
            // Åtkomst till former med Item-egenskapen
            Shape rectangle = shapes["Rectangle 1"];
            if (rectangle != null)
            {
                rectangle.FillFormat.ForeColor = System.Drawing.Color.Red;
            }
            
            Shape oval = shapes["Oval 2"];
            if (oval != null)
            {
                oval.FillFormat.ForeColor = System.Drawing.Color.Blue;
            }
            
            // Spara arbetsboken
            workbook.Save("ShapeCollectionDemo.xlsx");
        }
    }
}
```

### Se även

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


