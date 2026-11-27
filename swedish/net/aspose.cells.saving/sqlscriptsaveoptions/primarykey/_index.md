---
title: "SqlScriptSaveOptions.PrimaryKey"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SqlScriptSaveOptions egenskap. Representerar vilken kolumn som är primärnyckel i datatabellen"
type: docs
url: /sv/net/aspose.cells.saving/sqlscriptsaveoptions/primarykey/
---
## SqlScriptSaveOptions.PrimaryKey property

Representerar vilken kolumn som är primärnyckel i datatabellen.

```csharp
public int PrimaryKey { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyPrimaryKeyDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["B2"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue("Bob");

            // Konfigurera SQL-exportalternativ med PrimaryKey satt till första kolumnen (0)
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                PrimaryKey = 0,
                TableName = "Employees",
                CreateTable = true,
                HasHeaderRow = true
            };

            // Spara som SQL-skript
            workbook.Save("EmployeesExport.sql", saveOptions);

            Console.WriteLine("SQL script exported with PrimaryKey set to column 0 (ID)");
        }
    }
}
```

### Se även

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


