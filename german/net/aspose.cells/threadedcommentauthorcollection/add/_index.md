---
title: "ThreadedCommentAuthorCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ThreadedCommentAuthorCollection-Methode. Fügt eine Thread-Kommentarperson hinzu"
type: docs
url: /de/net/aspose.cells/threadedcommentauthorcollection/add/
---
## ThreadedCommentAuthorCollection.Add method

Fügt eine Thread‑Kommentar‑Person hinzu.

```csharp
public int Add(string name, string userId, string providerId)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | String | Der Name der Person. |
| userId | String |  |
| providerId | String | Die ID des Anbieters |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentAuthorCollectionMethodAddWithStringStringStringDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einen Threaded-Comment-Autor hinzu
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("Test Author", "testuser", "TA");

            // Abrufen des hinzugefügten Autors
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];

            // Fügen Sie Thread-Kommentare mit dem Autor hinzu
            worksheet.Comments.AddThreadedComment("C2", "First comment", author);
            worksheet.Comments.AddThreadedComment("C2", "Second comment", author);

            // Speichere die Arbeitsmappe
            workbook.Save("ThreadedCommentsExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


