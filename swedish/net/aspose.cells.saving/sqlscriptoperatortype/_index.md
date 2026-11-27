---
title: "Enum SqlScriptOperatorType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Saving.SqlScriptOperatorType enum. Representerar typen av operativ data"
type: docs
url: /sv/net/aspose.cells.saving/sqlscriptoperatortype/
---
## SqlScriptOperatorType enumeration

Representerar typen av driftsdata.

```csharp
public enum SqlScriptOperatorType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Insert | `0` | Infoga data. |
| Update | `1` | Uppdatera data. |
| Delete | `2` | Radera data. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);

            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["B2"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue("Charlie");

            // Skapa SqlScriptSaveOptions och ställ in egenskaper
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

            // Spara arbetsboken som SQL-skript
            workbook.Save("SqlScriptOperatorTypeExample.sql", saveOptions);

            // Skriv ut resultaten
            Console.WriteLine("SQL script has been saved successfully.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


