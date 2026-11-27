---
title: "ThreadedCommentAuthorCollection.IndexOf"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreadedCommentAuthorCollection‑metod. Hämtar index för ThreadedCommentAuthor‑objektet"
type: docs
url: /sv/net/aspose.cells/threadedcommentauthorcollection/indexof/
---
## ThreadedCommentAuthorCollection.IndexOf method

Hämtar index för ThreadedCommentAuthor‑objektet

```csharp
public int IndexOf(ThreadedCommentAuthor author)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| författare | ThreadedCommentAuthor | ThreadedCommentAuthor‑objektet |

### Returvärde

Indexet i ThreadedCommentAuthor‑samlingen

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentAuthorCollectionMethodIndexOfWithThreadedCommentAuthorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Hämta samlingen av trådade kommentarförfattare
            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;

            // Lägg till författare i samlingen
            int johnIndex = authors.Add("John Doe", "john.doe", "provider1");
            int janeIndex = authors.Add("Jane Smith", "jane.smith", "provider2");

            // Hämta författarobjekten
            ThreadedCommentAuthor johnAuthor = authors[johnIndex];
            ThreadedCommentAuthor janeAuthor = authors[janeIndex];

            try
            {
                // Anropa IndexOf‑metoden för att hitta positionen för Jane Smith
                int foundIndex = authors.IndexOf(janeAuthor);
                
                // Visa resultatet
                Console.WriteLine($"Author '{janeAuthor.Name}' found at index: {foundIndex}");

                // Verifiera att resultatet matchar förväntat index
                if (foundIndex == janeIndex)
                {
                    Console.WriteLine("IndexOf result matches the expected index");
                }
                else
                {
                    Console.WriteLine("IndexOf result does not match the expected index");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IndexOf method: {ex.Message}");
            }
            
            // Spara arbetsboken
            workbook.Save("ThreadedCommentAuthorIndexOfDemo.xlsx");
        }
    }
}
```

### Se även

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


