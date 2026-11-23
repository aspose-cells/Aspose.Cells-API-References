---
title: "Classe TableToRangeOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Tables.TableToRangeOptions. Représente les options lors de la conversion d'un tableau en plage"
type: docs
url: /fr/net/aspose.cells.tables/tabletorangeoptions/
---
## TableToRangeOptions class

Représente les options lors de la conversion d'une table en plage.

```csharp
public class TableToRangeOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [TableToRangeOptions](tabletorangeoptions/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [LastRow](../../aspose.cells.tables/tabletorangeoptions/lastrow/) { get; set; } | Obtient et définit l'index de la dernière ligne du tableau. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableToRangeOptionsDemo
    {
        public static void TableToRangeOptionsExample()
        {
            // Créer un nouveau classeur
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
                for (int column = 0; column < 5; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Ajoutez un ListObject (table) à la feuille de calcul
            ListObjectCollection tables = worksheet.ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Définissez certaines propriétés du tableau
            table.ShowTotals = true;
            table.ListColumns[4].TotalsCalculation = TotalsCalculation.Sum;

            // Créez une instance de TableToRangeOptions
            TableToRangeOptions options = new TableToRangeOptions
            {
                LastRow = 9 // Set the last row index of the table
            };

            // Convertissez le tableau en plage en utilisant les options
            table.ConvertToRange(options);

            // Enregistrez le classeur
            workbook.Save("TableToRangeOptionsExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


