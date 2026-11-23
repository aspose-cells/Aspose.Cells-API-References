---
title: "Cells.UnhideRows"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Dévoile les lignes masquées"
type: docs
url: /fr/net/aspose.cells/cells/unhiderows/
---
## Cells.UnhideRows method

Dévoile les lignes cachées.

```csharp
public void UnhideRows(int row, int totalRows, double height)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | L'index de ligne. |
| totalRows | Int32 | Le numéro de ligne. |
| hauteur | Double | Hauteur de la ligne. La hauteur de la ligne ne sera modifiée que lorsque la ligne est masquée et que la valeur de hauteur fournie est positive. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUnhideRowsWithInt32Int32DoubleDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Masquer les lignes 0-4
            cells.HideRows(0, 5);
            
            // Dévoiler les lignes 0-4 avec ajustement de hauteur (-1 pour ajustement automatique)
            cells.UnhideRows(0, 5, -1);
            
            // Vérifier que les lignes sont dévoilées
            for (int i = 0; i < 5; i++)
            {
                Console.WriteLine($"Row {i} hidden status: {cells.IsRowHidden(i)}");
            }
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


