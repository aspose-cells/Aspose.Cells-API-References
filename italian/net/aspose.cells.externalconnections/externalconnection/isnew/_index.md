---
title: "ExternalConnection.IsNew"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExternalConnection. Vero se la connessione non è stata ancora aggiornata per la prima volta, altrimenti falso. Questo stato può verificarsi quando l'utente salva il file prima che una query abbia terminato il ritorno dei dati"
type: docs
url: /it/net/aspose.cells.externalconnections/externalconnection/isnew/
---
## ExternalConnection.IsNew property

True se la connessione non è stata ancora aggiornata per la prima volta; altrimenti, false. Questo stato può verificarsi quando l'utente salva il file prima che una query abbia terminato il ritorno dei dati.

```csharp
public bool IsNew { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyIsNewDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Accedi alla prima connessione esterna (le connessioni appena create sono tipicamente "IsNew")
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Visualizza il valore iniziale di IsNew
                Console.WriteLine("Initial IsNew value: " + connection.IsNew);
                
                // Poiché IsNew è leggibile e scrivibile, dimostra come impostarlo
                connection.IsNew = false;
                Console.WriteLine("Updated IsNew value: " + connection.IsNew);
                
                // Salva la cartella di lavoro con le impostazioni di connessione modificate
                workbook.Save("IsNewDemo.xlsx");
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


