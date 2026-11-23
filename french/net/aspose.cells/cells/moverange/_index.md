---
title: "Cells.MoveRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Déplace la plage"
type: docs
url: /fr/net/aspose.cells/cells/moverange/
---
## Cells.MoveRange method

Déplace la plage.

```csharp
public void MoveRange(CellArea sourceArea, int destRow, int destColumn)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sourceArea | CellArea | La plage qui doit être déplacée. |
| destRow | Int32 | La ligne de destination. |
| destColumn | Int32 | La colonne de destination. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodMoveRangeWithCellAreaInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Insérer des valeurs dans les cellules
            cells["A1"].PutValue("Original");
            cells["B1"].PutValue(100);
            cells["A2"].PutValue("Data");
            cells["B2"].PutValue(200);

            // Définissez la zone de cellules à déplacer (A1:B2)
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 1;
            area.EndColumn = 1;

            // Déplacez la plage de 2 lignes vers le bas et de 3 colonnes vers la droite
            cells.MoveRange(area, 2, 3);

            // Enregistrez le classeur
            workbook.Save("MoveRangeExample.xlsx");
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


