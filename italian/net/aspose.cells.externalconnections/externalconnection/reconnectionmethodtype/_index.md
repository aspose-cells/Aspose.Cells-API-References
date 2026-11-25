---
title: "ExternalConnection.ReconnectionMethodType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExternalConnection. Specifica cosa deve fare l'applicazione di foglio di calcolo quando una connessione fallisce. Il valore predefinito è ReConnectionMethodType.Required"
type: docs
url: /it/net/aspose.cells.externalconnections/externalconnection/reconnectionmethodtype/
---
## ExternalConnection.ReconnectionMethodType property

Specifica cosa dovrebbe fare l'applicazione di foglio di calcolo quando una connessione fallisce. Il valore predefinito è ReConnectionMethodType.Required.

```csharp
public ReConnectionMethodType ReconnectionMethodType { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyReconnectionMethodTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Accedi alla prima connessione esterna (supponendo che ne esista una)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Visualizza il valore corrente di ReconnectionMethodType
                Console.WriteLine("Initial ReconnectionMethodType: " + connection.ReconnectionMethodType);
                
                // Dimostra l'impostazione della proprietà (poiché è leggibile e scrivibile)
                connection.ReconnectionMethodType = ReConnectionMethodType.Always;
                Console.WriteLine("Updated ReconnectionMethodType: " + connection.ReconnectionMethodType);
                
                // Scorri i valori possibili per dimostrare la capacità di impostazione
                foreach (ReConnectionMethodType method in Enum.GetValues(typeof(ReConnectionMethodType)))
                {
                    connection.ReconnectionMethodType = method;
                    Console.WriteLine($"ReconnectionMethodType set to: {method}");
                }
                
                // Salva la cartella di lavoro con le impostazioni di connessione modificate
                workbook.Save("ReconnectionMethodTypeDemo.xlsx");
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

* enum [ReConnectionMethodType](../../reconnectionmethodtype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


