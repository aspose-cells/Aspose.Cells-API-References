---
title: "ThreadedCommentAuthorCollection.IndexOf"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ThreadedCommentAuthorCollection metodo. Restituisce l'indice dell'oggetto ThreadedCommentAuthor"
type: docs
url: /it/net/aspose.cells/threadedcommentauthorcollection/indexof/
---
## ThreadedCommentAuthorCollection.IndexOf method

Restituisce l'indice dell'oggetto ThreadedCommentAuthor

```csharp
public int IndexOf(ThreadedCommentAuthor author)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| autore | ThreadedCommentAuthor | L'oggetto ThreadedCommentAuthor |

### Valore di ritorno

L'indice nella collezione ThreadedCommentAuthor

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentAuthorCollectionMethodIndexOfWithThreadedCommentAuthorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Ottieni la collezione degli autori dei commenti in thread
            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;

            // Aggiungi autori alla collezione
            int johnIndex = authors.Add("John Doe", "john.doe", "provider1");
            int janeIndex = authors.Add("Jane Smith", "jane.smith", "provider2");

            // Ottieni gli oggetti autore
            ThreadedCommentAuthor johnAuthor = authors[johnIndex];
            ThreadedCommentAuthor janeAuthor = authors[janeIndex];

            try
            {
                // Chiama il metodo IndexOf per trovare la posizione di Jane Smith
                int foundIndex = authors.IndexOf(janeAuthor);
                
                // Visualizza il risultato
                Console.WriteLine($"Author '{janeAuthor.Name}' found at index: {foundIndex}");

                // Verifica che il risultato corrisponda all'indice previsto
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
            
            // Salva la cartella di lavoro
            workbook.Save("ThreadedCommentAuthorIndexOfDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


