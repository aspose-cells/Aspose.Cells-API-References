---
title: "Worksheet.Shapes"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Retourne toutes les formes de dessin dans cette feuille de calcul"
type: docs
url: /fr/net/aspose.cells/worksheet/shapes/
---
## Worksheet.Shapes property

Renvoie toutes les formes de dessin de cette feuille de calcul.

```csharp
public ShapeCollection Shapes { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyShapesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ajouter quelques formes à la feuille de calcul
            sheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
            sheet.Shapes.AddLine(2, 0, 100, 100, 100, 1);
            
            // Modifier les propriétés des formes
            for (int i = 0; i < sheet.Shapes.Count; i++)
            {
                Aspose.Cells.Drawing.Shape shape = sheet.Shapes[i];
                Console.WriteLine($"Shape {i}: Type={shape.Type}, Name={shape.Name}");
                
                // Mettre à jour les propriétés de la première forme
                if (i == 0)
                {
                    shape.Name = "MyRectangle";
                    shape.FillFormat.ForeColor = System.Drawing.Color.Red;
                }
            }
            
            // Enregistrez le classeur
            workbook.Save("ShapesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ShapeCollection](../../../aspose.cells.drawing/shapecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


