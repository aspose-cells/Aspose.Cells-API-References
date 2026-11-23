---
title: "Worksheet.SelectRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Worksheet. Sélectionne une plage"
type: docs
url: /fr/net/aspose.cells/worksheet/selectrange/
---
## Worksheet.SelectRange method

Sélectionne une plage.

```csharp
public void SelectRange(int startRow, int startColumn, int totalRows, int totalColumns, 
    bool removeOthers)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | Int32 | La ligne de départ. |
| startColumn | Int32 | La colonne de départ |
| totalRows | Int32 | Le nombre de lignes. |
| totalColumns | Int32 | Le nombre de colonnes |
| removeOthers | Boolean | True signifie que les autres plages sélectionnées sont supprimées et que seule cette plage est sélectionnée. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodSelectRangeWithInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Sélectionner la plage de la ligne 1, colonne 1 à la ligne 5, colonne 5 (B2:F6) et la rendre active
            worksheet.SelectRange(1, 1, 5, 5, true);
            
            Console.WriteLine("Active cell: " + worksheet.ActiveCell);
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


