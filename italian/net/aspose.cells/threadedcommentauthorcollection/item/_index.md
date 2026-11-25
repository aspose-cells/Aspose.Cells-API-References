---
title: "ThreadedCommentAuthorCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ThreadedCommentAuthorCollection proprietà. Restituisce la persona che crea i commenti in thread"
type: docs
url: /it/net/aspose.cells/threadedcommentauthorcollection/item/
---
## ThreadedCommentAuthorCollection indexer (1 of 2)

Restituisce la persona che crea i commenti in thread.

```csharp
public ThreadedCommentAuthor this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice |

### Esempi

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
            
            // Aggiungi autori e dimostra l'uso della proprietà Item
            authors.Add("John Doe", "john.doe@example.com", "JD");
            authors.Add("Jane Smith", "jane.smith@example.com", "JS");
            
            // Accedi all'autore usando la proprietà Item
            ThreadedCommentAuthor firstAuthor = authors[0];
            Console.WriteLine($"First author: {firstAuthor.Name}, {firstAuthor.UserId}");
            
            // Imposta la persona corrente usando la proprietà Item
            authors.CurrentPerson = authors[1];
            Console.WriteLine($"Current person: {authors.CurrentPerson.Name}");

            // Aggiungi commenti a thread
            CommentCollection comments = workbook.Worksheets[0].Comments;
            comments.AddThreadedComment("A1", "Comment from " + authors[0].Name, authors[0]);
            comments.AddThreadedComment("A1", "Reply from " + authors[1].Name, authors[1]);

            workbook.Save("ThreadedCommentAuthorsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ThreadedCommentAuthorCollection indexer (2 of 2)

Restituisce la persona che crea i commenti in thread.

```csharp
public ThreadedCommentAuthor this[string name] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| name | Il nome dell'autore. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentAuthorCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            try
            {
                // Accedi alla ThreadedCommentAuthorCollection
                ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;

                // Aggiungi alcuni autori per dimostrare la proprietà Item
                authors.Add("John Doe", "john.doe@example.com", "JD");
                authors.Add("Jane Smith", "jane.smith@example.com", "JS");

                // Accedi agli autori usando la proprietà Item (indicizzatore)
                ThreadedCommentAuthor firstAuthor = authors[0];
                ThreadedCommentAuthor secondAuthor = authors[1];

                // Visualizza le informazioni dell'autore recuperate tramite la proprietà Item
                Console.WriteLine($"First author: {firstAuthor.Name}, {firstAuthor.UserId}");
                Console.WriteLine($"Second author: {secondAuthor.Name}, {secondAuthor.UserId}");

                // Imposta la persona corrente usando uno degli autori accessibili tramite la proprietà Item
                authors.CurrentPerson = authors[0];
                Console.WriteLine($"Current person set to: {authors.CurrentPerson.Name}");

                // Salva la cartella di lavoro
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

### Vedi anche

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


