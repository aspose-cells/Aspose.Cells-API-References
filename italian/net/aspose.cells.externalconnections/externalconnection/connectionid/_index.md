---
title: "ExternalConnection.ConnectionId"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExternalConnection. Specifica l'identificatore univoco di questa connessione"
type: docs
url: /it/net/aspose.cells.externalconnections/externalconnection/connectionid/
---
## ExternalConnection.ConnectionId property

Specifica l'identificatore univoco di questa connessione.

```csharp
[Obsolete("Use ExternalConnection.Id property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int ConnectionId { get; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà ExternalConnection.Id. Questa proprietà sarà rimossa tra 12 mesi a partire da ottobre 2024. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyConnectionIdDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            try
            {
                // Accedi alla prima connessione esterna (la cartella di lavoro include connessioni predefinite)
                ExternalConnection connection = workbook.DataConnections[0];

                // Visualizza il valore ConnectionId (proprietà di sola lettura)
                Console.WriteLine("ConnectionId value: " + connection.ConnectionId);

                // Visualizza il valore Id per confronto (anche di sola lettura)
                Console.WriteLine("Id value: " + connection.Id);

                // Mostra che entrambe le proprietà sono di sola lettura tentando di visualizzarle
                Console.WriteLine("ConnectionId and Id are both read-only properties");
                Console.WriteLine("ConnectionId: " + connection.ConnectionId + ", Id: " + connection.Id);

                // Salva la cartella di lavoro
                workbook.Save("ConnectionIdDemo.xlsx");
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

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


