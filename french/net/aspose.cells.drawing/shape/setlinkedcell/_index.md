---
title: "Shape.SetLinkedCell"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Shape. Définit la plage liée à la valeur du contrôle"
type: docs
url: /fr/net/aspose.cells.drawing/shape/setlinkedcell/
---
## Shape.SetLinkedCell method

Définit la plage liée à la valeur du contrôle.

```csharp
public void SetLinkedCell(string formula, bool isR1C1, bool isLocal)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| formule | String | La plage liée à la valeur du contrôle. |
| isR1C1 | Boolean | Indique si la formule doit être formatée en R1C1. |
| isLocal | Boolean | Indique si la formule doit être formatée selon la locale. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ShapeMethodSetLinkedCellWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme de barre de défilement
            Aspose.Cells.Drawing.Shape scrollBar = worksheet.Shapes.AddScrollBar(2, 0, 2, 0, 130, 30);

            // Lier la valeur de la barre de défilement à la cellule A12
            scrollBar.SetLinkedCell("$A$12", false, true);

            // Enregistrez le classeur
            workbook.Save("SetLinkedCellDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


