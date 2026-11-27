---
title: "SqlScriptSaveOptions.HasHeaderRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SqlScriptSaveOptions egenskap. Anger om intervallet innehåller en rubrikrad"
type: docs
url: /sv/net/aspose.cells.saving/sqlscriptsaveoptions/hasheaderrow/
---
## SqlScriptSaveOptions.HasHeaderRow property

Anger om intervallet innehåller en rubrikrad.

```csharp
public bool HasHeaderRow { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyHasHeaderRowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till rubrikrad och exempeldata
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Alice");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Bob");

            // Konfigurera SQL-exportalternativ med HasHeaderRow=true
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                TableName = "Employees",
                HasHeaderRow = true,
                CreateTable = true
            };

            // Spara som SQL-skript
            workbook.Save("Employees.sql", saveOptions);

            Console.WriteLine("SQL script with header row exported successfully.");
        }
    }
}
```

### Se även

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


