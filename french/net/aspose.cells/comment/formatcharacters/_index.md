---
title: "Comment.FormatCharacters"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Comment. Formate certains caractères avec le paramètre de police"
type: docs
url: /fr/net/aspose.cells/comment/formatcharacters/
---
## Comment.FormatCharacters method

Formate certains caractères avec le réglage de police.

```csharp
public void FormatCharacters(int startIndex, int length, Font font, StyleFlag flag)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startIndex | Int32 | L'index de départ. |
| longueur | Int32 | La longueur. |
| police | Police | Le paramètre de police. |
| flag | StyleFlag | Le drapeau du paramètre de police. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CommentMethodFormatCharactersWithInt32Int32FontStyleFlagDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un commentaire à la cellule A1
            int commentRow = 0;
            int commentColumn = 0;
            Comment comment = worksheet.Comments[commentRow, commentColumn];
            comment.Note = "This is a sample comment with formatted text.";

            // Créer une police pour le formatage - doit être obtenue à partir du style du classeur
            Aspose.Cells.Font font = workbook.CreateStyle().Font;
            font.IsBold = true;
            font.Color = Color.Red;
            font.Size = 14;
            font.Underline = FontUnderlineType.Single;

            // Créer un drapeau de style pour spécifier quelles propriétés de police appliquer
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontBold = true;
            styleFlag.FontColor = true;
            styleFlag.FontSize = true;
            styleFlag.FontUnderline = true;

            try
            {
                // Formater les caractères à partir de l'index 5, longueur 10
                comment.FormatCharacters(5, 10, font, styleFlag);

                Console.WriteLine("FormatCharacters method executed successfully on the comment.");
                
                // Rendre le commentaire visible pour voir l'effet
                comment.IsVisible = true;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing FormatCharacters method: {ex.Message}");
            }
            
            // Enregistrez le classeur
            workbook.Save("CommentFormatCharactersDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Font](../../font/)
* class [StyleFlag](../../styleflag/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


