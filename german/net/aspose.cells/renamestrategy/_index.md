---
title: "Enum RenameStrategy"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.RenameStrategy-Enum. Strategieoption für doppelte Spaltennamen"
type: docs
url: /de/net/aspose.cells/renamestrategy/
---
## RenameStrategy enumeration

Strategieoption für doppelte Spaltennamen.

```csharp
public enum RenameStrategy
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Exception | `0` | Wirft eine Ausnahme. |
| Digit | `1` | Benannt mit Ziffer. Doppelte Namen werden zu ...1, ...2 usw. |
| Letter | `2` | Benannt mit Buchstabe. Doppelte Namen werden zu ...A, ...B usw. |

### Hinweise

Beim Verarbeiten von Daten mit Kopfzeilen erfordern einige Szenarien, dass die Kopfzeilen für alle Spalten keine Duplikate aufweisen. Zum Beispiel ist beim Exportieren von Daten in ein DataTable die Kopfzeile als Spaltenname des DataTable erforderlich, sodass doppelte Werte der Kopfzeile ungültig sind. In solchen Situationen kann der Benutzer festlegen, wie damit umgegangen werden soll, indem er diese Strategie angibt.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RenameStrategyDemo
    {
        public static void RenameStrategyExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Beispieldaten zum Arbeitsblatt hinzu
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("John");

            // Erstellen Sie ExportTableOptions und setzen Sie die RenameStrategy.
            ExportTableOptions options = new ExportTableOptions
            {
                RenameStrategy = RenameStrategy.Digit // Use the Digit strategy for duplicate names
            };

            // Exportieren Sie die Arbeitsblattdaten in ein DataTable.
            System.Data.DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 4, 1, options);

            // Zeigen Sie den Inhalt des DataTable an.
            foreach (System.Data.DataRow row in dataTable.Rows)
            {
                foreach (var item in row.ItemArray)
                {
                    Console.Write(item + "\t");
                }
                Console.WriteLine();
            }

            // Speichere die Arbeitsmappe
            workbook.Save("RenameStrategyExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


