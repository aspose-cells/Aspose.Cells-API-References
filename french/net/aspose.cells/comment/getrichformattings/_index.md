---
title: "Comment.GetRichFormattings"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Comment méthode. Retourne tous les objets Characters qui représentent une plage de caractères dans le texte du commentaire"
type: docs
url: /fr/net/aspose.cells/comment/getrichformattings/
---
## Comment.GetRichFormattings method

Renvoie tous les objets Characters qui représentent une plage de caractères dans le texte du commentaire.

```csharp
public FontSetting[] GetRichFormattings()
```

### Valeur de retour

Tous les objets Characters

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentMethodGetRichFormattingsDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un commentaire à la cellule A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.HtmlNote = "<b>Bold</b>, <i>Italic</i>, <u>Underline</u>";

            // Obtenir les mises en forme de texte enrichi
            FontSetting[] formattings = comment.GetRichFormattings();

            // Afficher les informations de mise en forme
            Console.WriteLine("Rich Text Formattings:");
            foreach (FontSetting setting in formattings)
            {
                Console.WriteLine($"StartIndex: {setting.StartIndex}, Length: {setting.Length}");
                Console.WriteLine($"Bold: {setting.Font.IsBold}, Italic: {setting.Font.IsItalic}, Underline: {setting.Font.Underline}");
            }
        }
    }
}
```

### Voir aussi

* class [FontSetting](../../fontsetting/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


