---
title: "Shape.GetRichFormattings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape‑metod. Returnerar alla Characters‑objekt som representerar ett teckenintervall inom texten."
type: docs
url: /sv/net/aspose.cells.drawing/shape/getrichformattings/
---
## Shape.GetRichFormattings method

Returnerar alla Characters-objekt som representerar ett teckenintervall inom texten.

```csharp
public FontSetting[] GetRichFormattings()
```

### Returvärde

Alla Characters‑objekt

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetRichFormattingsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en figur med rik text (korrekt parameterantal för AddRectangle)
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);
            shape.Text = "This is bold and this is italic";
            
            // Formatera delar av texten
            shape.Characters(0, 4).Font.IsBold = true;
            shape.Characters(13, 6).Font.IsItalic = true;

            // Hämta rik textformatering
            FontSetting[] formattings = shape.GetRichFormattings();

            // Visa formateringsinformation
            Console.WriteLine("Rich text formattings:");
            foreach (FontSetting setting in formattings)
            {
                Console.WriteLine($"Text segment: '{shape.Text.Substring(setting.StartIndex, setting.Length)}'");
                Console.WriteLine($"Start index: {setting.StartIndex}");
                Console.WriteLine($"Length: {setting.Length}");
                Console.WriteLine($"Bold: {setting.Font.IsBold}");
                Console.WriteLine($"Italic: {setting.Font.IsItalic}");
                Console.WriteLine();
            }
        }
    }
}
```

### Se även

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


