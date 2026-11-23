---
title: "Cell.Comment"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cell. Obtient le commentaire de cette cellule"
type: docs
url: /fr/net/aspose.cells/cell/comment/
---
## Cell.Comment property

Obtient le commentaire de cette cellule.

```csharp
public Comment Comment { get; }
```

### Remarques

S'il n'y a aucun commentaire appliqué à la cellule, renvoie null.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellPropertyCommentDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un commentaire à la cellule A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Cell");

            // Ajouter un commentaire à la cellule
            Comment comment = cell.Comment;
            if (comment == null)
            {
                // Créer un nouveau commentaire s'il n'en existe pas
                int commentIndex = worksheet.Comments.Add("A1");
                comment = worksheet.Comments[commentIndex];
                comment.Author = "Author Name";
                comment.Note = "This is a sample comment";
            }

            try
            {
                // Afficher les propriétés du commentaire
                Console.WriteLine("Comment Author: " + comment.Author);
                Console.WriteLine("Comment Note: " + comment.Note);
                Console.WriteLine("Comment Row: " + comment.Row);
                Console.WriteLine("Comment Column: " + comment.Column);
                Console.WriteLine("Comment is Visible: " + comment.IsVisible);

                // Modifier certaines propriétés du commentaire
                comment.Note = "Updated comment text";
                comment.IsVisible = true;

                // Afficher la note de commentaire mise à jour
                Console.WriteLine("Updated Comment Note: " + comment.Note);

                // Enregistrez le classeur
                workbook.Save("CommentDemo.xlsx");
                Console.WriteLine("Comment has been demonstrated and saved to CommentDemo.xlsx");
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

* class [Comment](../../comment/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


