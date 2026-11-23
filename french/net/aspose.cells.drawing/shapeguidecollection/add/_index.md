---
title: "ShapeGuideCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeGuideCollection. Ajoute un guide de forme. Important : cette fonctionnalité n'est actuellement disponible que pour Excel07 et versions ultérieures"
type: docs
url: /fr/net/aspose.cells.drawing/shapeguidecollection/add/
---
## ShapeGuideCollection.Add method

Ajoute un guide de forme.(Important : Cette fonctionnalité n'est actuellement disponible que pour Excel07 et versions ultérieures)

```csharp
public int Add(string name, double val)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | le nom de adjust. C'est "adj (Utilisé lorsqu'il n'y a qu'une seule valeur d'ajustement)", "adj1", "adj2", "adj3" etc. |
| val | Double | la valeur de adjust |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeGuideCollectionMethodAddWithStringDoubleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur et accéder à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une forme qui utilise des guides d'ajustement
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.RightArrowCallout, 2, 0, 2, 0, 200, 150);

            try
            {
                // Obtenir le ShapeGuideCollection à partir des ajustements de géométrie de forme
                ShapeGuideCollection shapeGuides = shape.Geometry.ShapeAdjustValues;

                // Appeler la méthode Add avec des paramètres (String, Double)
                shapeGuides.Add("adj1", 25.5);
                shapeGuides.Add("adj2", 25.5);
                shapeGuides.Add("adj3", 25.5);
                shapeGuides.Add("adj4", 25.5);

                Console.WriteLine($"Total guides after addition: {shapeGuides.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }

            // Enregistrer le classeur modifié
            workbook.Save("ShapeGuideAddWithStringDoubleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ShapeGuideCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


