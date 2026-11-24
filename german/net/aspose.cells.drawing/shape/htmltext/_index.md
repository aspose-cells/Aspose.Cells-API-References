---
title: "Shape.HtmlText"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Ruft die HTML-Zeichenkette ab und setzt sie, die Daten und einige Formate in diesem Textfeld enthält."
type: docs
url: /de/net/aspose.cells.drawing/shape/htmltext/
---
## Shape.HtmlText property

Liest und legt die HTML-Zeichenkette fest, die Daten und einige Formate in diesem Textfeld enthält

```csharp
public string HtmlText { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHtmlTextDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt eine Form hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // Überprüfen Sie, ob HtmlText leer ist, und setzen Sie ihn bei Bedarf.
            string html = shape.HtmlText;
            if (string.IsNullOrEmpty(html))
            {
                shape.HtmlText = "<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>";
            }

            // Speichere die Arbeitsmappe
            workbook.Save("ShapeHtmlTextDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


