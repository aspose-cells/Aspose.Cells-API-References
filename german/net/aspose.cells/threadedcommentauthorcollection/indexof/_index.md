---
title: "ThreadedCommentAuthorCollection.IndexOf"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ThreadedCommentAuthorCollection-Methode. Gibt den Index des ThreadedCommentAuthor-Objekts zurück"
type: docs
url: /de/net/aspose.cells/threadedcommentauthorcollection/indexof/
---
## ThreadedCommentAuthorCollection.IndexOf method

Ermittelt den Index des ThreadedCommentAuthor-Objekts

```csharp
public int IndexOf(ThreadedCommentAuthor author)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Autor | ThreadedCommentAuthor | Das ThreadedCommentAuthor-Objekt |

### Rückgabewert

Der Index in der ThreadedCommentAuthor-Sammlung

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentAuthorCollectionMethodIndexOfWithThreadedCommentAuthorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Holen Sie die ThreadedCommentAuthor-Autoren-Sammlung
            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;

            // Fügen Sie Autoren zur Sammlung hinzu
            int johnIndex = authors.Add("John Doe", "john.doe", "provider1");
            int janeIndex = authors.Add("Jane Smith", "jane.smith", "provider2");

            // Holen Sie die Autor-Objekte
            ThreadedCommentAuthor johnAuthor = authors[johnIndex];
            ThreadedCommentAuthor janeAuthor = authors[janeIndex];

            try
            {
                // Rufen Sie die IndexOf-Methode auf, um die Position von Jane Smith zu finden
                int foundIndex = authors.IndexOf(janeAuthor);
                
                // Ergebnis anzeigen
                Console.WriteLine($"Author '{janeAuthor.Name}' found at index: {foundIndex}");

                // Überprüfen Sie, ob das Ergebnis dem erwarteten Index entspricht
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
            
            // Speichere die Arbeitsmappe
            workbook.Save("ThreadedCommentAuthorIndexOfDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


