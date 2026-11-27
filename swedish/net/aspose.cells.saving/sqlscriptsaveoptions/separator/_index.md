---
title: "SqlScriptSaveOptions.Separator"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SqlScriptSaveOptions egenskap. Hämtar och anger teckenseparator för sql-skript"
type: docs
url: /sv/net/aspose.cells.saving/sqlscriptsaveoptions/separator/
---
## SqlScriptSaveOptions.Separator property

Hämtar och anger teckenseparatorn för sql‑skriptet.

```csharp
public char Separator { get; set; }
```

### Anmärkningar

Kan endast vara ' ' eller '\n'. Om

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertySeparatorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["B2"].PutValue("John");

            // Konfigurera SQL-sparalternativ med anpassad separator
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                Separator = ';',
                TableName = "Employees",
                CreateTable = true,
                HasHeaderRow = true
            };

            // Spara med anpassad separator
            workbook.Save("SqlScriptWithSeparator.sql", saveOptions);

            Console.WriteLine("SQL script saved with custom separator.");
        }
    }
}
```

### Se även

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


