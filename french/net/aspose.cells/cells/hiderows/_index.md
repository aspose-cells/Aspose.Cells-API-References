---
title: "Cells.HideRows"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Masque plusieurs lignes"
type: docs
url: /fr/net/aspose.cells/cells/hiderows/
---
## Cells.HideRows method

Masque plusieurs lignes.

```csharp
public void HideRows(int row, int totalRows)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | L'index de ligne. |
| totalRows | Int32 | Le numéro de ligne. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplissez quelques données
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].Value = $"Row {i+1}, Col {j+1}";
                }
            }

            // Masquer les lignes 3 à 5 (index basé sur zéro : 2 à 4)
            worksheet.Cells.HideRows(2, 3);

            // Enregistrez le classeur
            workbook.Save("HideRowsExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


