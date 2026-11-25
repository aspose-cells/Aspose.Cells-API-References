---
title: "SqlScriptSaveOptions.SheetIndexes"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SqlScriptSaveOptions. Rappresenta gli indici dei fogli esportati"
type: docs
url: /it/net/aspose.cells.saving/sqlscriptsaveoptions/sheetindexes/
---
## SqlScriptSaveOptions.SheetIndexes property

Rappresenta gli indici dei fogli esportati.

```csharp
public int[] SheetIndexes { get; set; }
```

### Esempi

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
            // Crea una nuova cartella di lavoro con più fogli
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Popola alcuni dati in tutti i fogli
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

            // Crea un'istanza di SqlScriptSaveOptions
            SqlScriptSaveOptions options = new SqlScriptSaveOptions
            {
                TableName = "Employees",
                CreateTable = true,
                HasHeaderRow = true
            };

            // Visualizza gli SheetIndexes attuali (null indica tutti i fogli)
            Console.WriteLine("Initial SheetIndexes: " + 
                (options.SheetIndexes == null ? "All sheets" : string.Join(",", options.SheetIndexes)));

            // Imposta SheetIndexes per esportare solo il primo e il terzo foglio (0 e 2)
            options.SheetIndexes = new int[] { 0, 2 };

            // Salva con le opzioni
            workbook.Save("SqlScriptExportSelectedSheets.sql", options);

            // Modifica SheetIndexes per esportare solo il secondo foglio
            options.SheetIndexes = new int[] { 1 };
            workbook.Save("SqlScriptExportSecondSheet.sql", options);

            // Imposta SheetIndexes a null per esportare tutti i fogli
            options.SheetIndexes = null;
            workbook.Save("SqlScriptExportAllSheets.sql", options);
        }
    }
}
```

### Vedi anche

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


