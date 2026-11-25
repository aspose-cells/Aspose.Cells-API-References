---
title: "ExternalConnection.RefreshOnLoad"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExternalConnection. True se questa connessione deve essere aggiornata all'apertura del file, altrimenti false"
type: docs
url: /it/net/aspose.cells.externalconnections/externalconnection/refreshonload/
---
## ExternalConnection.RefreshOnLoad property

True se questa connessione deve essere aggiornata all'apertura del file; altrimenti, false.

```csharp
public bool RefreshOnLoad { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyRefreshOnLoadDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Accedi alla prima connessione esterna (la cartella di lavoro include connessioni predefinite)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Visualizza il valore iniziale di RefreshOnLoad
                Console.WriteLine("Initial RefreshOnLoad value: " + connection.RefreshOnLoad);
                
                // Dimostra l'impostazione della proprietà (poiché è leggibile e scrivibile)
                connection.RefreshOnLoad = !connection.RefreshOnLoad;
                Console.WriteLine("Updated RefreshOnLoad value: " + connection.RefreshOnLoad);
                
                // Salva la cartella di lavoro con le impostazioni di connessione modificate
                workbook.Save("RefreshOnLoadDemo.xlsx");
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


