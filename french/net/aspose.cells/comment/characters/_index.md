---
title: "Comment.Characters"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Comment. Retourne un objet Characters qui représente une plage de caractères dans le texte du commentaire"
type: docs
url: /fr/net/aspose.cells/comment/characters/
---
## Comment.Characters method

Renvoie un objet Characters qui représente une plage de caractères dans le texte du commentaire.

```csharp
public FontSetting Characters(int startIndex, int length)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startIndex | Int32 | L'index du début du caractère. |
| longueur | Int32 | Le nombre de caractères. |

### Valeur de retour

Objet Characters.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentMethodCharactersWithInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter un commentaire à la cellule A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment1 = worksheet.Comments[commentIndex];
            comment1.Note = "This is a sample comment";
            
            // Obtenir le paramètre de police pour les 4 premiers caractères
            FontSetting fontSetting = comment1.Characters(0, 4);
            
            // Modifier les paramètres de police
            fontSetting.Font.Color = System.Drawing.Color.Red;
            fontSetting.Font.IsBold = true;
            
            // Enregistrez le classeur
            workbook.Save("CommentFontSettingDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [FontSetting](../../fontsetting/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


