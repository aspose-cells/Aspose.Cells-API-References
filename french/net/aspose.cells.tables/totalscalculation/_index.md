---
title: "Enum TotalsCalculation"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.Tables.TotalsCalculation. Détermine le type de calcul dans la ligne Totaux de la colonne de liste"
type: docs
url: /fr/net/aspose.cells.tables/totalscalculation/
---
## TotalsCalculation enumeration

Détermine le type de calcul dans la ligne Totaux de la colonne de liste.

```csharp
public enum TotalsCalculation
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Sum | `6` | Représente le calcul des totaux de somme. |
| Count | `2` | Représente le calcul des totaux de comptage. |
| Average | `1` | Représente le calcul des totaux de moyenne. |
| Max | `4` | Représente le calcul des totaux maximum. |
| Min | `5` | Représente le calcul des totaux Min. |
| Var | `8` | Représente le calcul des totaux Var. |
| CountNums | `3` | Représente le calcul des totaux Count Nums. |
| StdDev | `7` | Représente le calcul des totaux StdDev. |
| None | `0` | Représente le calcul des totaux No. |
| Custom | `9` | Représente un calcul personnalisé. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TotalsCalculationDemo
    {
        public static void TotalsCalculationExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Remplissez la feuille de calcul avec quelques données
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }
            for (int row = 1; row < 10; row++)
            {
                for (int column = 0; column < 4; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Ajoutez un tableau à la feuille de calcul
            ListObjectCollection tables = workbook.Worksheets[0].ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Afficher la ligne des totaux
            table.ShowTotals = true;

            // Accéder à la cinquième colonne du tableau
            ListColumn listColumn = table.ListColumns[4];

            // Définir la propriété TotalsCalculation sur Sum
            listColumn.TotalsCalculation = TotalsCalculation.Sum;

            // Optionnellement, définir une formule pour la colonne
            listColumn.Formula = "=[A]";

            // Enregistrez le classeur
            workbook.Save("TotalsCalculationExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


