---
title: "ShapeTextAlignment.NumberOfColumns"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ShapeTextAlignment. Obtient et définit le nombre de colonnes de texte dans le rectangle englobant"
type: docs
url: /fr/net/aspose.cells.drawing.texts/shapetextalignment/numberofcolumns/
---
## ShapeTextAlignment.NumberOfColumns property

Obtient et définit le nombre de colonnes de texte dans le rectangle englobant.

```csharp
public int NumberOfColumns { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyNumberOfColumnsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme à la feuille de calcul
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);
            
            // Définir le texte pour la forme
            shape.Text = "This is sample text\nin multiple columns";
            
            // Accéder à l'alignement du texte et définir le nombre de colonnes
            shape.TextBody.TextAlignment.NumberOfColumns = 2;
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
            
            // Vérifier la propriété
            Console.WriteLine("Number of columns: " + 
                worksheet.Shapes[0].TextBody.TextAlignment.NumberOfColumns);
        }
    }
}
```

### Voir aussi

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


