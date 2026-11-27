---
title: "SqlScriptSaveOptions.OperatorType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SqlScriptSaveOptions egenskap. Hämtar och anger operatortypen för SQL"
type: docs
url: /sv/net/aspose.cells.saving/sqlscriptsaveoptions/operatortype/
---
## SqlScriptSaveOptions.OperatorType property

Hämtar och anger operator‑typen för sql.

```csharp
public SqlScriptOperatorType OperatorType { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyOperatorTypeDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok med testdata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Id");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Jane");

            // Konfigurera SQL-sparalternativ
            SqlScriptSaveOptions options = new SqlScriptSaveOptions();
            options.OperatorType = SqlScriptOperatorType.Delete;
            options.IdName = "Id";
            options.Separator = '\n';
            options.AddBlankLineBetweenRows = true;
            options.CreateTable = true;

            // Spara till minnesström och hämta SQL-skript som sträng
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, options);
                stream.Position = 0;
                using (StreamReader reader = new StreamReader(stream))
                {
                    string sqlScript = reader.ReadToEnd();
                    
                    // Skriv ut den genererade SQL
                    Console.WriteLine("Generated SQL Script:");
                    Console.WriteLine(sqlScript);
                }
            }
        }
    }
}
```

### Se även

* enum [SqlScriptOperatorType](../../sqlscriptoperatortype/)
* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


