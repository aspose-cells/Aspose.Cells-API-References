---
title: "Shape.MoveToRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Shape. Déplace la forme vers une plage spécifiée"
type: docs
url: /fr/net/aspose.cells.drawing/shape/movetorange/
---
## Shape.MoveToRange method

Déplace la forme vers une plage spécifiée.

```csharp
public void MoveToRange(int topRow, int leftColumn, int bottomRow, int rightColumn)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Indice de la ligne supérieure gauche. |
| leftColumn | Int32 | Indice de la colonne supérieure gauche. |
| bottomRow | Int32 | Index de la ligne du coin inférieur droit |
| rightColumn | Int32 | Index de la colonne du coin inférieur droit |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodMoveToRangeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme à la feuille de calcul
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Déplacez la forme vers une plage spécifique
            shape.MoveToRange(12, 3, 13, 5);

            // Enregistrez le classeur
            workbook.Save("ShapeMoveToRangeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


