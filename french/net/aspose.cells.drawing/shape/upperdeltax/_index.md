---
title: "Shape.UpperDeltaX"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Obtient ou définit le décalage horizontal de la forme par rapport à la colonne de son coin supérieur gauche"
type: docs
url: /fr/net/aspose.cells.drawing/shape/upperdeltax/
---
## Shape.UpperDeltaX property

Obtient ou définit le décalage horizontal de la forme depuis la colonne de son coin supérieur gauche.

```csharp
public int UpperDeltaX { get; set; }
```

### Remarques

La plage de valeurs est de 0 à 1024.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyUpperDeltaXDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme à la feuille de calcul
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Définir et afficher la propriété UpperDeltaX
            shape.UpperDeltaX = 150;
            Console.WriteLine("UpperDeltaX: " + shape.UpperDeltaX);

            // Modifier UpperDeltaX si elle satisfait une condition
            if (shape.UpperDeltaX == 150)
            {
                shape.UpperDeltaX = 100;
                Console.WriteLine("Modified UpperDeltaX: " + shape.UpperDeltaX);
            }
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


