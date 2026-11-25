---
title: "Workbook.DataConnections"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Workbook. Restituisce la collezione ExternalConnection"
type: docs
url: /it/net/aspose.cells/workbook/dataconnections/
---
## Workbook.DataConnections property

Restituisce la collezione [`ExternalConnection`](../../../aspose.cells.externalconnections/externalconnection/).

```csharp
public ExternalConnectionCollection DataConnections { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookPropertyDataConnectionsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Crea un foglio di lavoro di esempio
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati per rendere l'esempio significativo
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Accedi alla proprietà DataConnections
                var dataConnections = workbook.DataConnections;

                // Visualizza il valore corrente della proprietà (operazione di lettura)
                Console.WriteLine("DataConnections count: " + dataConnections.Count);

                // Itera attraverso le connessioni, se ne esistono
                for (int i = 0; i < dataConnections.Count; i++)
                {
                    var connection = dataConnections[i];
                    Console.WriteLine($"Connection {i + 1}: {connection.Name}");
                }

                // Mostra come la proprietà influisce sul comportamento
                Console.WriteLine("DataConnections has been demonstrated");

                // Salva il risultato
                workbook.Save("DataConnectionsDemo.xlsx");
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

* class [ExternalConnectionCollection](../../../aspose.cells.externalconnections/externalconnectioncollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


