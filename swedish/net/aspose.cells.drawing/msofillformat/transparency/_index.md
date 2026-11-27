---
title: "MsoFillFormat.Transparency"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoFillFormat‑egenskap. Returnerar eller anger graden av transparens för den angivna fyllningen som ett värde från 0.0 (opak) till 1.0 (klar)"
type: docs
url: /sv/net/aspose.cells.drawing/msofillformat/transparency/
---
## MsoFillFormat.Transparency property

Returnerar eller anger graden av transparens för den angivna fyllningen som ett värde från 0,0 (opak) till 1,0 (klar).

```csharp
public double Transparency { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFillFormatPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en kommentar till cell A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a test comment";

            // Ange fyllningsformatets egenskaper inklusive transparens
            comment.CommentShape.FillFormat.IsVisible = true;
            comment.CommentShape.FillFormat.ForeColor = System.Drawing.Color.Red;
            comment.CommentShape.FillFormat.BackColor = System.Drawing.Color.Yellow;
            
            // Ange transparens (0.0 = helt opak, 1.0 = helt transparent)
            comment.CommentShape.FillFormat.Transparency = 0.5;

            // Spara arbetsboken
            workbook.Save("CommentTransparencyDemo.xlsx");

            // Läs in den sparade arbetsboken för att verifiera transparensen
            Workbook verifyWorkbook = new Workbook("CommentTransparencyDemo.xlsx");
            Comment verifyComment = verifyWorkbook.Worksheets[0].Comments[0];
            
            // Skriv ut transparensvärdet för att demonstrera att det sparades och lästes in korrekt
            Console.WriteLine("Comment fill transparency: " + 
                verifyComment.CommentShape.FillFormat.Transparency);
        }
    }
}
```

### Se även

* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


