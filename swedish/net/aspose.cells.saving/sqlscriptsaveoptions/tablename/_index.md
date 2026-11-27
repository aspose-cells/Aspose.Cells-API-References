---
title: "SqlScriptSaveOptions.TableName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SqlScriptSaveOptions egenskap. Hämtar och anger tabellnamnet"
type: docs
url: /sv/net/aspose.cells.saving/sqlscriptsaveoptions/tablename/
---
## SqlScriptSaveOptions.TableName property

Hämtar och anger tabellnamnet.

```csharp
public string TableName { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyTableNameDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok med lite data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Konfigurera SQL‑sparalternativ med anpassat tabellnamn
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions();
            saveOptions.TableName = "Employees"; // Demonstrating TableName property
            saveOptions.CreateTable = true;
            saveOptions.OperatorType = SqlScriptOperatorType.Insert;

            // Spara som SQL-skript
            workbook.Save("output.sql", saveOptions);

            Console.WriteLine("SQL Script generated with table name 'Employees'");
        }
    }
}
```

### Se även

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


