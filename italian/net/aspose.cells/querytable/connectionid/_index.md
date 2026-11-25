---
title: "QueryTable.ConnectionId"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà QueryTable. Ottiene l'ID di connessione della query table"
type: docs
url: /it/net/aspose.cells/querytable/connectionid/
---
## QueryTable.ConnectionId property

Ottiene l'ID di connessione della tabella query.

```csharp
public int ConnectionId { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyConnectionIdDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per simulare uno scenario di tabella di query
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Sample Data");

            try
            {
                // Verifica se ci sono tabelle query nel foglio di lavoro
                if (worksheet.QueryTables.Count > 0)
                {
                    // Ottieni la prima tabella query
                    QueryTable queryTable = worksheet.QueryTables[0];

                    // Visualizza il valore della proprietà ConnectionId (di sola lettura)
                    Console.WriteLine("Query Table ConnectionId: " + queryTable.ConnectionId);

                    // Visualizza altre proprietà correlate per contesto
                    Console.WriteLine("Query Table Name: " + queryTable.Name);
                    Console.WriteLine("External Connection: " +
                        (queryTable.ExternalConnection != null ? queryTable.ExternalConnection.Name : "None"));
                }
                else
                {
                    Console.WriteLine("No query tables found in the worksheet.");
                }

                // Salva la cartella di lavoro
                workbook.Save("ConnectionIdDemo.xlsx");
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


