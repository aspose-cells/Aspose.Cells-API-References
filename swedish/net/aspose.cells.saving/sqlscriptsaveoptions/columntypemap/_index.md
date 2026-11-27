---
title: "SqlScriptSaveOptions.ColumnTypeMap"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SqlScriptSaveOptions-egenskap. Hämtar och anger mappningen av kolumntyp för olika databaser"
type: docs
url: /sv/net/aspose.cells.saving/sqlscriptsaveoptions/columntypemap/
---
## SqlScriptSaveOptions.ColumnTypeMap property

Hämtar och anger mappningen av kolumntyp för olika databaser.

```csharp
public SqlScriptColumnTypeMap ColumnTypeMap { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyColumnTypeMapDemo
    {
        public static void Run()
        {
            // Skapa en anpassad kolumntypmappning
            SqlScriptColumnTypeMap customTypeMap = new SqlScriptColumnTypeMap();
            
            // Skapa SQL-sparalternativ
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                TableName = "Employees",
                CreateTable = true,
                ColumnTypeMap = customTypeMap,
                CheckIfTableExists = true,
                ExportAsString = false
            };

            // Skapa en exempelarbetsbok med data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till rubriker
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["C1"].PutValue("Salary");
            
            // Lägg till datarader
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John Smith");
            worksheet.Cells["C2"].PutValue(5000.50);
            
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Jane Doe");
            worksheet.Cells["C3"].PutValue(6500.75);

            // Spara som SQL-skript
            workbook.Save("EmployeeData.sql", saveOptions);
            
            Console.WriteLine("SQL script generated successfully with custom column type mapping.");
        }
    }
}
```

### Se även

* class [SqlScriptColumnTypeMap](../../sqlscriptcolumntypemap/)
* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


