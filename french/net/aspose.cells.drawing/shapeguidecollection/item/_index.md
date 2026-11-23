---
title: "ShapeGuideCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ShapeGuideCollection. Obtient un guide de forme par indice"
type: docs
url: /fr/net/aspose.cells.drawing/shapeguidecollection/item/
---
## ShapeGuideCollection indexer

Obtient un guide de forme par index

```csharp
public ShapeGuide this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice |  |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeGuideCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme qui utilise des guides d'ajustement
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.RightArrowCallout, 2, 0, 2, 0, 200, 150);

            // Accéder à la collection de guides d'ajustement de la forme via Geometry
            ShapeGuideCollection shapeGuides = shape.Geometry.ShapeAdjustValues;

            // Ajouter de nouveaux guides à la collection
            shapeGuides.Add("adj1", 25.5);
            shapeGuides.Add("adj2", 30);
            shapeGuides.Add("adj3", 25.5);
            shapeGuides.Add("adj4", 35);

            // Démontrer la lecture des valeurs de guide (la propriété Name n'est pas disponible dans la définition fournie)
            Console.WriteLine("First guide value: " + shapeGuides[0].Value);
            Console.WriteLine("Second guide value: " + shapeGuides[1].Value);
            Console.WriteLine("third guide value: " + shapeGuides[2].Value);
            Console.WriteLine("fourth guide value: " + shapeGuides[3].Value);

            // Enregistrer le classeur modifié
            workbook.Save("ShapeGuideCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ShapeGuide](../../shapeguide/)
* class [ShapeGuideCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


