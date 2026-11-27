---
title: "Comment.GetRichFormattings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Comment-metod. Returnerar alla Characters-objekt som representerar ett teckenintervall inom kommentartexten"
type: docs
url: /sv/net/aspose.cells/comment/getrichformattings/
---
## Comment.GetRichFormattings method

Returnerar alla Characters-objekt som representerar ett intervall av tecken i kommentartexten.

```csharp
public FontSetting[] GetRichFormattings()
```

### Returvärde

Alla Characters‑objekt

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentMethodGetRichFormattingsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en kommentar till cell A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.HtmlNote = "<b>Bold</b>, <i>Italic</i>, <u>Underline</u>";

            // Hämta rik textformatering
            FontSetting[] formattings = comment.GetRichFormattings();

            // Visa formateringsinformation
            Console.WriteLine("Rich Text Formattings:");
            foreach (FontSetting setting in formattings)
            {
                Console.WriteLine($"StartIndex: {setting.StartIndex}, Length: {setting.Length}");
                Console.WriteLine($"Bold: {setting.Font.IsBold}, Italic: {setting.Font.IsItalic}, Underline: {setting.Font.Underline}");
            }
        }
    }
}
```

### Se även

* class [FontSetting](../../fontsetting/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


