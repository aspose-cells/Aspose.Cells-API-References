---
title: "SqlScriptSaveOptions.CheckAllDataForColumnType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SqlScriptSaveOptions. Controlla tutti i dati per trovare il tipo di dati delle colonne"
type: docs
url: /it/net/aspose.cells.saving/sqlscriptsaveoptions/checkalldataforcolumntype/
---
## SqlScriptSaveOptions.CheckAllDataForColumnType property

Controlla tutti i dati per trovare il tipo di dato delle colonne.

```csharp
public bool CheckAllDataForColumnType { get; set; }
```

### Osservazioni

Il valore predefinito è false, controlliamo solo la prima riga per motivi di prestazioni. Se questa proprietà è true e le colonne contengono tipi di valore misti, il tipo delle colonne sarà testo.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyCheckAllDataForColumnTypeDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di esempio con dati di test
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Aggiungi dati di esempio con tipi misti
            sheet.Cells["A1"].PutValue("First_name");
            sheet.Cells["B1"].PutValue("Last_name");
            sheet.Cells["C1"].PutValue("age");
            sheet.Cells["D1"].PutValue("tax");
            
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["B2"].PutValue("Doe");
            sheet.Cells["C2"].PutValue(30);
            sheet.Cells["D2"].PutValue("10%");
            
            sheet.Cells["A3"].PutValue("Jane");
            sheet.Cells["B3"].PutValue("Smith");
            sheet.Cells["C3"].PutValue(25);
            sheet.Cells["D3"].PutValue(0.15);

            // Configura le opzioni di salvataggio SQL
            SqlScriptSaveOptions sqlSaveOptions = new SqlScriptSaveOptions();
            sqlSaveOptions.OperatorType = SqlScriptOperatorType.Insert;
            sqlSaveOptions.CreateTable = true;
            sqlSaveOptions.CheckAllDataForColumnType = true; // This will examine all data to determine column types
            
            // Salva come script SQL - il metodo Save non restituisce una stringa, quindi è necessario salvare prima e poi leggere il file
            wb.Save("output.sql", sqlSaveOptions);
            
            // Leggi lo script SQL generato
            string sqlScript = System.IO.File.ReadAllText("output.sql");
            
            Console.WriteLine("SQL Script generated:");
            Console.WriteLine(sqlScript);
        }
    }
}
```

### Vedi anche

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


