---
title: "SqlScriptSaveOptions.CheckAllDataForColumnType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SqlScriptSaveOptions egenskap. Kontrollerar all data för att hitta kolumners datatyp"
type: docs
url: /sv/net/aspose.cells.saving/sqlscriptsaveoptions/checkalldataforcolumntype/
---
## SqlScriptSaveOptions.CheckAllDataForColumnType property

Kontrollera all data för att hitta kolumnernas datatyp.

```csharp
public bool CheckAllDataForColumnType { get; set; }
```

### Anmärkningar

Standardvärdet är falskt, vi kontrollerar bara den första raden för prestanda. Om denna egenskap är sann och kolumnerna innehåller blandade värdetyper, blir kolumnernas typ text.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyCheckAllDataForColumnTypeDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok med testdata
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Lägg till exempeldata med blandade typer
            sheet.Cells["A1"].PutValue("First_name");
            sheet.Cells["B1"].PutValue("Last_name");
            sheet.Cells["C1"].PutValue("age");
            sheet.Cells["D1"].PutValue("tax");
            
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["B2"].PutValue("Doe");
            sheet.Cells["C2"].PutValue(30);
            sheet.Cells["D2"].PutValue("10%");
            
            sheet.Cells["A3"].PutValue("Jane");
            sheet.Cells["B3"].PutValue("Smith");
            sheet.Cells["C3"].PutValue(25);
            sheet.Cells["D3"].PutValue(0.15);

            // Konfigurera SQL-sparalternativ
            SqlScriptSaveOptions sqlSaveOptions = new SqlScriptSaveOptions();
            sqlSaveOptions.OperatorType = SqlScriptOperatorType.Insert;
            sqlSaveOptions.CreateTable = true;
            sqlSaveOptions.CheckAllDataForColumnType = true; // This will examine all data to determine column types
            
            // Spara som SQL‑script – Spara‑metoden returnerar inte en sträng, så vi måste spara först och sedan läsa filen
            wb.Save("output.sql", sqlSaveOptions);
            
            // Läs det genererade SQL‑scriptet
            string sqlScript = System.IO.File.ReadAllText("output.sql");
            
            Console.WriteLine("SQL Script generated:");
            Console.WriteLine(sqlScript);
        }
    }
}
```

### Se även

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


