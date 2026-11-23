---
title: "TableToRangeOptions.LastRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TableToRangeOptions. Obtient et définit l'index de la dernière ligne du tableau"
type: docs
url: /fr/net/aspose.cells.tables/tabletorangeoptions/lastrow/
---
## TableToRangeOptions.LastRow property

Obtient et définit l'index de la dernière ligne du tableau.

```csharp
public int LastRow { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableToRangeOptionsPropertyLastRowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Créer des données d'exemple
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    cells[row, col].PutValue($"Data {row}-{col}");
                }
            }

            // Créez un tableau
            int tableIndex = worksheet.ListObjects.Add(0, 0, 9, 4, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.TableStyleType = Aspose.Cells.Tables.TableStyleType.TableStyleMedium2;

            // Convertir le tableau en plage avec LastRow spécifié
            TableToRangeOptions options = new TableToRangeOptions
            {
                LastRow = 7 // Only convert rows 0-7 (excluding 8-9)
            };
            table.ConvertToRange(options);

            workbook.Save("TableToRangeWithLastRow.xlsx");
        }
    }
}
```

### Voir aussi

* class [TableToRangeOptions](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


