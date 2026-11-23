---
title: "Cells.GetGroupedRowOutlineLevel"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Obtient le niveau de contour (zéro‑indexé) de la ligne"
type: docs
url: /fr/net/aspose.cells/cells/getgroupedrowoutlinelevel/
---
## Cells.GetGroupedRowOutlineLevel method

Obtient le niveau de contour (à base zéro) de la ligne.

```csharp
public int GetGroupedRowOutlineLevel(int rowIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | L'index de ligne. |

### Valeur de retour

Le niveau de contour (zéro‑indexé) de la ligne.

### Remarques

Si la ligne n’est pas groupée, renvoie zéro.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetGroupedRowOutlineLevelWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Grouper les lignes 0-3 (niveau 1)
            cells.GroupRows(0, 3, false);
            
            // Grouper les lignes 0-1 (niveau 2)
            cells.GroupRows(0, 1, false);

            // Obtenir le niveau de contour pour chaque ligne
            for (int row = 0; row <= 4; row++)
            {
                int outlineLevel = cells.GetGroupedRowOutlineLevel(row);
                Console.WriteLine($"Row {row} outline level: {outlineLevel}");
            }

            // Dégrouper toutes les lignes
            cells.UngroupRows(0, 3);
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


