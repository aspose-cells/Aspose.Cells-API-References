---
title: "SqlScriptSaveOptions.SheetIndexes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SqlScriptSaveOptions-egenskap. Representerar indexen för exporterade blad"
type: docs
url: /sv/net/aspose.cells.saving/sqlscriptsaveoptions/sheetindexes/
---
## SqlScriptSaveOptions.SheetIndexes property

Representerar indexen för exporterade blad.

```csharp
public int[] SheetIndexes { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class SqlScriptSaveOptionsPropertySheetIndexesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med flera blad
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Fyll i lite data i alla blad
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Worksheet worksheet = workbook.Worksheets[i];
                worksheet.Cells["A1"].PutValue("ID");
                worksheet.Cells["B1"].PutValue("Name");
                worksheet.Cells["A2"].PutValue(1);
                worksheet.Cells["B2"].PutValue("John");
                worksheet.Cells["A3"].PutValue(2);
                worksheet.Cells["B3"].PutValue("Jane");
            }

            // Skapa SqlScriptSaveOptions-instans
            SqlScriptSaveOptions options = new SqlScriptSaveOptions
            {
                TableName = "Employees",
                CreateTable = true,
                HasHeaderRow = true
            };

            // Visa aktuella SheetIndexes (null betyder alla blad)
            Console.WriteLine("Initial SheetIndexes: " + 
                (options.SheetIndexes == null ? "All sheets" : string.Join(",", options.SheetIndexes)));

            // Ställ in SheetIndexes för att exportera endast första och tredje bladen (0 och 2)
            options.SheetIndexes = new int[] { 0, 2 };

            // Spara med alternativen
            workbook.Save("SqlScriptExportSelectedSheets.sql", options);

            // Ändra SheetIndexes för att exportera endast det andra bladet
            options.SheetIndexes = new int[] { 1 };
            workbook.Save("SqlScriptExportSecondSheet.sql", options);

            // Ställ SheetIndexes till null för att exportera alla blad
            options.SheetIndexes = null;
            workbook.Save("SqlScriptExportAllSheets.sql", options);
        }
    }
}
```

### Se även

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


