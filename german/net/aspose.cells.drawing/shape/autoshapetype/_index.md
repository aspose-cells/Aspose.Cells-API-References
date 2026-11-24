---
title: "Shape.AutoShapeType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt den Auto-Shape-Typ zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing/shape/autoshapetype/
---
## Shape.AutoShapeType property

Liest und legt den AutoShape-Typ fest.

```csharp
public AutoShapeType AutoShapeType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyAutoShapeTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein Shape dem Arbeitsblatt mit korrekten Parametern hinzu.
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 1, 1, 100, 150, 0, 0);

            // Überprüfen und bei Bedarf den AutoShapeType ändern
            if (shape.AutoShapeType == AutoShapeType.Unknown)
            {
                shape.AutoShapeType = AutoShapeType.Rectangle;
            }

            // Ändern Sie den Shape-Typ, um die Eigenschaft zu demonstrieren
            shape.AutoShapeType = AutoShapeType.Oval;

            // Speichere die Arbeitsmappe
            workbook.Save("ShapePropertyAutoShapeTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [AutoShapeType](../../autoshapetype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


