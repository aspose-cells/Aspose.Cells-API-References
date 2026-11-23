---
title: "ShapeSegmentPath.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ShapeSegmentPath. Obtient le type du segment de chemin"
type: docs
url: /fr/net/aspose.cells.drawing/shapesegmentpath/type/
---
## ShapeSegmentPath.Type property

Obtient le type de segment de chemin

```csharp
public ShapePathType Type { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeSegmentPathPropertyTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                //Créer un nouveau chemin de forme
                ShapePath shapePath = new ShapePath();

                // Déplacer vers le point de départ
                shapePath.MoveTo(10, 10);

                // Appeler la méthode LineTo avec les paramètres (Single, Single)
                shapePath.LineTo(50.5f, 10.5f);
                shapePath.LineTo(50.5f, 50.5f);
                shapePath.LineTo(10.5f, 50.5f);
                shapePath.Close();

                // Accéder à la propriété PathSegementList
                ShapeSegmentPathCollection segmentList = shapePath.PathSegementList;

                // Afficher le nombre de segments de chemin
                Console.WriteLine("Number of path segments: " + segmentList.Count);

                // Itérer à travers chaque segment et afficher son type
                foreach (ShapeSegmentPath segment in segmentList)
                {
                    Console.WriteLine("Segment type: " + segment.Type);
                }

                //ajouter une forme libre
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });

            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing LineTo method: {ex.Message}");
            }


            // Enregistrez le classeur
            workbook.Save("ShapeSegmentPathTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ShapePathType](../../shapepathtype/)
* class [ShapeSegmentPath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


