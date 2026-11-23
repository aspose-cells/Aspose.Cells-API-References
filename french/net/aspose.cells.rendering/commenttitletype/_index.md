---
title: "Énumération CommentTitleType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.Rendering.CommentTitleType. Représente le type de titre de commentaire lors du rendu lorsque le commentaire est configuré pour s'afficher à la fin de la feuille"
type: docs
url: /fr/net/aspose.cells.rendering/commenttitletype/
---
## CommentTitleType enumeration

Représente le type de titre de commentaire lors du rendu lorsque le commentaire est configuré pour s'afficher à la fin de la feuille.

```csharp
public enum CommentTitleType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Cell | `0` | Représente la cellule de titre de commentaire. |
| Comment | `1` | Représente le commentaire du titre de commentaire. |
| Note | `2` | Représente la note du titre de commentaire. |
| Reply | `3` | Représente la réponse du titre de commentaire. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassCommentTitleTypeDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Créer des paramètres de mondialisation personnalisés
                SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

                // Démontrer toutes les valeurs de l'énumération CommentTitleType
                Console.WriteLine("Available CommentTitleType values:");
                Console.WriteLine($"Cell: {(int)CommentTitleType.Cell}");
                Console.WriteLine($"Comment: {(int)CommentTitleType.Comment}");
                Console.WriteLine($"Note: {(int)CommentTitleType.Note}");
                Console.WriteLine($"Reply: {(int)CommentTitleType.Reply}");

                // Définir des titres personnalisés pour chaque type de commentaire
                globalizationSettings.SetCommentTitleName(CommentTitleType.Cell, "Custom Cell Title");
                globalizationSettings.SetCommentTitleName(CommentTitleType.Comment, "Custom Comment Title");
                globalizationSettings.SetCommentTitleName(CommentTitleType.Note, "Custom Note Title");
                globalizationSettings.SetCommentTitleName(CommentTitleType.Reply, "Custom Reply Title");

                // Appliquer les paramètres de globalisation au classeur
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                // Ajouter un commentaire pour démontrer la fonctionnalité
                int commentIndex = worksheet.Comments.Add("A1");
                Comment comment = worksheet.Comments[commentIndex];
                comment.Note = "This is a test comment";
                comment.Author = "Test Author";

                // Enregistrez le classeur
                workbook.Save("CommentTitleTypeDemo.xlsx");

                Console.WriteLine("CommentTitleType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in CommentTitleType demonstration: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


