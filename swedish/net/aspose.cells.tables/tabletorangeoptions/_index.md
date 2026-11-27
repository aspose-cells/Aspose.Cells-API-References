---
title: "Klass TableToRangeOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Tables.TableToRangeOptions-klass. Representerar alternativen när en tabell konverteras till ett område"
type: docs
url: /sv/net/aspose.cells.tables/tabletorangeoptions/
---
## TableToRangeOptions class

Representerar alternativen när tabell konverteras till ett område.

```csharp
public class TableToRangeOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [TableToRangeOptions](tabletorangeoptions/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [LastRow](../../aspose.cells.tables/tabletorangeoptions/lastrow/) { get; set; } | Hämtar och anger det sista radindexet för tabellen. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Fyll i arbetsbladet med några data
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

            // Lägg till ett ListObject (tabell) i kalkylbladet
            ListObjectCollection tables = worksheet.ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Ställ in några egenskaper för tabellen
            table.ShowTotals = true;
            table.ListColumns[4].TotalsCalculation = TotalsCalculation.Sum;

            // Skapa en instans av TableToRangeOptions
            TableToRangeOptions options = new TableToRangeOptions
            {
                LastRow = 9 // Set the last row index of the table
            };

            // Konvertera tabellen till ett område med hjälp av alternativen
            table.ConvertToRange(options);

            // Spara arbetsboken
            workbook.Save("TableToRangeOptionsExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


