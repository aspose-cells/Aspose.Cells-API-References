---
title: "SqlScriptColumnTypeMap.GetStringType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SqlScriptColumnTypeMap‑metod. Hämtar strängtyp i databasen"
type: docs
url: /sv/net/aspose.cells.saving/sqlscriptcolumntypemap/getstringtype/
---
## SqlScriptColumnTypeMap.GetStringType method

Hämtar strängtyp i databasen.

```csharp
public virtual string GetStringType()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptColumnTypeMapMethodGetStringTypeDemo
    {
        public static void Run()
        {
            // Skapa en instans av SqlScriptColumnTypeMap
            SqlScriptColumnTypeMap columnTypeMap = new SqlScriptColumnTypeMap();

            // Hämta och visa standardsträngtypen
            string stringType = columnTypeMap.GetStringType();
            Console.WriteLine("Default String Type: " + stringType);

            // Skapa en enkel arbetsbok med strängdata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John Doe");

            // Spara med SQL‑skriptalternativ med hjälp av typmappningen
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                ColumnTypeMap = columnTypeMap
            };
            
            workbook.Save("SqlScriptOutput.sql", saveOptions);
            Console.WriteLine("SQL script saved with string type: " + stringType);
        }
    }
}
```

### Se även

* class [SqlScriptColumnTypeMap](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


