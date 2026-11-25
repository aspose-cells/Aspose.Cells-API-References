---
title: "SqlScriptSaveOptions.ExportAsString"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SqlScriptSaveOptions. Indica se esportare tutti i dati come valore stringa"
type: docs
url: /it/net/aspose.cells.saving/sqlscriptsaveoptions/exportasstring/
---
## SqlScriptSaveOptions.ExportAsString property

Indica se esportare tutti i dati come valore stringa.

```csharp
public bool ExportAsString { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyExportAsStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["B2"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue("Bob");

            // Configura le opzioni di esportazione SQL
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                TableName = "Employees",
                ExportAsString = true, // Demonstrating ExportAsString property
                HasHeaderRow = true
            };

            // Salva con esportazione stringa abilitata
            workbook.Save("ExportAsString_True.sql", saveOptions);

            // Modifica su false e salva nuovamente
            saveOptions.ExportAsString = false;
            workbook.Save("ExportAsString_False.sql", saveOptions);

            Console.WriteLine("SQL scripts saved with different ExportAsString settings.");
        }
    }
}
```

### Vedi anche

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


