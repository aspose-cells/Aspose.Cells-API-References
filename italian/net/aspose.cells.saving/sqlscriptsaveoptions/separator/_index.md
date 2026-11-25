---
title: "SqlScriptSaveOptions.Separator"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SqlScriptSaveOptions. Ottiene e imposta il separatore di caratteri dello script SQL"
type: docs
url: /it/net/aspose.cells.saving/sqlscriptsaveoptions/separator/
---
## SqlScriptSaveOptions.Separator property

Ottiene e imposta il separatore di caratteri dello script SQL.

```csharp
public char Separator { get; set; }
```

### Osservazioni

Può essere solo ' ' o '\n'. Se il

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertySeparatorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["B2"].PutValue("John");

            // Configura le opzioni di salvataggio SQL con separatore personalizzato
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                Separator = ';',
                TableName = "Employees",
                CreateTable = true,
                HasHeaderRow = true
            };

            // Salva con separatore personalizzato
            workbook.Save("SqlScriptWithSeparator.sql", saveOptions);

            Console.WriteLine("SQL script saved with custom separator.");
        }
    }
}
```

### Vedi anche

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


