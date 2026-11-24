---
title: "Shape.Spt"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt eine optionale Nummer an, die eine Anwendung verwenden kann, um die bestimmte Form einem definierten Formtyp zuzuordnen."
type: docs
url: /de/net/aspose.cells.drawing/shape/spt/
---
## Shape.Spt property

Gibt eine optionale Nummer an, die eine Anwendung verwenden kann, um die jeweilige Form einem definierten Formtyp zuzuordnen.

```csharp
public int Spt { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertySptDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Rechteck shape mit korrekten Parametern hinzu
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 1, 1, 100, 100, 100, 100);

            // Rufen Sie die Spt-Eigenschaft ab und zeigen Sie sie an.
            int spt = shape.Spt;
            Console.WriteLine("Shape Spt value: " + spt);

            // Erstellen Sie eine neue ovale Form, um verschiedene Spt-Werte zu demonstrieren.
            Shape ovalShape = worksheet.Shapes.AddShape(MsoDrawingType.Oval, 1, 1, 100, 100, 100, 100);
            Console.WriteLine("Oval shape Spt value: " + ovalShape.Spt);
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


