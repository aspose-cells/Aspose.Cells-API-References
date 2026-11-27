---
title: "SqlScriptSaveOptions.CreateTable"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SqlScriptSaveOptions egenskap. Anger om export av SQL för att skapa tabell"
type: docs
url: /sv/net/aspose.cells.saving/sqlscriptsaveoptions/createtable/
---
## SqlScriptSaveOptions.CreateTable property

Indikerar om sql för att skapa tabell exporteras.

```csharp
public bool CreateTable { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyCreateTableDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Jane");

            // Konfigurera SQL-exportalternativ med CreateTable aktiverat
            SqlScriptSaveOptions options = new SqlScriptSaveOptions
            {
                CreateTable = true,
                TableName = "Employees",
                HasHeaderRow = true
            };

            // Spara som SQL-skript
            workbook.Save("output.sql", options);
        }
    }
}
```

### Se även

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


