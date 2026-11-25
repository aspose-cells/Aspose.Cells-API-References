---
title: "ExternalConnection.OnlyUseConnectionFile"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExternalConnection. Indica se l'applicazione di foglio di calcolo deve sempre e solo utilizzare le informazioni di connessione nel file di connessione esterno indicato dall'attributo odcFile quando la connessione viene aggiornata. Se false, l'applicazione di foglio di calcolo deve seguire la procedura indicata dall'attributo reconnectionMethod"
type: docs
url: /it/net/aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile/
---
## ExternalConnection.OnlyUseConnectionFile property

Indica se l'applicazione di foglio di calcolo dovrebbe sempre e solo utilizzare le informazioni di connessione nel file di connessione esterna indicato dall'attributo odcFile quando la connessione viene aggiornata. Se false, l'applicazione di foglio di calcolo dovrebbe seguire la procedura indicata dall'attributo reconnectionMethod.

```csharp
public bool OnlyUseConnectionFile { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyOnlyUseConnectionFileDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Accedi alla prima connessione esterna (supponendo che ne esista una)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Visualizza il valore corrente di OnlyUseConnectionFile
                Console.WriteLine("Initial OnlyUseConnectionFile value: " + connection.OnlyUseConnectionFile);
                
                // Imposta un nuovo valore di OnlyUseConnectionFile (poiché è leggibile e scrivibile)
                connection.OnlyUseConnectionFile = true;
                Console.WriteLine("Updated OnlyUseConnectionFile value: " + connection.OnlyUseConnectionFile);
                
                // Attiva/disattiva il valore per dimostrare la capacità di impostazione
                connection.OnlyUseConnectionFile = !connection.OnlyUseConnectionFile;
                Console.WriteLine("Toggled OnlyUseConnectionFile value: " + connection.OnlyUseConnectionFile);
                
                // Salva la cartella di lavoro con le impostazioni di connessione modificate
                workbook.Save("OnlyUseConnectionFileDemo.xlsx");
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


