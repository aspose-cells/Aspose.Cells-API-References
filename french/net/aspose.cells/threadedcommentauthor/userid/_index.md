---
title: "ThreadedCommentAuthor.UserId"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ThreadedCommentAuthor. Obtient et définit l'identifiant de l'utilisateur"
type: docs
url: /fr/net/aspose.cells/threadedcommentauthor/userid/
---
## ThreadedCommentAuthor.UserId property

Obtient et définit l'identifiant de l'utilisateur.

```csharp
public string UserId { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentAuthorPropertyUserIdDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Ajouter un auteur de commentaire en fil avec le nom, userId et providerId
                int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("John Doe", "JD123", "PROVIDER123");

                // Obtenir l'objet ThreadedCommentAuthor
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];

                // Afficher la valeur UserId (opération de lecture)
                Console.WriteLine("Author UserId: " + author.UserId);

                // Démontrer la définition d'un nouveau UserId (opération d'écriture)
                author.UserId = "NEW_USER_ID";
                Console.WriteLine("Updated UserId: " + author.UserId);

                // Créer un commentaire en fil en utilisant l'auteur
                worksheet.Comments.AddThreadedComment("A1", "This is a sample comment", author);

                // Enregistrez le classeur
                workbook.Save("UserIdDemo.xlsx");

                Console.WriteLine("UserId property demonstration completed successfully.");
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

* class [ThreadedCommentAuthor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


