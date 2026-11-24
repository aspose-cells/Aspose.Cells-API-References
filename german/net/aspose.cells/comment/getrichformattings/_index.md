---
title: "Comment.GetRichFormattings"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Comment-Methode. Gibt alle Characters‑Objekte zurück, die einen Zeichenbereich im Kommentartext darstellen"
type: docs
url: /de/net/aspose.cells/comment/getrichformattings/
---
## Comment.GetRichFormattings method

Gibt alle Characters-Objekte zurück, die einen Zeichenbereich im Kommentartext darstellen.

```csharp
public FontSetting[] GetRichFormattings()
```

### Rückgabewert

Alle Characters-Objekte

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentMethodGetRichFormattingsDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einen Kommentar zur Zelle A1 hinzufügen
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.HtmlNote = "<b>Bold</b>, <i>Italic</i>, <u>Underline</u>";

            // Rufe Rich‑Text‑Formatierungen ab
            FontSetting[] formattings = comment.GetRichFormattings();

            // Zeige Formatierungsinformationen an
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

### Siehe auch

* class [FontSetting](../../fontsetting/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


