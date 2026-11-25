---
title: "ExternalConnection.BackgroundRefresh"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExternalConnection. Indica se la connessione può essere aggiornata in background in modo asincrono. true se l'uso preferito della connessione è aggiornare in modo asincrono in background, false se l'uso preferito della connessione è aggiornare in modo sincrono in primo piano"
type: docs
url: /it/net/aspose.cells.externalconnections/externalconnection/backgroundrefresh/
---
## ExternalConnection.BackgroundRefresh property

Indica se la connessione può essere aggiornata in background (asincronicamente). true se l'uso preferito della connessione è aggiornare asincronamente in background; false se l'uso preferito della connessione è aggiornare sincronicamente in primo piano.

```csharp
public bool BackgroundRefresh { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyBackgroundRefreshDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Accedi alla prima connessione esterna (supponendo che ne esista una)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Visualizza il valore corrente di BackgroundRefresh
                Console.WriteLine("Initial BackgroundRefresh value: " + connection.BackgroundRefresh);
                
                // Attiva/disattiva il valore di BackgroundRefresh
                connection.BackgroundRefresh = !connection.BackgroundRefresh;
                Console.WriteLine("Updated BackgroundRefresh value: " + connection.BackgroundRefresh);
                
                // Salva la cartella di lavoro con le impostazioni di connessione modificate
                workbook.Save("BackgroundRefreshDemo.xlsx");
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


