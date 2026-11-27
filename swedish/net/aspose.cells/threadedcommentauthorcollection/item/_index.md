---
title: "ThreadedCommentAuthorCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreadedCommentAuthorCollection-egenskap. Hämtar personen som skapar trådade kommentarer"
type: docs
url: /sv/net/aspose.cells/threadedcommentauthorcollection/item/
---
## ThreadedCommentAuthorCollection indexer (1 of 2)

Hämtar personen som skapar trådade kommentarer.

```csharp
public ThreadedCommentAuthor this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Indexet |

### Exempel

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
            
            // Lägg till författare och demonstrera användning av Item-egenskapen
            authors.Add("John Doe", "john.doe@example.com", "JD");
            authors.Add("Jane Smith", "jane.smith@example.com", "JS");
            
            // Få åtkomst till författaren med Item-egenskapen
            ThreadedCommentAuthor firstAuthor = authors[0];
            Console.WriteLine($"First author: {firstAuthor.Name}, {firstAuthor.UserId}");
            
            // Ställ in aktuell person med Item-egenskapen
            authors.CurrentPerson = authors[1];
            Console.WriteLine($"Current person: {authors.CurrentPerson.Name}");

            // Lägg till trådade kommentarer
            CommentCollection comments = workbook.Worksheets[0].Comments;
            comments.AddThreadedComment("A1", "Comment from " + authors[0].Name, authors[0]);
            comments.AddThreadedComment("A1", "Reply from " + authors[1].Name, authors[1]);

            workbook.Save("ThreadedCommentAuthorsDemo.xlsx");
        }
    }
}
```

### Se även

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ThreadedCommentAuthorCollection indexer (2 of 2)

Hämtar personen som skapar trådade kommentarer.

```csharp
public ThreadedCommentAuthor this[string name] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| namn | Namnet på författaren. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentAuthorCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            try
            {
                // Åtkomst till ThreadedCommentAuthorCollection
                ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;

                // Lägg till några författare för att demonstrera Item-egenskapen
                authors.Add("John Doe", "john.doe@example.com", "JD");
                authors.Add("Jane Smith", "jane.smith@example.com", "JS");

                // Få åtkomst till författare med Item-egenskapen (indexerare)
                ThreadedCommentAuthor firstAuthor = authors[0];
                ThreadedCommentAuthor secondAuthor = authors[1];

                // Visa författarinformationen som hämtats via Item-egenskapen
                Console.WriteLine($"First author: {firstAuthor.Name}, {firstAuthor.UserId}");
                Console.WriteLine($"Second author: {secondAuthor.Name}, {secondAuthor.UserId}");

                // Ställ in aktuell person med en av författarna som nås via Item‑egenskapen
                authors.CurrentPerson = authors[0];
                Console.WriteLine($"Current person set to: {authors.CurrentPerson.Name}");

                // Spara arbetsboken
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

### Se även

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


