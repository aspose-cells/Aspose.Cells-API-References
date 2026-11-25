---
title: "SqlScriptSaveOptions.StartId"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SqlScriptSaveOptions. Ottiene e imposta l'ID iniziale"
type: docs
url: /it/net/aspose.cells.saving/sqlscriptsaveoptions/startid/
---
## SqlScriptSaveOptions.StartId property

Ottiene e imposta l'ID iniziale.

```csharp
public int StartId { get; set; }
```

### Osservazioni

Funziona solo quando [`IdName`](../idname/) è impostato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyStartIdDemo
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

            // Configura le opzioni di esportazione SQL con StartId impostato a 100
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                TableName = "Employees",
                IdName = "ID",
                StartId = 100, // Demonstrating StartId property
                HasHeaderRow = true,
                OperatorType = SqlScriptOperatorType.Insert
            };

            // Salva come script SQL
            workbook.Save("Employees_WithStartId.sql", saveOptions);
        }
    }
}
```

### Vedi anche

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


