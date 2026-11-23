---
title: "Shape.TopInch"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Représente le décalage vertical de la forme par rapport à sa ligne supérieure en pouces"
type: docs
url: /fr/net/aspose.cells.drawing/shape/topinch/
---
## Shape.TopInch property

Représente le décalage vertical de la forme par rapport à sa ligne supérieure, en pouces.

```csharp
public double TopInch { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTopInchDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme rectangulaire
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Définir et démontrer la propriété TopInch
            shape.TopInch = 3;
            Console.WriteLine("Shape Top position (inches): " + shape.TopInch);

            // Modifier TopInch si elle vaut 3
            if (shape.TopInch == 3)
            {
                shape.TopInch = 1;
                Console.WriteLine("Modified Shape Top position (inches): " + shape.TopInch);
            }

            // Enregistrez le classeur
            workbook.Save("ShapeTopInchDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


