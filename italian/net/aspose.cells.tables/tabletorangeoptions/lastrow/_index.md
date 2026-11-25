---
title: "TableToRangeOptions.LastRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TableToRangeOptions. Ottiene e imposta l'indice dell'ultima riga della tabella"
type: docs
url: /it/net/aspose.cells.tables/tabletorangeoptions/lastrow/
---
## TableToRangeOptions.LastRow property

Ottiene e imposta l'indice dell'ultima riga della tabella.

```csharp
public int LastRow { get; set; }
```

### Esempi

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

            // Crea dati di esempio
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    cells[row, col].PutValue($"Data {row}-{col}");
                }
            }

            // Crea tabella
            int tableIndex = worksheet.ListObjects.Add(0, 0, 9, 4, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.TableStyleType = Aspose.Cells.Tables.TableStyleType.TableStyleMedium2;

            // Converti la tabella in intervallo con LastRow specificato
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

### Vedi anche

* class [TableToRangeOptions](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


