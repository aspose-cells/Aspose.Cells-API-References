---
title: "Aufzählung SqlScriptOperatorType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Saving.SqlScriptOperatorType enum. Stellt den Typ der Betriebsdaten dar."
type: docs
url: /de/net/aspose.cells.saving/sqlscriptoperatortype/
---
## SqlScriptOperatorType enumeration

Stellt den Typ der Betriebsdaten dar.

```csharp
public enum SqlScriptOperatorType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Insert | `0` | Daten einfügen. |
| Update | `1` | Daten aktualisieren. |
| Delete | `2` | Daten löschen. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class SqlScriptOperatorTypeDemo
    {
        public static void SqlScriptOperatorTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);

            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["B2"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue("Charlie");

            // Erstelle SqlScriptSaveOptions und setze Eigenschaften
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                CheckIfTableExists = true,
                AddBlankLineBetweenRows = true,
                Separator = ';',
                OperatorType = SqlScriptOperatorType.Insert,
                PrimaryKey = 0,
                CreateTable = true,
                IdName = "ID",
                StartId = 1,
                TableName = "SampleTable",
                ExportAsString = false,
                ExportArea = new CellArea { StartRow = 1, StartColumn = 0, EndRow = 3, EndColumn = 1 },
                HasHeaderRow = true
            };

            // Speichere die Arbeitsmappe als SQL‑Skript
            workbook.Save("SqlScriptOperatorTypeExample.sql", saveOptions);

            // Ergebnisse ausgeben
            Console.WriteLine("SQL script has been saved successfully.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


