---
title: "MsoFillFormat.Transparency"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MsoFillFormat. Retourne ou définit le degré de transparence du remplissage spécifié comme une valeur de 0,0 opaque à 1,0 clair"
type: docs
url: /fr/net/aspose.cells.drawing/msofillformat/transparency/
---
## MsoFillFormat.Transparency property

Renvoie ou définit le degré de transparence du remplissage spécifié sous forme d'une valeur comprise entre 0.0 (opaque) et 1.0 (transparent).

```csharp
public double Transparency { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFillFormatPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un commentaire à la cellule A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a test comment";

            // Définissez les propriétés du format de remplissage, y compris la transparence
            comment.CommentShape.FillFormat.IsVisible = true;
            comment.CommentShape.FillFormat.ForeColor = System.Drawing.Color.Red;
            comment.CommentShape.FillFormat.BackColor = System.Drawing.Color.Yellow;
            
            // Définissez la transparence (0,0 = totalement opaque, 1,0 = totalement transparent)
            comment.CommentShape.FillFormat.Transparency = 0.5;

            // Enregistrez le classeur
            workbook.Save("CommentTransparencyDemo.xlsx");

            // Chargez le classeur enregistré pour vérifier la transparence
            Workbook verifyWorkbook = new Workbook("CommentTransparencyDemo.xlsx");
            Comment verifyComment = verifyWorkbook.Worksheets[0].Comments[0];
            
            // Affichez la valeur de transparence pour démontrer qu'elle a été enregistrée et chargée correctement
            Console.WriteLine("Comment fill transparency: " + 
                verifyComment.CommentShape.FillFormat.Transparency);
        }
    }
}
```

### Voir aussi

* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


