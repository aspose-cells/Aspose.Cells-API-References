---
title: "QueryTable.ExternalConnection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà QueryTable. Ottiene la connessione esterna correlata"
type: docs
url: /it/net/aspose.cells/querytable/externalconnection/
---
## QueryTable.ExternalConnection property

Ottiene la connessione esterna correlata.

```csharp
public ExternalConnection ExternalConnection { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class QueryTablePropertyExternalConnectionDemo
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

                    // Accedi alla proprietà ExternalConnection (di sola lettura)
                    ExternalConnection externalConnection = queryTable.ExternalConnection;

                    // Visualizza le informazioni sulla connessione esterna
                    if (externalConnection != null)
                    {
                        Console.WriteLine("External Connection ID: " + externalConnection.Id);
                        Console.WriteLine("External Connection Name: " + externalConnection.Name);
                        Console.WriteLine("External Connection Type: " + externalConnection.ClassType);
                        Console.WriteLine("Connection String: " + externalConnection.ConnectionString);
                        Console.WriteLine("Refresh on Load: " + externalConnection.RefreshOnLoad);
                    }
                    else
                    {
                        Console.WriteLine("No external connection associated with this query table.");
                    }

                    // Visualizza altre proprietà della query table per contesto
                    Console.WriteLine("Query Table Name: " + queryTable.Name);
                    Console.WriteLine("Connection ID: " + queryTable.ConnectionId);
                }
                else
                {
                    Console.WriteLine("No query tables found in the worksheet.");
                }

                // Salva la cartella di lavoro
                workbook.Save("ExternalConnectionDemo.xlsx");
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

* class [ExternalConnection](../../../aspose.cells.externalconnections/externalconnection/)
* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


