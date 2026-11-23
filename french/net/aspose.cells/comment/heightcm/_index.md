---
title: "Comment.HeightCM"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Comment. Représente la hauteur du commentaire en centimètres"
type: docs
url: /fr/net/aspose.cells/comment/heightcm/
---
## Comment.HeightCM property

Représente la hauteur du commentaire, en centimètres.

```csharp
public double HeightCM { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyHeightCMDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter un commentaire à la cellule A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // Définir le texte du commentaire
            comment.Note = "Sample comment";
            
            // Définir la hauteur du commentaire en centimètres
            comment.HeightCM = 1.5;
            
            // Enregistrez le classeur
            workbook.Save("CommentHeightCMDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


