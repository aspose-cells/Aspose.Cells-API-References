---
title: "SqlScriptSaveOptions.HasHeaderRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SqlScriptSaveOptions. Indica se l'intervallo contiene una riga di intestazione"
type: docs
url: /it/net/aspose.cells.saving/sqlscriptsaveoptions/hasheaderrow/
---
## SqlScriptSaveOptions.HasHeaderRow property

Indica se l'intervallo contiene la riga di intestazione.

```csharp
public bool HasHeaderRow { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyHasHeaderRowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi la riga di intestazione e dati di esempio
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Alice");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Bob");

            // Configura le opzioni di esportazione SQL con HasHeaderRow=true
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                TableName = "Employees",
                HasHeaderRow = true,
                CreateTable = true
            };

            // Salva come script SQL
            workbook.Save("Employees.sql", saveOptions);

            Console.WriteLine("SQL script with header row exported successfully.");
        }
    }
}
```

### Vedi anche

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


