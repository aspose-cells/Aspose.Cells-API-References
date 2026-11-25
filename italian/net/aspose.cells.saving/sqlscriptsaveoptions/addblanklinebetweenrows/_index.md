---
title: "SqlScriptSaveOptions.AddBlankLineBetweenRows"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SqlScriptSaveOptions. Inserisce una riga vuota tra ogni dato"
type: docs
url: /it/net/aspose.cells.saving/sqlscriptsaveoptions/addblanklinebetweenrows/
---
## SqlScriptSaveOptions.AddBlankLineBetweenRows property

Inserisci una riga vuota tra ogni dato.

```csharp
public bool AddBlankLineBetweenRows { get; set; }
```

### Osservazioni

Se [`Separator`](../separator/) è '\n', è meglio impostare questa proprietà su true per aumentare la leggibilità.

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyAddBlankLineBetweenRowsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di esempio con dati di test
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Jane");

            // Configura le opzioni di salvataggio SQL
            SqlScriptSaveOptions options = new SqlScriptSaveOptions
            {
                OperatorType = SqlScriptOperatorType.Insert,
                TableName = "Employees",
                IdName = "ID",
                AddBlankLineBetweenRows = true,
                CreateTable = true
            };

            // Salva su stream di memoria e ottieni lo script SQL come stringa
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, options);
                stream.Position = 0;
                using (StreamReader reader = new StreamReader(stream))
                {
                    string sqlScript = reader.ReadToEnd();
                    Console.WriteLine("SQL script generated with blank lines between rows:");
                    Console.WriteLine(sqlScript);
                }
            }
        }
    }
}
```

### Vedi anche

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


