---
title: "SqlScriptSaveOptions.SqlScriptSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SqlScriptSaveOptions-konstruktör. Skapar alternativ för att spara sql-fil"
type: docs
url: /sv/net/aspose.cells.saving/sqlscriptsaveoptions/sqlscriptsaveoptions/
---
## SqlScriptSaveOptions constructor

Skapar alternativ för att spara sql‑fil.

```csharp
public SqlScriptSaveOptions()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");

            // Skapa SqlScriptSaveOptions med konstruktör
            SqlScriptSaveOptions options = new SqlScriptSaveOptions();
            options.OperatorType = SqlScriptOperatorType.Insert;
            options.AddBlankLineBetweenRows = true;

            // Spara som SQL-skript
            workbook.Save("output.sql", options);
            
            // Skriv ut den genererade SQL
            Console.WriteLine("Generated SQL Script:");
            Console.WriteLine(System.IO.File.ReadAllText("output.sql"));
        }
    }
}
```

### Se även

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


