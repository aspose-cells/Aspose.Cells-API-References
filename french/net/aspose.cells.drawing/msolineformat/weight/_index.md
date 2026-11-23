---
title: "MsoLineFormat.Weight"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MsoLineFormat. Retourne ou définit l'épaisseur de la ligne en unités de pt"
type: docs
url: /fr/net/aspose.cells.drawing/msolineformat/weight/
---
## MsoLineFormat.Weight property

Renvoie ou définit l'épaisseur de la ligne, en unités de pt.

```csharp
public double Weight { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyWeightDemo
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
            
            // Accéder au format de ligne de la forme de commentaire et définir l'épaisseur
            comment.CommentShape.LineFormat.Weight = 0.75;
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
            
            // Vérifier que l'épaisseur a été définie correctement
            Console.WriteLine("Line weight: " + worksheet.Comments[0].CommentShape.LineFormat.Weight);
        }
    }
}
```

### Voir aussi

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


