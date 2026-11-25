---
title: "SqlScriptColumnTypeMap.GetNumbericType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SqlScriptColumnTypeMap. Restituisce il tipo numerico nel database"
type: docs
url: /it/net/aspose.cells.saving/sqlscriptcolumntypemap/getnumberictype/
---
## SqlScriptColumnTypeMap.GetNumbericType method

Ottiene il tipo numerico nel database.

```csharp
[Obsolete("Use SqlScriptColumnTypeMap.GetNumberType() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual string GetNumbericType()
```

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo SqlScriptColumnTypeMap.GetNumberType(). Questo metodo sarà rimosso 6 mesi dopo, a partire da luglio 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptColumnTypeMapMethodGetNumbericTypeDemo
    {
        public static void Run()
        {
            // Crea un'istanza di SqlScriptColumnTypeMap
            SqlScriptColumnTypeMap columnTypeMap = new SqlScriptColumnTypeMap();

            // Ottieni e visualizza la mappatura dei tipi numerici
            string numericType = columnTypeMap.GetNumbericType();
            Console.WriteLine("Numeric Type in Database: " + numericType);

            // Crea una cartella di lavoro semplice con dati numerici
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Number");
            worksheet.Cells["A2"].PutValue(123.45);

            // Salva con le opzioni di script SQL usando la mappatura dei tipi
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                ColumnTypeMap = columnTypeMap
            };
            workbook.Save("NumericTypeDemo.sql", saveOptions);
        }
    }
}
```

### Vedi anche

* class [SqlScriptColumnTypeMap](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


