---
title: "ThreadedComment.Column"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ThreadedComment. Obtient l'index de colonne du commentaire"
type: docs
url: /fr/net/aspose.cells/threadedcomment/column/
---
## ThreadedComment.Column property

Obtient l'index de colonne du commentaire.

```csharp
public int Column { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentPropertyColumnDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Créez d'abord un auteur de commentaire en fil
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[0];
                
                // Ajouter un commentaire en fil à la cellule A1 (ligne 0, colonne 0)
                int commentRow = 0;
                int commentColumn = 0;
                worksheet.Comments.AddThreadedComment(commentRow, commentColumn, "Sample comment text", author);
                
                // Obtenir le premier commentaire en fil
                ThreadedComment comment = worksheet.Comments[0].ThreadedComments[0];
                
                // Affichez la valeur de la propriété Column (lecture seule)
                Console.WriteLine("Threaded comment column index: " + comment.Column);
                
                // Vérifiez que l'index de colonne correspond à l'endroit où nous avons placé le commentaire
                if (comment.Column == commentColumn)
                {
                    Console.WriteLine("Comment is correctly placed in column " + commentColumn);
                }
                
                // Enregistrez le classeur
                workbook.Save("ThreadedCommentColumnDemo.xlsx");
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


