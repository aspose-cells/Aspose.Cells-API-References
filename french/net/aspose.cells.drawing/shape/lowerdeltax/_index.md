---
title: "Shape.LowerDeltaX"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Obtient ou définit le décalage horizontal de la forme depuis la colonne de son coin inférieur droit"
type: docs
url: /fr/net/aspose.cells.drawing/shape/lowerdeltax/
---
## Shape.LowerDeltaX property

Obtient ou définit le décalage horizontal de la forme par rapport à la colonne de son coin inférieur droit.

```csharp
public int LowerDeltaX { get; set; }
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
    public class ShapePropertyLowerDeltaXDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme rectangulaire
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Définir et démontrer la propriété LowerDeltaX
            shape.LowerDeltaX = 3;
            Console.WriteLine("Initial LowerDeltaX: " + shape.LowerDeltaX);

            // Modifier LowerDeltaX si la condition est remplie
            if (shape.LowerDeltaX == 3)
            {
                shape.LowerDeltaX = 1;
                Console.WriteLine("Modified LowerDeltaX: " + shape.LowerDeltaX);
            }
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


