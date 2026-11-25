---
title: "SqlScriptColumnTypeMap.GetStringType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SqlScriptColumnTypeMap. Ottiene il tipo stringa nel database"
type: docs
url: /it/net/aspose.cells.saving/sqlscriptcolumntypemap/getstringtype/
---
## SqlScriptColumnTypeMap.GetStringType method

Ottiene il tipo stringa nel database.

```csharp
public virtual string GetStringType()
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptColumnTypeMapMethodGetStringTypeDemo
    {
        public static void Run()
        {
            // Crea un'istanza di SqlScriptColumnTypeMap
            SqlScriptColumnTypeMap columnTypeMap = new SqlScriptColumnTypeMap();

            // Ottieni e visualizza il tipo stringa predefinito
            string stringType = columnTypeMap.GetStringType();
            Console.WriteLine("Default String Type: " + stringType);

            // Crea una cartella di lavoro semplice con dati stringa
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John Doe");

            // Salva con le opzioni di script SQL usando la mappa dei tipi
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                ColumnTypeMap = columnTypeMap
            };
            
            workbook.Save("SqlScriptOutput.sql", saveOptions);
            Console.WriteLine("SQL script saved with string type: " + stringType);
        }
    }
}
```

### Vedi anche

* class [SqlScriptColumnTypeMap](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


