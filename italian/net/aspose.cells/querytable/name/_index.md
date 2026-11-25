---
title: "QueryTable.Name"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà QueryTable. Ottiene il nome della querytable"
type: docs
url: /it/net/aspose.cells/querytable/name/
---
## QueryTable.Name property

Ottiene il nome della querytable.

```csharp
public string Name { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per simulare una tabella di query
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");

            try
            {
                // Verifica se ci sono tabelle query nel foglio di lavoro
                if (worksheet.QueryTables.Count > 0)
                {
                    // Ottieni la prima tabella query
                    QueryTable queryTable = worksheet.QueryTables[0];

                    // Visualizza il valore della proprietà Name (operazione di sola lettura)
                    Console.WriteLine("Query Table Name: " + queryTable.Name);

                    // Visualizza altre proprietà di sola lettura per contesto
                    Console.WriteLine("Connection ID: " + queryTable.ConnectionId);
                    Console.WriteLine("Result Range: " + queryTable.ResultRange.Address);
                }
                else
                {
                    Console.WriteLine("No query tables found in the worksheet.");
                }

                // Salva la cartella di lavoro
                workbook.Save("QueryTableNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


