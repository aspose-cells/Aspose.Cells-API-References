---
title: "SettableGlobalizationSettings.SetCommentTitleName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettableGlobalizationSettings. Obtient le nom du titre de commentaire dépendant de la locale selon le type de titre de commentaire"
type: docs
url: /fr/net/aspose.cells/settableglobalizationsettings/setcommenttitlename/
---
## SettableGlobalizationSettings.SetCommentTitleName method

Obtient le nom du titre du commentaire dépendant de la langue selon le type de titre de commentaire.

```csharp
public void SetCommentTitleName(CommentTitleType type, string name)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | CommentTitleType | type de titre de commentaire |
| name | String | nom du titre du commentaire dépendant de la locale |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SettableGlobalizationSettingsMethodSetCommentTitleNameWithCommentTitleTypeStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un commentaire à la cellule A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a sample comment";
            comment.IsVisible = true;

            // Créer des paramètres de mondialisation
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Définir des noms de titre de commentaire personnalisés pour différents types
                settings.SetCommentTitleName(CommentTitleType.Cell, "Custom Cell Title");
                settings.SetCommentTitleName(CommentTitleType.Comment, "Custom Comment Title");
                settings.SetCommentTitleName(CommentTitleType.Note, "Custom Note Title");
                settings.SetCommentTitleName(CommentTitleType.Reply, "Custom Reply Title");

                // Appliquer les paramètres de globalisation au classeur
                workbook.Settings.GlobalizationSettings = settings;

                Console.WriteLine("SetCommentTitleName method executed successfully with parameters (CommentTitleType, String)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetCommentTitleName method: {ex.Message}");
            }

            // Enregistrez le classeur
            workbook.Save("MethodSetCommentTitleNameDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [CommentTitleType](../../../aspose.cells.rendering/commenttitletype/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


