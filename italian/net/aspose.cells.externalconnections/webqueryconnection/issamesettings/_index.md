---
title: "WebQueryConnection.IsSameSettings"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "WebQueryConnection proprietà. Flag che indica se analizzare tutte le tabelle all'interno di un blocco PRE con le stesse impostazioni di larghezza della prima riga"
type: docs
url: /it/net/aspose.cells.externalconnections/webqueryconnection/issamesettings/
---
## WebQueryConnection.IsSameSettings property

Flag che indica se analizzare tutte le tabelle all'interno di un blocco PRE con le stesse impostazioni di larghezza della prima riga.

```csharp
public bool IsSameSettings { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsSameSettingsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Accedi alla prima connessione di query web esistente, se disponibile
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Mostra il valore iniziale di IsSameSettings
                    Console.WriteLine("Initial IsSameSettings value: " + connection.IsSameSettings);
                    
                    // Imposta IsSameSettings su true (poiché è leggibile e scrivibile)
                    connection.IsSameSettings = true;
                    Console.WriteLine("Updated IsSameSettings value: " + connection.IsSameSettings);
                    
                    // Reimposta IsSameSettings su false
                    connection.IsSameSettings = false;
                    Console.WriteLine("Final IsSameSettings value: " + connection.IsSameSettings);
                    
                    // Salva la cartella di lavoro
                    workbook.Save("WebQueryConnectionIsSameSettingsDemo.xlsx");
                }
                else
                {
                    Console.WriteLine("No web query connection found in the workbook.");
                }
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

* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


