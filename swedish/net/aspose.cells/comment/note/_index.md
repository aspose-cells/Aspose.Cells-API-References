---
title: "Comment.Note"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Comment-egenskap. Representerar innehållet i kommentaren"
type: docs
url: /sv/net/aspose.cells/comment/note/
---
## Comment.Note property

Representerar kommentarinnehållet.

```csharp
public string Note { get; set; }
```

### Anmärkningar

Om detta är en trådad kommentar kan noteringen inte ändras, annars kan MS Excel inte behandla den som en trådad kommentar.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyNoteDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en kommentar till cell A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment1 = worksheet.Comments[commentIndex];
            
            // Ställ in noten för kommentaren
            comment1.Note = "First note.";
            
            // Verifiera att noten har satts
            Console.WriteLine("Comment note: " + comment1.Note);
        }
    }
}
```

### Se även

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


