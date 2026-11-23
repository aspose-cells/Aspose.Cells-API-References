---
title: "ThreadedComment.Notes"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ThreadedComment. Obtient et définit le texte du commentaire"
type: docs
url: /fr/net/aspose.cells/threadedcomment/notes/
---
## ThreadedComment.Notes property

Obtient et définit le texte du commentaire.

```csharp
public string Notes { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentPropertyNotesDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Créer ou obtenir un auteur de commentaire en fil
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors["User1"];
                author.Name = "User1";

                // Ajouter un commentaire en fil à la cellule A1 (ligne 0, colonne 0) avec le texte initial
                worksheet.Comments.AddThreadedComment(0, 0, "Initial comment text", author);

                // Récupérer le commentaire en fil nouvellement ajouté
                ThreadedComment threadedComment = worksheet.Comments[0].ThreadedComments[0];

                // Mettre à jour la propriété Notes (le texte du commentaire)
                threadedComment.Notes = "Updated comment notes";

                // Lire et afficher la valeur de la propriété Notes
                Console.WriteLine("Threaded comment Notes: " + threadedComment.Notes);

                // Enregistrer le classeur (facultatif)
                workbook.Save("ThreadedCommentNotesDemo.xlsx");
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


