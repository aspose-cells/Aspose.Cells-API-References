---
title: "Shape.HtmlText"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Hämtar och anger HTML-strängen som innehåller data och vissa format i den här textrutan"
type: docs
url: /sv/net/aspose.cells.drawing/shape/htmltext/
---
## Shape.HtmlText property

Hämtar och anger HTML‑strängen som innehåller data och vissa format i den här textrutan.

```csharp
public string HtmlText { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form i kalkylbladet
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // Kontrollera om HtmlText är tom och sätt den om det behövs
            string html = shape.HtmlText;
            if (string.IsNullOrEmpty(html))
            {
                shape.HtmlText = "<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>";
            }

            // Spara arbetsboken
            workbook.Save("ShapeHtmlTextDemo.xlsx");
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


