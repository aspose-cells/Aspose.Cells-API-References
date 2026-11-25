---
title: "SqlScriptSaveOptions.CreateTable"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SqlScriptSaveOptions. Indica se esportare l'SQL per la creazione della tabella"
type: docs
url: /it/net/aspose.cells.saving/sqlscriptsaveoptions/createtable/
---
## SqlScriptSaveOptions.CreateTable property

Indica se esportare SQL per la creazione della tabella.

```csharp
public bool CreateTable { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyCreateTableDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Jane");

            // Configura le opzioni di esportazione SQL con CreateTable abilitato
            SqlScriptSaveOptions options = new SqlScriptSaveOptions
            {
                CreateTable = true,
                TableName = "Employees",
                HasHeaderRow = true
            };

            // Salva come script SQL
            workbook.Save("output.sql", options);
        }
    }
}
```

### Vedi anche

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


