---
title: "Enum ShapeTextVerticalAlignmentType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Texts.ShapeTextVerticalAlignmentType-enum. Det motsvarar Format Shape  Text Options  Text Box  Vertical Alignment i Excel"
type: docs
url: /sv/net/aspose.cells.drawing.texts/shapetextverticalalignmenttype/
---
## ShapeTextVerticalAlignmentType enumeration

Det motsvarar "Format Shape - Text Options - Text Box - Vertical Alignment" i Excel.

```csharp
public enum ShapeTextVerticalAlignmentType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Top | `0` |  |
| Middle | `1` |  |
| Bottom | `2` |  |
| TopCentered | `3` |  |
| MiddleCentered | `4` |  |
| BottomCentered | `5` |  |
| Left | `6` |  |
| Center | `7` |  |
| Right | `8` |  |
| LeftMiddle | `9` |  |
| CenterMiddle | `10` |  |
| RightMiddle | `11` |  |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextsClassShapeTextVerticalAlignmentTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Lägg till en textruta i kalkylbladet
                var textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 300);
                textBox.Text = "Sample text for vertical alignment demonstration";

                // Ställ in vertikal textjustering till Mitten
                textBox.TextBoxOptions.ShapeTextVerticalAlignment = ShapeTextVerticalAlignmentType.Middle;

                // Visa den aktuella vertikala justeringen
                Console.WriteLine("Current vertical alignment: " + textBox.TextBoxOptions.ShapeTextVerticalAlignment);

                // Ändra till Övre justering
                textBox.TextBoxOptions.ShapeTextVerticalAlignment = ShapeTextVerticalAlignmentType.Top;
                Console.WriteLine("Changed to: " + textBox.TextBoxOptions.ShapeTextVerticalAlignment);

                // Spara arbetsboken
                workbook.Save("ShapeTextVerticalAlignmentTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ShapeTextVerticalAlignmentType: {ex.Message}");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


