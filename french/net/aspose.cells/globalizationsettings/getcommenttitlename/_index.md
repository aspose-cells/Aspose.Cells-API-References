---
title: "GlobalizationSettings.GetCommentTitleName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode GlobalizationSettings. Obtient le nom du titre du commentaire dépendant de la locale selon le type de titre de commentaire"
type: docs
url: /fr/net/aspose.cells/globalizationsettings/getcommenttitlename/
---
## GlobalizationSettings.GetCommentTitleName method

Obtient le nom du titre du commentaire dépendant de la langue selon le type de titre de commentaire.

```csharp
public virtual string GetCommentTitleName(CommentTitleType type)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | CommentTitleType |  |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class GlobalizationSettingsMethodGetCommentTitleNameWithCommentTitleTypeDemo : GlobalizationSettings
    {
        public override string GetCommentTitleName(CommentTitleType type)
        {
            switch (type)
            {
                case CommentTitleType.Cell:
                    return "Custom Cell Comment";
                case CommentTitleType.Reply:  // Changed from Threaded to Reply
                    return "Custom Threaded Comment";
                default:
                    return base.GetCommentTitleName(type);
            }
        }

        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new GlobalizationSettingsMethodGetCommentTitleNameWithCommentTitleTypeDemo(); // Changed to use Settings

            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter un commentaire de test
            int commentIndex = worksheet.Comments.Add("B5");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Test comment content";

            try
            {
                // Obtenir le titre du commentaire pour différents types
                var cellTitle = workbook.Settings.GlobalizationSettings.GetCommentTitleName(CommentTitleType.Cell); // Changed to use Settings
                var threadedTitle = workbook.Settings.GlobalizationSettings.GetCommentTitleName(CommentTitleType.Reply); // Changed type and Settings

                Console.WriteLine($"Cell Comment Title: {cellTitle}");
                Console.WriteLine($"Threaded Comment Title: {threadedTitle}");

                // Définir l'auteur du commentaire (titre) en utilisant nos paramètres de globalisation personnalisés
                comment.Author = cellTitle; // Changed from Title to Author
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCommentTitleName method: {ex.Message}");
            }

            workbook.Save("GetCommentTitleNameDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [CommentTitleType](../../../aspose.cells.rendering/commenttitletype/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


