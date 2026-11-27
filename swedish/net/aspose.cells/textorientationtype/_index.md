---
title: "Enum TextOrientationType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.TextOrientationType enum. Enumererar textorienteringstyper"
type: docs
url: /sv/net/aspose.cells/textorientationtype/
---
## TextOrientationType enumeration

Enumererar typer av textorientering.

```csharp
public enum TextOrientationType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| ClockWise | `0` | Roterar text med 90 grader medurs. |
| CounterClockWise | `1` | Roterar text med 90 grader moturs. |
| NoRotation | `2` | Representerar standardvärdet. |
| TopToBottom | `3` | Visar text från toppen till botten av cellen. Staplad text. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TextOrientationTypeDemo
    {
        public static void TextOrientationTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Hello, Aspose!");
            worksheet.Cells["A2"].PutValue("This is a test comment.");

            // Lägg till en kommentar till cell A1
            int commentIndex = worksheet.Comments.Add(0, 0);
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a comment with text orientation.";

            // Ange olika textorienteringstyper för kommentaren
            comment.TextOrientationType = TextOrientationType.ClockWise;
            Console.WriteLine("Text Orientation: ClockWise");

            // Spara arbetsboken
            workbook.Save("TextOrientationTypeExample_ClockWise.xlsx");

            // Ändra textorientering till CounterClockWise
            comment.TextOrientationType = TextOrientationType.CounterClockWise;
            Console.WriteLine("Text Orientation: CounterClockWise");

            // Spara arbetsboken
            workbook.Save("TextOrientationTypeExample_CounterClockWise.xlsx");

            // Ändra textorientering till NoRotation
            comment.TextOrientationType = TextOrientationType.NoRotation;
            Console.WriteLine("Text Orientation: NoRotation");

            // Spara arbetsboken
            workbook.Save("TextOrientationTypeExample_NoRotation.xlsx");

            // Ändra textorientering till TopToBottom
            comment.TextOrientationType = TextOrientationType.TopToBottom;
            Console.WriteLine("Text Orientation: TopToBottom");

            // Spara arbetsboken
            workbook.Save("TextOrientationTypeExample_TopToBottom.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


