---
title: "SqlScriptSaveOptions.PrimaryKey"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SqlScriptSaveOptions. Rappresenta quale colonna è la chiave primaria della tabella dati"
type: docs
url: /it/net/aspose.cells.saving/sqlscriptsaveoptions/primarykey/
---
## SqlScriptSaveOptions.PrimaryKey property

Rappresenta quale colonna è la chiave primaria della tabella dati.

```csharp
public int PrimaryKey { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyPrimaryKeyDemo
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

            // Configura le opzioni di esportazione SQL con PrimaryKey impostata alla prima colonna (0)
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                PrimaryKey = 0,
                TableName = "Employees",
                CreateTable = true,
                HasHeaderRow = true
            };

            // Salva come script SQL
            workbook.Save("EmployeesExport.sql", saveOptions);

            Console.WriteLine("SQL script exported with PrimaryKey set to column 0 (ID)");
        }
    }
}
```

### Vedi anche

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


