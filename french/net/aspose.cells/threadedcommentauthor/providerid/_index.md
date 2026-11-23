---
title: "ThreadedCommentAuthor.ProviderId"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ThreadedCommentAuthor. Obtient l'identifiant du fournisseur"
type: docs
url: /fr/net/aspose.cells/threadedcommentauthor/providerid/
---
## ThreadedCommentAuthor.ProviderId property

Obtient l'identifiant du fournisseur.

```csharp
public string ProviderId { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentAuthorPropertyProviderIdDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Ajouter un auteur de commentaire en fil et obtenir son index
                int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("John Doe", "JD123", "PROVIDER123");
                
                // Obtenir l'objet ThreadedCommentAuthor
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];
                
                // Afficher la valeur ProviderId (opération de lecture)
                Console.WriteLine("Author ProviderId: " + author.ProviderId);
                
                // Créer un commentaire en fil en utilisant l'auteur
                worksheet.Comments.AddThreadedComment("A1", "This is a sample comment", author);
                
                // Enregistrez le classeur
                workbook.Save("ThreadedCommentAuthorDemo.xlsx");
                
                Console.WriteLine("Demo completed successfully.");
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


