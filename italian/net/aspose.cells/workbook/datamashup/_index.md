---
title: "Workbook.DataMashup"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Workbook. Ottiene i dati mashup"
type: docs
url: /it/net/aspose.cells/workbook/datamashup/
---
## Workbook.DataMashup property

Ottiene i dati mashup.

```csharp
public DataMashup DataMashup { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyDataMashupDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per attivare Power Query
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(150);

            // Salva su un file
            string sourcePath = "source.xlsx";
            workbook.Save(sourcePath);

            // Riapri la cartella di lavoro per accedere a DataMashup
            workbook = new Workbook(sourcePath);
            
            // Accedi alle formule Power Query tramite la proprietà DataMashup
            var queries = workbook.DataMashup.PowerQueryFormulas;
            
            // Restituisci informazioni di base sulle query
            Console.WriteLine($"Number of Power Query formulas: {queries.Count}");
            
            // Se ci sono query, mostra i dettagli della prima
            if (queries.Count > 0)
            {
                foreach (var query in queries)
                {
                    Console.WriteLine($"Query Name: {query.Name}");
                    Console.WriteLine($"Number of items: {query.PowerQueryFormulaItems.Count}");
                    break; // Just show first query for demo
                }
            }

            // Salva su un nuovo file
            string destPath = "output.xlsx";
            workbook.Save(destPath);
        }
    }
}
```

### Vedi anche

* class [DataMashup](../../../aspose.cells.querytables/datamashup/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


