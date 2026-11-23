---
title: "Cells.DeleteRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Supprime une plage de cellules et décale les cellules selon l'option de décalage"
type: docs
url: /fr/net/aspose.cells/cells/deleterange/
---
## Cells.DeleteRange method

Supprime une plage de cellules et décale les cellules selon l'option de décalage.

```csharp
public void DeleteRange(int startRow, int startColumn, int endRow, int endColumn, 
    ShiftType shiftType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Indice de ligne de départ. |
| startColumn | Int32 | Indice de colonne de départ. |
| endRow | Int32 | Indice de ligne de fin. |
| endColumn | Int32 | Indice de colonne de fin. |
| shiftType | ShiftType | Option de déplacement des cellules. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRangeWithInt32Int32Int32Int32ShiftTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Remplir des données d'exemple
            sheet.Cells["A1"].PutValue("A1");
            sheet.Cells["B1"].PutValue("B1");
            sheet.Cells["C1"].PutValue("C1");
            sheet.Cells["A2"].PutValue("A2");
            sheet.Cells["B2"].PutValue("B2");
            sheet.Cells["C2"].PutValue("C2");

            // Supprimez la plage et décalez à gauche
            sheet.Cells.DeleteRange(0, 1, 1, 2, ShiftType.Left);

            // Enregistrez le classeur
            workbook.Save("DeleteRangeExample.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


