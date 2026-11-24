---
title: "FillFormat.FillType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FillFormat-Eigenschaft. Gibt den Fülltyp zurück und legt ihn fest."
type: docs
url: /de/net/aspose.cells.drawing/fillformat/filltype/
---
## FillFormat.FillType property

Liest und setzt den Fülltyp

```csharp
public FillType FillType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyFillTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rechteckform hinzufügen
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // Setzen Sie eine einfarbige Füllung mit Farbe.
            shape.Fill.FillType = FillType.Solid;
            shape.Fill.SolidFill.Color = System.Drawing.Color.Red;

            // Geben Sie den Fülltyp aus.
            Console.WriteLine("Shape fill type: " + shape.Fill.FillType);

            // Wechseln Sie zu einer Farbverlauffüllung.
            shape.Fill.FillType = FillType.Gradient;
            Console.WriteLine("Shape fill type changed to: " + shape.Fill.FillType);

            // Speichere die Arbeitsmappe
            workbook.Save("FillTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [FillType](../../filltype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


