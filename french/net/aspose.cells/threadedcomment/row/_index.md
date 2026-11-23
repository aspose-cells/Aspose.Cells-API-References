---
title: "ThreadedComment.Row"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ThreadedComment. Obtient l'index de ligne du commentaire"
type: docs
url: /fr/net/aspose.cells/threadedcomment/row/
---
## ThreadedComment.Row property

Obtient l'index de ligne du commentaire.

```csharp
public int Row { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentPropertyRowDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Créer un auteur de commentaire en fil
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[0];
                author.Name = "Test Author";
                author.UserId = "test@example.com";
                
                // Ajouter un commentaire en fil à la cellule B2 (ligne 1, colonne 1)
                worksheet.Comments.AddThreadedComment(1, 1, "Sample threaded comment", author);
                
                // Obtenir le premier commentaire en fil
                ThreadedComment comment = worksheet.Comments[0].ThreadedComments[0];
                
                // Afficher la valeur de la propriété Row (lecture seule)
                Console.WriteLine("Threaded comment row index: " + comment.Row);
                
                // Vérifier que l'index de ligne correspond à l'endroit où nous avons placé le commentaire
                if (comment.Row == 1)
                {
                    Console.WriteLine("Comment is correctly placed in row 1");
                }
                
                // Enregistrez le classeur
                workbook.Save("ThreadedCommentRowDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [ThreadedComment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


