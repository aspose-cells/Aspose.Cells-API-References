---
title: "Comment.Row"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Comment-Eigenschaft. Gibt den Zeilenindex des Kommentars zurück"
type: docs
url: /de/net/aspose.cells/comment/row/
---
## Comment.Row property

Liefert den Zeilenindex des Kommentars.

```csharp
public int Row { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyRowDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einen Kommentar zur Zelle A1 hinzufügen
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment1 = worksheet.Comments[commentIndex];
            comment1.Note = "This is a sample comment";

            // Rufe den Zeilenindex der kommentierten Zelle ab und zeige ihn an
            int row = comment1.Row;
            Console.WriteLine("The comment is in row: " + row);

            // Füge der Zelle B3 einen weiteren Kommentar hinzu
            commentIndex = worksheet.Comments.Add("B3");
            Comment comment2 = worksheet.Comments[commentIndex];
            comment2.Note = "Another comment";

            // Zeige den Zeilenindex des zweiten Kommentars an
            Console.WriteLine("Second comment is in row: " + comment2.Row);
        }
    }
}
```

### Siehe auch

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


