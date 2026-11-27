---
title: "SqlScriptSaveOptions.AddBlankLineBetweenRows"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SqlScriptSaveOptions-egenskap. Infoga en tom rad mellan varje datapost"
type: docs
url: /sv/net/aspose.cells.saving/sqlscriptsaveoptions/addblanklinebetweenrows/
---
## SqlScriptSaveOptions.AddBlankLineBetweenRows property

Infoga en tom rad mellan varje data.

```csharp
public bool AddBlankLineBetweenRows { get; set; }
```

### Anmärkningar

Om [`Separator`](../separator/) är '\\n' , är det bättre att sätta denna egenskap till true för att öka läsbarheten.

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyAddBlankLineBetweenRowsDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok med testdata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Jane");

            // Konfigurera SQL-sparalternativ
            SqlScriptSaveOptions options = new SqlScriptSaveOptions
            {
                OperatorType = SqlScriptOperatorType.Insert,
                TableName = "Employees",
                IdName = "ID",
                AddBlankLineBetweenRows = true,
                CreateTable = true
            };

            // Spara till minnesström och hämta SQL-skript som sträng
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, options);
                stream.Position = 0;
                using (StreamReader reader = new StreamReader(stream))
                {
                    string sqlScript = reader.ReadToEnd();
                    Console.WriteLine("SQL script generated with blank lines between rows:");
                    Console.WriteLine(sqlScript);
                }
            }
        }
    }
}
```

### Se även

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


