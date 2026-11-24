---
title: "Comment.IsVisible"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Comment-Eigenschaft. Gibt an, ob der Kommentar sichtbar ist oder nicht"
type: docs
url: /de/net/aspose.cells/comment/isvisible/
---
## Comment.IsVisible property

Stellt dar, ob der Kommentar sichtbar ist oder nicht.

```csharp
public bool IsVisible { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyIsVisibleDemo
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

            // Setze den Kommentar auf sichtbar
            comment.IsVisible = true;

            // Prüfe, ob der Kommentar sichtbar ist
            if (comment.IsVisible)
            {
                Console.WriteLine("The comment is visible");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("CommentVisibilityDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


