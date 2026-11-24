---
title: "ShapeCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Eigenschaft. Gibt das Shape-Objekt am angegebenen Index in der Liste zurück"
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/item/
---
## ShapeCollection indexer (1 of 2)

Gibt das [`Shape`](../../shape/) Objekt am angegebenen Index in der Liste zurück.

```csharp
public Shape this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der Index. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügt einige Formen zum Arbeitsblatt mit korrekten Parametern hinzu
            worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
            worksheet.Shapes.AddOval(2, 0, 150, 100, 100, 100);
            worksheet.Shapes.AddLine(3, 0, 300, 100, 100, 100);

            // Rufe die Shape-Sammlung ab
            ShapeCollection shapes = worksheet.Shapes;

            // Demonstriere die Item-Eigenschaft, indem du die erste Form abrufst
            Shape firstShape = shapes[0];
            Console.WriteLine("First shape type: " + firstShape.Type);

            // Demonstriere die Item-Eigenschaft, indem du die Form per ID abrufst
            Shape shapeById = shapes[2];
            Console.WriteLine("Shape with ID 2 type: " + shapeById.Type);
        }
    }
}
```

### Siehe auch

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## ShapeCollection indexer (2 of 2)

Liefert das [`Shape`](../../shape/) Objekt anhand des Namens der Form.

```csharp
public Shape this[string name] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Name | Der Name der Form. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Formen zum Arbeitsblatt hinzufügen
            ShapeCollection shapes = worksheet.Shapes;
            shapes.AddRectangle(2, 0, 2, 0, 130, 130);
            shapes.AddOval(5, 0, 2, 0, 130, 130);
            
            // Zugriff auf Formen über die Item-Eigenschaft
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
            
            // Speichere die Arbeitsmappe
            workbook.Save("ShapeCollectionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


