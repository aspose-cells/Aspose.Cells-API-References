---
title: "MsoFillFormat.Transparency"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MsoFillFormat-Eigenschaft. Gibt den Transparenzgrad der angegebenen Füllung zurück oder setzt ihn als Wert von 0,0 (undurchsichtig) bis 1,0 (klar)"
type: docs
url: /de/net/aspose.cells.drawing/msofillformat/transparency/
---
## MsoFillFormat.Transparency property

Gibt den Transparenzgrad der angegebenen Füllung zurück oder setzt ihn, als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent).

```csharp
public double Transparency { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einen Kommentar zur Zelle A1 hinzufügen
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a test comment";

            // Setzen Sie Füllformat-Eigenschaften einschließlich Transparenz
            comment.CommentShape.FillFormat.IsVisible = true;
            comment.CommentShape.FillFormat.ForeColor = System.Drawing.Color.Red;
            comment.CommentShape.FillFormat.BackColor = System.Drawing.Color.Yellow;
            
            // Setzen Sie die Transparenz (0,0 = vollständig undurchsichtig, 1,0 = vollständig transparent)
            comment.CommentShape.FillFormat.Transparency = 0.5;

            // Speichere die Arbeitsmappe
            workbook.Save("CommentTransparencyDemo.xlsx");

            // Laden Sie die gespeicherte Arbeitsmappe, um die Transparenz zu überprüfen
            Workbook verifyWorkbook = new Workbook("CommentTransparencyDemo.xlsx");
            Comment verifyComment = verifyWorkbook.Worksheets[0].Comments[0];
            
            // Geben Sie den Transparenzwert aus, um zu demonstrieren, dass er korrekt gespeichert und geladen wurde
            Console.WriteLine("Comment fill transparency: " + 
                verifyComment.CommentShape.FillFormat.Transparency);
        }
    }
}
```

### Siehe auch

* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


