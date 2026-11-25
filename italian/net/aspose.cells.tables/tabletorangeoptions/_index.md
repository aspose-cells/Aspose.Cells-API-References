---
title: "Classe TableToRangeOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Tables.TableToRangeOptions. Rappresenta le opzioni durante la conversione di una tabella in un intervallo"
type: docs
url: /it/net/aspose.cells.tables/tabletorangeoptions/
---
## TableToRangeOptions class

Rappresenta le opzioni durante la conversione della tabella in intervallo.

```csharp
public class TableToRangeOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [TableToRangeOptions](tabletorangeoptions/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [LastRow](../../aspose.cells.tables/tabletorangeoptions/lastrow/) { get; set; } | Ottiene e imposta l'indice dell'ultima riga della tabella. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Popola il foglio di lavoro con alcuni dati
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

            // Aggiungi un ListObject (tabella) al foglio di lavoro
            ListObjectCollection tables = worksheet.ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Imposta alcune proprietà della tabella
            table.ShowTotals = true;
            table.ListColumns[4].TotalsCalculation = TotalsCalculation.Sum;

            // Crea un'istanza di TableToRangeOptions
            TableToRangeOptions options = new TableToRangeOptions
            {
                LastRow = 9 // Set the last row index of the table
            };

            // Converti la tabella in un intervallo usando le opzioni
            table.ConvertToRange(options);

            // Salva la cartella di lavoro
            workbook.Save("TableToRangeOptionsExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


