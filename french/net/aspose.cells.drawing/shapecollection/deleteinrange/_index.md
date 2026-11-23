---
title: "ShapeCollection.DeleteInRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeCollection. Supprime les formes dans la plage.Comment les formes de commentaire ne seront pas supprimées"
type: docs
url: /fr/net/aspose.cells.drawing/shapecollection/deleteinrange/
---
## ShapeCollection.DeleteInRange method

Supprime les formes dans la plage.Comment les formes de commentaire ne seront pas supprimées.

```csharp
public void DeleteInRange(CellArea ca)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ca | CellArea | La plage.Si les formes sont contenues dans la plage, elles seront supprimées. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodDeleteInRangeWithCellAreaDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // Ajouter la première forme de rectangle
            shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            // Ajouter la deuxième forme de rectangle
            shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // Définir la plage où les formes doivent être supprimées
            CellArea area = new CellArea();
            area.StartColumn = 0;
            area.StartRow = 5;
            area.EndColumn = 5;
            area.EndRow = 8;

            // Supprimer les formes dans la plage spécifiée
            shapes.DeleteInRange(area);

            // Enregistrer le classeur (facultatif)
            workbook.Save("ShapeDeleteInRangeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


