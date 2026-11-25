---
title: "SqlScriptSaveOptions.SqlScriptSaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore SqlScriptSaveOptions. Crea opzioni per salvare un file sql"
type: docs
url: /it/net/aspose.cells.saving/sqlscriptsaveoptions/sqlscriptsaveoptions/
---
## SqlScriptSaveOptions constructor

Crea le opzioni per il salvataggio del file SQL.

```csharp
public SqlScriptSaveOptions()
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");

            // Crea SqlScriptSaveOptions usando il costruttore
            SqlScriptSaveOptions options = new SqlScriptSaveOptions();
            options.OperatorType = SqlScriptOperatorType.Insert;
            options.AddBlankLineBetweenRows = true;

            // Salva come script SQL
            workbook.Save("output.sql", options);
            
            // Restituisci l'SQL generato
            Console.WriteLine("Generated SQL Script:");
            Console.WriteLine(System.IO.File.ReadAllText("output.sql"));
        }
    }
}
```

### Vedi anche

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


