---
title: "ThreadedCommentCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ThreadedCommentCollection. Ajoute un commentaire en fil de discussion"
type: docs
url: /fr/net/aspose.cells/threadedcommentcollection/add/
---
## ThreadedCommentCollection.Add method

Ajoute un commentaire en fil de discussion.

```csharp
public int Add(string text, ThreadedCommentAuthor author)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| texte | String | Le texte du commentaire en fil de discussion. |
| auteur | ThreadedCommentAuthor | L'auteur du commentaire en fil de discussion |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentCollectionMethodAddWithStringThreadedCommentDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données pour le contexte
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Créer un auteur de commentaire en fil de discussion en utilisant ThreadedCommentAuthorCollection
                ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
                int authorIndex = authors.Add("John Doe", "john.doe@example.com", "EXAMPLE_PROVIDER");
                ThreadedCommentAuthor author = authors[authorIndex];

                // Accéder à la collection de commentaires en fil de discussion d'une cellule
                Comment comment = worksheet.Comments[worksheet.Comments.Add("A1")];
                ThreadedCommentCollection threadedComments = comment.ThreadedComments;

                // Appeler la méthode Add avec les paramètres String et ThreadedCommentAuthor
                int commentIndex = threadedComments.Add("This is a threaded comment", author);

                // Afficher le résultat
                Console.WriteLine($"Added threaded comment at index: {commentIndex}");
                Console.WriteLine($"Comment text: {threadedComments[commentIndex].Notes}");
                Console.WriteLine($"Author: {threadedComments[commentIndex].Author.Name}");

                // Enregistrez le classeur
                workbook.Save("ThreadedCommentAddDemo.xlsx");
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

### Voir aussi

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedCommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


