---
title: "Worksheet.QueryTables"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Ottiene QueryTableCollection nel foglio di lavoro"
type: docs
url: /it/net/aspose.cells/worksheet/querytables/
---
## Worksheet.QueryTables property

Ottiene [`QueryTableCollection`](../../querytablecollection/) nel foglio di lavoro.

```csharp
public QueryTableCollection QueryTables { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyQueryTablesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);
            
            // Ottieni la prima tabella di query (poiché non possiamo aggiungerne di nuove direttamente)
            // Nota: la collezione QueryTables è di sola lettura in questa versione dell'API
            if (worksheet.QueryTables.Count > 0)
            {
                QueryTable queryTable = worksheet.QueryTables[0];
                
                // Visualizza le informazioni della tabella di query
                Console.WriteLine("Query Table Name: " + queryTable.Name);
                Console.WriteLine("Result Range: " + queryTable.ResultRange.Address);
                Console.WriteLine("Number of Query Tables: " + worksheet.QueryTables.Count);
            }
            else
            {
                Console.WriteLine("No query tables found in the worksheet.");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("QueryTableDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [QueryTableCollection](../../querytablecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


