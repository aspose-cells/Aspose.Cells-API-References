---
title: "Cells.IsDefaultRowHeightMatched"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cells. Indique que la hauteur de ligne et la hauteur de police par défaut correspondent"
type: docs
url: /fr/net/aspose.cells/cells/isdefaultrowheightmatched/
---
## Cells.IsDefaultRowHeightMatched property

Indique que la hauteur de ligne et la hauteur de police par défaut correspondent.

```csharp
public bool IsDefaultRowHeightMatched { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyIsDefaultRowHeightMatchedDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Définir et démontrer la propriété IsDefaultRowHeightMatched
            cells.IsDefaultRowHeightMatched = true;
            Console.WriteLine("IsDefaultRowHeightMatched: " + cells.IsDefaultRowHeightMatched);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");

            // Chargez le classeur enregistré pour vérifier la propriété
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Cells loadedCells = loadedWorkbook.Worksheets[0].Cells;
            Console.WriteLine("Loaded IsDefaultRowHeightMatched: " + loadedCells.IsDefaultRowHeightMatched);
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


