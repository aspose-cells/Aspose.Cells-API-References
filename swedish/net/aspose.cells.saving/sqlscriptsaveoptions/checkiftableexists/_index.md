---
title: "SqlScriptSaveOptions.CheckIfTableExists"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SqlScriptSaveOptions-egenskap. Kontrollera om tabellnamnet finns innan det skapas"
type: docs
url: /sv/net/aspose.cells.saving/sqlscriptsaveoptions/checkiftableexists/
---
## SqlScriptSaveOptions.CheckIfTableExists property

Kontrollera om tabellnamnet finns innan det skapas

```csharp
public bool CheckIfTableExists { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyCheckIfTableExistsDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok med testdata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Jane");

            // Konfigurera SQL-sparalternativ
            SqlScriptSaveOptions sqlOptions = new SqlScriptSaveOptions();
            sqlOptions.CreateTable = true;
            sqlOptions.CheckIfTableExists = true;
            sqlOptions.OperatorType = SqlScriptOperatorType.Insert;

            // Spara till SQL-skriptfil
            workbook.Save("output.sql", sqlOptions);

            // Läs och skriv ut den genererade SQL-koden
            string sqlScript = System.IO.File.ReadAllText("output.sql");
            Console.WriteLine("Generated SQL Script:");
            Console.WriteLine(sqlScript);
        }
    }
}
```

### Se även

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


