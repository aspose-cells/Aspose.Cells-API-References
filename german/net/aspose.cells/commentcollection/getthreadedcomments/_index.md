---
title: "CommentCollection.GetThreadedComments"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CommentCollection-Methode. Ruft die Threaded‑Kommentare nach Zeilen‑ und Spaltenindex ab"
type: docs
url: /de/net/aspose.cells/commentcollection/getthreadedcomments/
---
## GetThreadedComments(int, int) {#getthreadedcomments}

Liefert die Threaded‑Kommentare nach Zeilen‑ und Spaltenindex.

```csharp
public ThreadedCommentCollection GetThreadedComments(int row, int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Der Zeilenindex. |
| column | Int32 | Der Spaltenindex. |

### Beispiele

```csharp

[C#]
ThreadedCommentCollection threadedComments1 = comments.GetThreadedComments(1, 1);
for (int i = 0; i < threadedComments1.Count; ++i)
{
    ThreadedComment tc = threadedComments1[i];
    string note = tc.Notes;
}
```

### Siehe auch

* class [ThreadedCommentCollection](../../threadedcommentcollection/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetThreadedComments(string) {#getthreadedcomments_1}

Liefert die Threaded‑Kommentare nach Zellnamen.

```csharp
public ThreadedCommentCollection GetThreadedComments(string cellName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | String | Der Name der Zelle. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionMethodGetThreadedCommentsWithStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einen Threaded‑Kommentar‑Autor hinzu und erhalte den Autor per Index
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("John Doe", "JD", "1");
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];

            // Füge einen Threaded‑Kommentar zur Zelle B2 hinzu
            worksheet.Comments.AddThreadedComment("B2", "Initial comment", author);

            // Rufe alle Threaded‑Kommentare für die Zelle B2 ab
            ThreadedCommentCollection threadedComments = worksheet.Comments.GetThreadedComments("B2");

            // Zeige die Threaded‑Kommentare an
            foreach (ThreadedComment comment in threadedComments)
            {
                Console.WriteLine($"Comment by {comment.Author.Name}: {comment.Notes}");
            }
        }
    }
}
```

### Siehe auch

* class [ThreadedCommentCollection](../../threadedcommentcollection/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


