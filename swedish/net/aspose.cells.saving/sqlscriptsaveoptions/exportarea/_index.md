---
title: "SqlScriptSaveOptions.ExportArea"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SqlScriptSaveOptions egenskap. Hämtar eller anger exportintervallet"
type: docs
url: /sv/net/aspose.cells.saving/sqlscriptsaveoptions/exportarea/
---
## SqlScriptSaveOptions.ExportArea property

Hämtar eller anger exportintervallet.

```csharp
public CellArea ExportArea { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyExportAreaDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll kalkylbladet med exempeldata
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Jane");

            // Konfigurera SQL-exportalternativ med ExportArea
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                TableName = "Employees",
                ExportArea = new CellArea { StartRow = 0, EndRow = 3, StartColumn = 0, EndColumn = 1 },
                HasHeaderRow = true
            };

            // Spara med angivet exportområde (kolumner A1:B3)
            workbook.Save("EmployeesExport.sql", saveOptions);
        }
    }
}
```

### Se även

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


