---
title: "Cells.IsDeletingRangeEnabled"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Vérifiez si la plage peut être supprimée"
type: docs
url: /fr/net/aspose.cells/cells/isdeletingrangeenabled/
---
## Cells.IsDeletingRangeEnabled method

Vérifie si la plage peut être supprimée.

```csharp
public bool IsDeletingRangeEnabled(int startRow, int startColumn, int totalRows, int totalColumns)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | Int32 | L'index de ligne de départ de la plage. |
| startColumn | Int32 | L'index de colonne de départ de la plage. |
| totalRows | Int32 | Le nombre de lignes dans la plage. |
| totalColumns | Int32 | Le nombre de colonnes dans la plage. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodIsDeletingRangeEnabledWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Remplir les cellules A1:C5 avec des données d'exemple
            for (int row = 0; row < 5; row++)
            {
                for (int col = 0; col < 3; col++)
                {
                    cells[row, col].Value = $"Data{row}_{col}";
                }
            }

            try
            {
                // Vérifiez si la suppression de 5 lignes x 3 colonnes à partir de A1 est activée
                bool canDelete = cells.IsDeletingRangeEnabled(0, 0, 5, 3);
                Console.WriteLine($"Can delete range: {canDelete}");

                if (canDelete)
                {
                    // Supprimez la plage A1:C5 et déplacez les cellules vers le haut
                    cells.DeleteRange(0, 0, 4, 2, ShiftType.Up);
                    Console.WriteLine("Deleted range A1:C5 successfully");
                }

                workbook.Save("IsDeletingRangeEnabledOutput.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during range deletion: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


