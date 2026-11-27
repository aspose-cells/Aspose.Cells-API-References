---
title: "TextBoxOptions.ShapeTextDirection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextBoxOptions egenskap. Hämtar eller anger textens visningsriktning inom ett givet textområde. Det motsvarar Format Shape  Text Options  Text Box  Text direction i Excel"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textboxoptions/shapetextdirection/
---
## TextBoxOptions.ShapeTextDirection property

Hämtar eller anger textriktningen inom ett givet textområde. Det motsvarar "Format Shape - Text Options - Text Box - Text direction" i Excel

```csharp
public TextVerticalType ShapeTextDirection { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyShapeTextDirectionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en textruta
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);

            // Ställ in textriktning till vertikal
            shape.TextBoxOptions.ShapeTextDirection = TextVerticalType.Vertical;

            // Ange lite text för att demonstrera riktningen
            shape.Text = "Vertical Text Example";

            // Spara arbetsboken
            workbook.Save("TextBoxTextDirectionDemo.xlsx");
        }
    }
}
```

### Se även

* enum [TextVerticalType](../../textverticaltype/)
* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


