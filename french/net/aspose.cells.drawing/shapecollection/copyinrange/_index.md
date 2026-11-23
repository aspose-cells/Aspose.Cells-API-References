---
title: "ShapeCollection.CopyInRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeCollection. Copie les formes de la plage vers la plage de destination"
type: docs
url: /fr/net/aspose.cells.drawing/shapecollection/copyinrange/
---
## ShapeCollection.CopyInRange method

Copie les formes de la plage vers la plage de destination.

```csharp
public void CopyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, 
    bool isContained)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sourceShapes | ShapeCollection | Formes source. |
| ca | CellArea | La plage source. |
| destRow | Int32 | L'index de ligne de destination de la plage de destination. |
| destColumn | Int32 | La colonne de destination de la plage de destination. |
| isContained | Boolean | Indique s'il faut uniquement copier les formes contenues dans la plage. Si vrai, seules les formes de la plage sont copiées. Sinon, le comportement est celui de MS Office. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodCopyInRangeWithShapeCollectionCellAreaInt32InDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtenir la collection de formes
            ShapeCollection shapes = worksheet.Shapes;

            // Ajouter une forme rectangulaire
            shapes.AddRectangle(2, 0, 2, 0, 130, 130);

            // Définir la zone de cellules à copier depuis
            CellArea area2 = new CellArea();
            area2.StartColumn = 1;
            area2.StartRow = 1;
            area2.EndColumn = 5;
            area2.EndRow = 11;

            // Copier les formes dans la plage spécifiée
            shapes.CopyInRange(shapes, area2, 12, 1, false);

            // Enregistrez le classeur
            workbook.Save("ShapeCopyDemo.xlsx");
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


