---
title: "SqlScriptSaveOptions.IdName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SqlScriptSaveOptions egenskap. Hämtar och anger namnet på id-kolumnen"
type: docs
url: /sv/net/aspose.cells.saving/sqlscriptsaveoptions/idname/
---
## SqlScriptSaveOptions.IdName property

Hämtar och anger namnet på id‑kolumnen.

```csharp
public string IdName { get; set; }
```

### Anmärkningar

Om denna egenskap är inställd, kommer en kolumn att infogas med automatiskt ökande heltalsvärde.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyIdNameDemo
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

            // Konfigurera SQL-exportalternativ med IdName
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                TableName = "Employees",
                IdName = "ID",
                CreateTable = true,
                HasHeaderRow = true
            };

            // Spara som SQL-skript
            workbook.Save("Employees.sql", saveOptions);

            Console.WriteLine("SQL script exported with IdName property");
        }
    }
}
```

### Se även

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


