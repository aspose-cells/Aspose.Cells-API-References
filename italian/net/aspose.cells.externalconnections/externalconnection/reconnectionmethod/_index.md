---
title: "ExternalConnection.ReconnectionMethod"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExternalConnection. Specifica cosa deve fare l'applicazione di foglio di calcolo quando una connessione fallisce. Il valore predefinito è ReConnectionMethodType.Required"
type: docs
url: /it/net/aspose.cells.externalconnections/externalconnection/reconnectionmethod/
---
## ExternalConnection.ReconnectionMethod property

Specifica cosa dovrebbe fare l'applicazione di foglio di calcolo quando una connessione fallisce. Il valore predefinito è ReConnectionMethodType.Required.

```csharp
[Obsolete("Use ExternalConnection.ReconnectionMethodType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ReConnectionMethodType ReconnectionMethod { get; set; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà ExternalConnection.ReconnectionMethodType. Questa proprietà sarà rimossa 12 mesi dopo, a partire da ottobre 2017. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyReconnectionMethodDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Accedi alla prima connessione esterna (supponendo che ne esista una)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Visualizza il valore corrente di ReconnectionMethod (operazione di lettura)
                Console.WriteLine("Initial ReconnectionMethod value: " + connection.ReconnectionMethod);
                
                // Imposta nuovi valori di ReconnectionMethod (poiché è leggibile e scrivibile)
                connection.ReconnectionMethod = ReConnectionMethodType.Always;
                Console.WriteLine("Updated ReconnectionMethod value: " + connection.ReconnectionMethod);
                
                connection.ReconnectionMethod = ReConnectionMethodType.Never;
                Console.WriteLine("Updated ReconnectionMethod value: " + connection.ReconnectionMethod);
                
                // Ripristina al valore predefinito
                connection.ReconnectionMethod = ReConnectionMethodType.Required;
                Console.WriteLine("Reset ReconnectionMethod value: " + connection.ReconnectionMethod);
                
                // Salva la cartella di lavoro con le impostazioni di connessione modificate
                workbook.Save("ReconnectionMethodDemo.xlsx");
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


