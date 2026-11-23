---
title: "Shape.IsDecorative"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Shape property. Indique si l'objet est décoratif"
type: docs
url: /fr/net/aspose.cells.drawing/shape/isdecorative/
---
## Shape.IsDecorative property

Indique si l'objet est décoratif.

```csharp
public bool IsDecorative { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsDecorativeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une forme rectangulaire
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);
            
            // Définir le shape comme décoratif
            shape.IsDecorative = true;
            
            // Enregistrez le classeur
            string outputPath = "ShapeIsDecorativeDemo.xlsx";
            workbook.Save(outputPath);
            
            // Recharger le workbook pour vérifier la propriété
            Workbook loadedWorkbook = new Workbook(outputPath);
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            
            // Afficher le résultat
            Console.WriteLine("Shape IsDecorative property: " + loadedShape.IsDecorative);
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


