---
title: "Klasse TableToRangeOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Tables.TableToRangeOptions Klasse. Stellt die Optionen beim Konvertieren einer Tabelle in einen Bereich dar"
type: docs
url: /de/net/aspose.cells.tables/tabletorangeoptions/
---
## TableToRangeOptions class

Stellt die Optionen beim Konvertieren einer Tabelle in einen Bereich dar.

```csharp
public class TableToRangeOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [TableToRangeOptions](tabletorangeoptions/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [LastRow](../../aspose.cells.tables/tabletorangeoptions/lastrow/) { get; set; } | Liest und setzt den Index der letzten Zeile der Tabelle. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Fülle das Arbeitsblatt mit einigen Daten
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

            // Füge ein ListObject (Tabelle) zum Arbeitsblatt hinzu
            ListObjectCollection tables = worksheet.ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Setzt einige Eigenschaften der Tabelle
            table.ShowTotals = true;
            table.ListColumns[4].TotalsCalculation = TotalsCalculation.Sum;

            // Erstelle eine Instanz von TableToRangeOptions
            TableToRangeOptions options = new TableToRangeOptions
            {
                LastRow = 9 // Set the last row index of the table
            };

            // Konvertiere die Tabelle mithilfe der Optionen in einen Bereich
            table.ConvertToRange(options);

            // Speichere die Arbeitsmappe
            workbook.Save("TableToRangeOptionsExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


