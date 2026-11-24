---
title: "MsoFillFormat.ForeColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MsoFillFormat-Eigenschaft. Gibt die Vordergrundfarbe der Füllung zurück und setzt sie"
type: docs
url: /de/net/aspose.cells.drawing/msofillformat/forecolor/
---
## MsoFillFormat.ForeColor property

Liest und setzt die Vordergrundfarbe der Füllung.

```csharp
public Color ForeColor { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFillFormatPropertyForeColorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Rechteckform mit allen erforderlichen Parametern hinzu
            var rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 150, 200);

            // Hole das Füllformat
            MsoFillFormat fillFormat = rectangle.FillFormat;

            // Setzen und demonstrieren Sie die ForeColor-Eigenschaft
            fillFormat.ForeColor = System.Drawing.Color.Red;
            Console.WriteLine("ForeColor set to: " + fillFormat.ForeColor);

            // Ändern Sie die ForeColor
            fillFormat.ForeColor = System.Drawing.Color.FromArgb(0, 128, 255);
            Console.WriteLine("ForeColor changed to: " + fillFormat.ForeColor);

            // Speichere die Arbeitsmappe
            workbook.Save("MsoFillFormatForeColorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


