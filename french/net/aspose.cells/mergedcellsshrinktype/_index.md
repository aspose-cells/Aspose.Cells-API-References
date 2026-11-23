---
title: "Enum MergedCellsShrinkType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.MergedCellsShrinkType enum. Représente la stratégie de réduction des cellules fusionnées pour des opérations telles que la suppression de lignes/colonnes vides."
type: docs
url: /fr/net/aspose.cells/mergedcellsshrinktype/
---
## MergedCellsShrinkType enumeration

Représente la stratégie de réduction des cellules fusionnées pour des opérations telles que la suppression de lignes/colonnes vides.

```csharp
public enum MergedCellsShrinkType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Laisse les cellules fusionnées telles quelles, sans aucune modification. |
| ShrinkToFit | `1` | Réduit la zone fusionnée si nécessaire, en supprimant les lignes du bas ou les colonnes de droite, tout en veillant à ce que tout le contenu reste visible. |
| KeepHeaderOnly | `2` | Ne conserve que les lignes/colonnes d'en-tête de la zone fusionnée lorsque la cellule supérieure gauche de la zone fusionnée n'est pas vide. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassMergedCellsShrinkTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            Cells cells = ws.Cells;

            // Initialiser des données d'exemple avec des cellules fusionnées
            cells.Merge(0, 0, 1, 2);
            cells[0, 0].PutValue("Merged Header");
            cells[1, 2].PutValue("Data 1");
            cells[2, 2].PutValue("Data 2");

            Console.WriteLine("Original worksheet:");
            PrintCellValues(cells);

            // Option 1 : KeepHeaderOnly
            DeleteBlankOptions opts1 = new DeleteBlankOptions();
            opts1.MergedCellsShrinkType = MergedCellsShrinkType.KeepHeaderOnly;
            cells.DeleteBlankColumns(opts1);
            Console.WriteLine("\nAfter DeleteBlankColumns with KeepHeaderOnly:");
            PrintCellValues(cells);

            // Réinitialiser la feuille de calcul
            cells.ClearContents(0, 0, cells.MaxDataRow, cells.MaxDataColumn);
            cells.Merge(0, 0, 1, 2);
            cells[0, 0].PutValue("Merged Header");
            cells[1, 2].PutValue("Data 1");
            cells[2, 2].PutValue("Data 2");

            // Option 2 : None
            DeleteBlankOptions opts2 = new DeleteBlankOptions();
            opts2.MergedCellsShrinkType = MergedCellsShrinkType.None;
            cells.DeleteBlankColumns(opts2);
            Console.WriteLine("\nAfter DeleteBlankColumns with None:");
            PrintCellValues(cells);

            // Réinitialiser la feuille de calcul
            cells.ClearContents(0, 0, cells.MaxDataRow, cells.MaxDataColumn);
            cells.Merge(0, 0, 1, 2);
            cells[0, 0].PutValue("Merged Header");
            cells[1, 2].PutValue("Data 1");
            cells[2, 2].PutValue("Data 2");

            // Option 3 : ShrinkToFit
            DeleteBlankOptions opts3 = new DeleteBlankOptions();
            opts3.MergedCellsShrinkType = MergedCellsShrinkType.ShrinkToFit;
            cells.DeleteBlankColumns(opts3);
            Console.WriteLine("\nAfter DeleteBlankColumns with ShrinkToFit:");
            PrintCellValues(cells);
        }

        private static void PrintCellValues(Cells cells)
        {
            for (int row = 0; row < 3; row++)
            {
                for (int col = 0; col < 3; col++)
                {
                    Console.Write($"({row},{col}): {cells[row, col].Value ?? "empty"} | ");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


