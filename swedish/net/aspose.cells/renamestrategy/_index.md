---
title: "Enum RenameStrategy"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.RenameStrategy enum. Strategialternativ för duplicerade kolumnnamn"
type: docs
url: /sv/net/aspose.cells/renamestrategy/
---
## RenameStrategy enumeration

Strategialternativ för dubblettnamn på kolumner.

```csharp
public enum RenameStrategy
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Exception | `0` | Kastar undantag. |
| Digit | `1` | Namngiven med siffra. Duplicerade namn blir ...1, ...2 osv. |
| Letter | `2` | Namngiven med bokstav.. Duplicerade namn blir ...A, ...B osv. |

### Anmärkningar

När data med rubriker bearbetas kräver vissa scenarier att rubrikerna inte dupliceras för någon kolumn. Till exempel, när data exporteras till en datatabell och rubriken måste användas som datatabellens kolumnnamn, är duplicerade rubrikvärden ogiltiga. I sådana situationer kan användaren bestämma hur de ska hanteras genom att ange denna strategi.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RenameStrategyDemo
    {
        public static void RenameStrategyExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("John");

            // Skapa ExportTableOptions och ange RenameStrategy
            ExportTableOptions options = new ExportTableOptions
            {
                RenameStrategy = RenameStrategy.Digit // Use the Digit strategy for duplicate names
            };

            // Exportera arbetsbladets data till en DataTable
            System.Data.DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 4, 1, options);

            // Visa DataTable-innehållet
            foreach (System.Data.DataRow row in dataTable.Rows)
            {
                foreach (var item in row.ItemArray)
                {
                    Console.Write(item + "\t");
                }
                Console.WriteLine();
            }

            // Spara arbetsboken
            workbook.Save("RenameStrategyExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


