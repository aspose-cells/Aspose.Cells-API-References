---
title: "Cell.IsMerged"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cell. Vérifie si une cellule fait partie d'une plage fusionnée ou non"
type: docs
url: /fr/net/aspose.cells/cell/ismerged/
---
## Cell.IsMerged property

Vérifie si une cellule fait partie d'une plage fusionnée ou non.

```csharp
public bool IsMerged { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsMergedDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fusionner les cellules A1 à B2
            worksheet.Cells.Merge(0, 0, 2, 2);

            // Vérifier si la cellule A1 est fusionnée
            bool isMerged = worksheet.Cells["A1"].IsMerged;
            Console.WriteLine("Is cell A1 merged? " + isMerged);

            // Vérifier si la cellule C1 est fusionnée (devrait être faux)
            isMerged = worksheet.Cells["C1"].IsMerged;
            Console.WriteLine("Is cell C1 merged? " + isMerged);

            // Enregistrez le classeur
            workbook.Save("MergedCellsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


