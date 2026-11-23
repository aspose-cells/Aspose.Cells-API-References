---
title: "Classe ListColumn"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Tables.ListColumn. Représente une colonne dans un tableau"
type: docs
url: /fr/net/aspose.cells.tables/listcolumn/
---
## ListColumn class

Représente une colonne dans une Table.

```csharp
public class ListColumn
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Formula](../../aspose.cells.tables/listcolumn/formula/) { get; set; } | Obtient et définit la formule de la colonne de liste. |
| [IsArrayFormula](../../aspose.cells.tables/listcolumn/isarrayformula/) { get; } | Indique si la formule est une formule matricielle. |
| [Name](../../aspose.cells.tables/listcolumn/name/) { get; set; } | Obtient et définit le nom de la colonne. |
| [Range](../../aspose.cells.tables/listcolumn/range/) { get; } | Obtient la plage de cette colonne de liste. |
| [TotalsCalculation](../../aspose.cells.tables/listcolumn/totalscalculation/) { get; set; } | Obtient et définit le type de calcul dans la ligne Totaux de la colonne de liste. |
| [TotalsRowLabel](../../aspose.cells.tables/listcolumn/totalsrowlabel/) { get; set; } | Obtient et définit les libellés d’affichage de la ligne de total. |

## Méthodes

| Nom | Description |
| --- | --- |
| [GetCustomCalculatedFormula](../../aspose.cells.tables/listcolumn/getcustomcalculatedformula/)(bool, bool) | Obtient la formule de cette colonne de liste. |
| [GetCustomTotalsRowFormula](../../aspose.cells.tables/listcolumn/getcustomtotalsrowformula/)(bool, bool) | Obtient la formule de la ligne de totaux de cette colonne de liste. |
| [GetDataStyle](../../aspose.cells.tables/listcolumn/getdatastyle/)() | Obtient le style des données dans cette colonne du tableau. |
| [SetCustomCalculatedFormula](../../aspose.cells.tables/listcolumn/setcustomcalculatedformula/)(string, bool, bool) | Définit la formule pour cette colonne de liste. |
| [SetCustomTotalsRowFormula](../../aspose.cells.tables/listcolumn/setcustomtotalsrowformula/)(string, bool, bool) | Obtient la formule de la ligne de totaux de cette colonne de liste. |
| [SetDataStyle](../../aspose.cells.tables/listcolumn/setdatastyle/)(Style) | Définit le style des données dans cette colonne du tableau. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListColumnDemo
    {
        public static void ListColumnExample()
        {
            // Créer un nouveau classeur et accéder à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

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

            // Ajoutez un ListObject (table) à la feuille de calcul
            ListObjectCollection tables = worksheet.ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];
            table.ShowTotals = true;

            // Accédez à la ListColumn et définissez ses propriétés
            ListColumn listColumn = table.ListColumns[4];
            listColumn.TotalsCalculation = TotalsCalculation.Sum;
            listColumn.Formula = "=[A]";
            listColumn.Name = "CustomColumn";
            listColumn.TotalsRowLabel = "Total";

            // Enregistrez le classeur
            workbook.Save("ListColumnExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


