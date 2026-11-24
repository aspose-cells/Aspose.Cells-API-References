---
title: "Comment.Note"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Comment-Eigenschaft. Gibt den Inhalt des Kommentars an"
type: docs
url: /de/net/aspose.cells/comment/note/
---
## Comment.Note property

Stellt den Inhalt des Kommentars dar.

```csharp
public string Note { get; set; }
```

### Hinweise

Wenn dies ein Threaded‑Kommentar ist, kann die Notiz nicht geändert werden, sonst könnte MS Excel ihn nicht als Threaded‑Kommentar verarbeiten.

### Beispiele

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

            // Einen Kommentar zur Zelle A1 hinzufügen
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment1 = worksheet.Comments[commentIndex];
            
            // Setzen Sie die Notiz für den Kommentar
            comment1.Note = "First note.";
            
            // Überprüfen Sie, ob die Notiz gesetzt wurde
            Console.WriteLine("Comment note: " + comment1.Note);
        }
    }
}
```

### Siehe auch

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


