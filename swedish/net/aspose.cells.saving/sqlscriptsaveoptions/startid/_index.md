---
title: "SqlScriptSaveOptions.StartId"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SqlScriptSaveOptions egenskap. Hämtar och anger start‑id"
type: docs
url: /sv/net/aspose.cells.saving/sqlscriptsaveoptions/startid/
---
## SqlScriptSaveOptions.StartId property

Hämtar och anger start‑id.

```csharp
public int StartId { get; set; }
```

### Anmärkningar

Fungerar endast när [`IdName`](../idname/) är inställt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyStartIdDemo
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

            // Konfigurera SQL-exportalternativ med StartId satt till 100
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                TableName = "Employees",
                IdName = "ID",
                StartId = 100, // Demonstrating StartId property
                HasHeaderRow = true,
                OperatorType = SqlScriptOperatorType.Insert
            };

            // Spara som SQL-skript
            workbook.Save("Employees_WithStartId.sql", saveOptions);
        }
    }
}
```

### Se även

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


