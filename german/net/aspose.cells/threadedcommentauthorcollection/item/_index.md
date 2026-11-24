---
title: "ThreadedCommentAuthorCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ThreadedCommentAuthorCollection-Eigenschaft. Gibt die Person zurück, die Thread-Kommentare erstellt."
type: docs
url: /de/net/aspose.cells/threadedcommentauthorcollection/item/
---
## ThreadedCommentAuthorCollection indexer (1 of 2)

Gibt die Person zurück, die Thread-Kommentare erstellt.

```csharp
public ThreadedCommentAuthor this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der Index |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentAuthorCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
            
            // Fügen Sie Autoren hinzu und demonstrieren Sie die Verwendung der Item-Eigenschaft
            authors.Add("John Doe", "john.doe@example.com", "JD");
            authors.Add("Jane Smith", "jane.smith@example.com", "JS");
            
            // Zugriff auf den Autor über die Item-Eigenschaft
            ThreadedCommentAuthor firstAuthor = authors[0];
            Console.WriteLine($"First author: {firstAuthor.Name}, {firstAuthor.UserId}");
            
            // Setzen Sie die aktuelle Person über die Item-Eigenschaft
            authors.CurrentPerson = authors[1];
            Console.WriteLine($"Current person: {authors.CurrentPerson.Name}");

            // Threaded-Kommentare hinzufügen
            CommentCollection comments = workbook.Worksheets[0].Comments;
            comments.AddThreadedComment("A1", "Comment from " + authors[0].Name, authors[0]);
            comments.AddThreadedComment("A1", "Reply from " + authors[1].Name, authors[1]);

            workbook.Save("ThreadedCommentAuthorsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ThreadedCommentAuthorCollection indexer (2 of 2)

Gibt die Person zurück, die Thread-Kommentare erstellt.

```csharp
public ThreadedCommentAuthor this[string name] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Name | Der Name des Autors. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentAuthorCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            try
            {
                // Zugriff auf die ThreadedCommentAuthorCollection
                ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;

                // Fügen Sie einige Autoren hinzu, um die Item-Eigenschaft zu demonstrieren
                authors.Add("John Doe", "john.doe@example.com", "JD");
                authors.Add("Jane Smith", "jane.smith@example.com", "JS");

                // Zugriff auf Autoren über die Item-Eigenschaft (Indexer)
                ThreadedCommentAuthor firstAuthor = authors[0];
                ThreadedCommentAuthor secondAuthor = authors[1];

                // Anzeige der über die Item-Eigenschaft abgerufenen Autorinformationen
                Console.WriteLine($"First author: {firstAuthor.Name}, {firstAuthor.UserId}");
                Console.WriteLine($"Second author: {secondAuthor.Name}, {secondAuthor.UserId}");

                // Setzen Sie die aktuelle Person mithilfe eines der über die Item-Eigenschaft abgerufenen Autoren
                authors.CurrentPerson = authors[0];
                Console.WriteLine($"Current person set to: {authors.CurrentPerson.Name}");

                // Speichere die Arbeitsmappe
                workbook.Save("ThreadedCommentAuthorsItemDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


