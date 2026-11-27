---
title: "SqlScriptSaveOptions.ExportAsString"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SqlScriptSaveOptions egenskap. Anger om all data exporteras som strängvärde"
type: docs
url: /sv/net/aspose.cells.saving/sqlscriptsaveoptions/exportasstring/
---
## SqlScriptSaveOptions.ExportAsString property

Indikerar om all data exporteras som strängvärde.

```csharp
public bool ExportAsString { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyExportAsStringDemo
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

            // Konfigurera SQL-exportalternativ
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                TableName = "Employees",
                ExportAsString = true, // Demonstrating ExportAsString property
                HasHeaderRow = true
            };

            // Spara med strängexport aktiverad
            workbook.Save("ExportAsString_True.sql", saveOptions);

            // Ändra till false och spara igen
            saveOptions.ExportAsString = false;
            workbook.Save("ExportAsString_False.sql", saveOptions);

            Console.WriteLine("SQL scripts saved with different ExportAsString settings.");
        }
    }
}
```

### Se även

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


