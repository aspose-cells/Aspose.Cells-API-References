---
title: "SqlScriptSaveOptions.OperatorType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SqlScriptSaveOptions. Ottiene e imposta il tipo di operatore di sql"
type: docs
url: /it/net/aspose.cells.saving/sqlscriptsaveoptions/operatortype/
---
## SqlScriptSaveOptions.OperatorType property

Ottiene e imposta il tipo di operatore SQL.

```csharp
public SqlScriptOperatorType OperatorType { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyOperatorTypeDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di esempio con dati di test
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Id");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Jane");

            // Configura le opzioni di salvataggio SQL
            SqlScriptSaveOptions options = new SqlScriptSaveOptions();
            options.OperatorType = SqlScriptOperatorType.Delete;
            options.IdName = "Id";
            options.Separator = '\n';
            options.AddBlankLineBetweenRows = true;
            options.CreateTable = true;

            // Salva su stream di memoria e ottieni lo script SQL come stringa
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, options);
                stream.Position = 0;
                using (StreamReader reader = new StreamReader(stream))
                {
                    string sqlScript = reader.ReadToEnd();
                    
                    // Restituisci l'SQL generato
                    Console.WriteLine("Generated SQL Script:");
                    Console.WriteLine(sqlScript);
                }
            }
        }
    }
}
```

### Vedi anche

* enum [SqlScriptOperatorType](../../sqlscriptoperatortype/)
* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


