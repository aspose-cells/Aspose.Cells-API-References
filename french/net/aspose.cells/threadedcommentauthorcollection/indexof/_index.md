---
title: "ThreadedCommentAuthorCollection.IndexOf"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ThreadedCommentAuthorCollection. Obtient l'index de l'objet ThreadedCommentAuthor"
type: docs
url: /fr/net/aspose.cells/threadedcommentauthorcollection/indexof/
---
## ThreadedCommentAuthorCollection.IndexOf method

Obtient l'index de l'objet ThreadedCommentAuthor

```csharp
public int IndexOf(ThreadedCommentAuthor author)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| auteur | ThreadedCommentAuthor | L'objet ThreadedCommentAuthor |

### Valeur de retour

L'index dans la collection ThreadedCommentAuthor

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentAuthorCollectionMethodIndexOfWithThreadedCommentAuthorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Obtenez la collection des auteurs de commentaires en fil
            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;

            // Ajoutez des auteurs à la collection
            int johnIndex = authors.Add("John Doe", "john.doe", "provider1");
            int janeIndex = authors.Add("Jane Smith", "jane.smith", "provider2");

            // Obtenez les objets auteur
            ThreadedCommentAuthor johnAuthor = authors[johnIndex];
            ThreadedCommentAuthor janeAuthor = authors[janeIndex];

            try
            {
                // Appelez la méthode IndexOf pour trouver la position de Jane Smith
                int foundIndex = authors.IndexOf(janeAuthor);
                
                // Afficher le résultat
                Console.WriteLine($"Author '{janeAuthor.Name}' found at index: {foundIndex}");

                // Vérifiez que le résultat correspond à l'index attendu
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
            
            // Enregistrez le classeur
            workbook.Save("ThreadedCommentAuthorIndexOfDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


