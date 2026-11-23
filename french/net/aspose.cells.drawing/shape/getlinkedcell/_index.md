---
title: "Shape.GetLinkedCell"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Shape. Obtient la plage liée à la valeur du contrôle"
type: docs
url: /fr/net/aspose.cells.drawing/shape/getlinkedcell/
---
## Shape.GetLinkedCell method

Obtient la plage liée à la valeur du contrôle.

```csharp
public string GetLinkedCell(bool isR1C1, bool isLocal)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| isR1C1 | Boolean | Indique si la formule doit être formatée en R1C1. |
| isLocal | Boolean | Indique si la formule doit être formatée selon la locale. |

### Valeur de retour

La plage liée à la valeur du contrôle.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetLinkedCellWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme et définir sa cellule liée
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
            shape.LinkedCell = "A1";

            // Obtenir l'adresse de la cellule liée avec différentes combinaisons de paramètres
            string link1 = shape.GetLinkedCell(false, false); // Returns absolute reference like "$A$1"
            string link2 = shape.GetLinkedCell(true, false);   // Returns relative reference like "A1"
            string link3 = shape.GetLinkedCell(false, true);   // Returns R1C1 style absolute reference

            Console.WriteLine("Linked cell (absolute A1): " + link1);
            Console.WriteLine("Linked cell (relative A1): " + link2);
            Console.WriteLine("Linked cell (R1C1 style): " + link3);
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


