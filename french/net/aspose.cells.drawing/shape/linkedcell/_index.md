---
title: "Shape.LinkedCell"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Obtient ou définit la plage de la feuille liée à la valeur du contrôle"
type: docs
url: /fr/net/aspose.cells.drawing/shape/linkedcell/
---
## Shape.LinkedCell property

Obtient ou définit la plage de la feuille de calcul liée à la valeur du contrôle.

```csharp
public string LinkedCell { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLinkedCellDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme à la feuille de calcul
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Définir la propriété LinkedCell à B6
            shape.LinkedCell = "$B$6";

            // Modifier le LinkedCell en A1 s'il était B6
            if (shape.LinkedCell.Equals("$B$6"))
            {
                shape.LinkedCell = "A1";
            }

            // Afficher la valeur actuelle du LinkedCell
            Console.WriteLine("Shape's LinkedCell: " + shape.LinkedCell);
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


