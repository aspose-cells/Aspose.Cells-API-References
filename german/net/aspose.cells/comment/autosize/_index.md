---
title: "Comment.AutoSize"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Comment-Eigenschaft. Gibt an, ob die Größe des Kommentars automatisch an dessen Inhalt angepasst wird. Hinweis: In einigen speziellen Fällen, wie z. B. einer Mac-Umgebung, kann diese Einstellung keine Wirkung zeigen. Wenn diese Einstellung keine Wirkung zeigt, ersetzen Sie sie bitte durch FitToTextSize."
type: docs
url: /de/net/aspose.cells/comment/autosize/
---
## Comment.AutoSize property

Gibt an, ob die Größe des Kommentars automatisch an seinen Inhalt angepasst wird. Hinweis: In einigen Sonderfällen (z. B. in einer Mac-Umgebung) kann diese Einstellung keine Wirkung zeigen. Wenn diese Einstellung keine Wirkung zeigt, ersetzen Sie sie bitte durch FitToTextSize().

```csharp
public bool AutoSize { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyAutoSizeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einen Kommentar zur Zelle A1 hinzufügen
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a sample comment that will auto-size to fit its content.";

            // Setze AutoSize auf true
            comment.AutoSize = true;

            // Speichere die Arbeitsmappe
            workbook.Save("CommentAutoSizeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


