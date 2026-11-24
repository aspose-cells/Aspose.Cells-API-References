---
title: "TableToRangeOptions.LastRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TableToRangeOptions-Eigenschaft. Liest und schreibt den Index der letzten Zeile der Tabelle"
type: docs
url: /de/net/aspose.cells.tables/tabletorangeoptions/lastrow/
---
## TableToRangeOptions.LastRow property

Liest und setzt den Index der letzten Zeile der Tabelle.

```csharp
public int LastRow { get; set; }
```

### Beispiele

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

            // Erstelle Beispieldaten
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    cells[row, col].PutValue($"Data {row}-{col}");
                }
            }

            // Tabelle erstellen
            int tableIndex = worksheet.ListObjects.Add(0, 0, 9, 4, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.TableStyleType = Aspose.Cells.Tables.TableStyleType.TableStyleMedium2;

            // Tabelle in Bereich konvertieren mit angegebenem LastRow
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

### Siehe auch

* class [TableToRangeOptions](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


