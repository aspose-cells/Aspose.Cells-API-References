---
title: "ThreadedComment.Author"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ThreadedComment. Obtient l'auteur du commentaire"
type: docs
url: /fr/net/aspose.cells/threadedcomment/author/
---
## ThreadedComment.Author property

Obtient l'auteur du commentaire.

```csharp
public ThreadedCommentAuthor Author { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentPropertyAuthorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Obtenir l'auteur de commentaire en fil par défaut du classeur
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[0];
                author.Name = "John Doe";
                author.UserId = "john.doe@example.com";

                // Ajouter un commentaire en fil à la cellule A1 (ligne 0, colonne 0)
                worksheet.Comments.AddThreadedComment(0, 0, "Sample comment", author);

                // Obtenir le premier commentaire en fil
                ThreadedComment comment = worksheet.Comments[0].ThreadedComments[0];

                // Afficher la valeur de la propriété Author (opération de lecture)
                Console.WriteLine("Author Name: " + comment.Author.Name);
                Console.WriteLine("Author UserId: " + comment.Author.UserId);
                Console.WriteLine("Author ProviderId: " + comment.Author.ProviderId);

                // Démontrer la définition de la propriété Author (puisqu'elle est en lecture/écriture)
                ThreadedCommentAuthor newAuthor = workbook.Worksheets.ThreadedCommentAuthors[0];
                newAuthor.Name = "Jane Smith";
                newAuthor.UserId = "jane.smith@example.com";
                comment.Author = newAuthor;

                // Afficher la valeur mise à jour de la propriété Author
                Console.WriteLine("Updated Author Name: " + comment.Author.Name);
                Console.WriteLine("Updated Author UserId: " + comment.Author.UserId);

                // Enregistrez le classeur
                workbook.Save("ThreadedCommentAuthorDemo.xlsx");
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

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedComment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


