---
title: "ExternalConnection.KeepAlive"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExternalConnection. True quando l'applicazione di foglio di calcolo dovrebbe fare sforzi per mantenere la connessione aperta. Quando false l'applicazione dovrebbe chiudere la connessione dopo aver recuperato le informazioni."
type: docs
url: /it/net/aspose.cells.externalconnections/externalconnection/keepalive/
---
## ExternalConnection.KeepAlive property

True quando l'applicazione di foglio di calcolo dovrebbe impegnarsi a mantenere la connessione aperta. Quando false, l'applicazione dovrebbe chiudere la connessione dopo aver recuperato le informazioni.

```csharp
public bool KeepAlive { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyKeepAliveDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Accedi alla prima connessione esterna (supponendo che ne esista una)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Visualizza il valore corrente di KeepAlive
                Console.WriteLine("Initial KeepAlive value: " + connection.KeepAlive);
                
                // Attiva/disattiva il valore KeepAlive poiché è leggibile-scrivibile
                connection.KeepAlive = !connection.KeepAlive;
                Console.WriteLine("Updated KeepAlive value: " + connection.KeepAlive);
                
                // Salva la cartella di lavoro con le impostazioni di connessione modificate
                workbook.Save("KeepAliveDemo.xlsx");
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


