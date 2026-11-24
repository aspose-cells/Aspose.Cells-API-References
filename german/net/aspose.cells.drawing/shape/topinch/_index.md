---
title: "Shape.TopInch"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt den vertikalen Abstand des Shapes von seiner oberen Zeile in Zoll an"
type: docs
url: /de/net/aspose.cells.drawing/shape/topinch/
---
## Shape.TopInch property

Stellt den vertikalen Versatz der Form von ihrer oberen Zeile dar, in der Einheit Zoll.

```csharp
public double TopInch { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTopInchDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rechteckform hinzufügen
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Setze und demonstriere die TopInch-Eigenschaft
            shape.TopInch = 3;
            Console.WriteLine("Shape Top position (inches): " + shape.TopInch);

            // Modifiziere TopInch, wenn es 3 ist
            if (shape.TopInch == 3)
            {
                shape.TopInch = 1;
                Console.WriteLine("Modified Shape Top position (inches): " + shape.TopInch);
            }

            // Speichere die Arbeitsmappe
            workbook.Save("ShapeTopInchDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


