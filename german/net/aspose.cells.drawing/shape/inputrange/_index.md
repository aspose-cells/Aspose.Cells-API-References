---
title: "Shape.InputRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape Eigenschaft. Liest oder schreibt den Arbeitsblattbereich, der zum Befüllen der angegebenen Kombinationsbox verwendet wird."
type: docs
url: /de/net/aspose.cells.drawing/shape/inputrange/
---
## Shape.InputRange property

Liest oder legt den Arbeitsblattbereich fest, der zum Befüllen der angegebenen Kombinationsbox verwendet wird

```csharp
public string InputRange { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyInputRangeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Value 1");
            worksheet.Cells["A2"].PutValue("Value 2");
            worksheet.Cells["A3"].PutValue("Value 3");
            worksheet.Cells["A4"].PutValue("Value 4");
            worksheet.Cells["A5"].PutValue("Value 5");

            // Eine Form (Rechteck) hinzufügen
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // Eingabebereich für die Form festlegen
            shape.InputRange = "$A$1:$A$5";

            // Eingabebereich bei Bedarf prüfen und ändern
            if (shape.InputRange.Equals("$A$1:$A$5"))
            {
                shape.InputRange = "$B$1:$B$5";
                Console.WriteLine("Input range changed to: " + shape.InputRange);
            }
            else
            {
                Console.WriteLine("Current input range: " + shape.InputRange);
            }
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


