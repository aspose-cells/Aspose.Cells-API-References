---
title: "WebQueryConnection.IsXmlSourceData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WebQueryConnection. Flag che indica che i dati sorgente XML devono essere importati invece della tabella HTML stessa"
type: docs
url: /it/net/aspose.cells.externalconnections/webqueryconnection/isxmlsourcedata/
---
## WebQueryConnection.IsXmlSourceData property

Flag che indica che i dati sorgente XML devono essere importati invece della tabella HTML stessa.

```csharp
public bool IsXmlSourceData { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsXmlSourceDataDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Accedi a una connessione di query web esistente o creane una tramite un'adeguata inizializzazione
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Mostra il valore iniziale di IsXmlSourceData
                    Console.WriteLine("Initial IsXmlSourceData value: " + connection.IsXmlSourceData);
                    
                    // Imposta IsXmlSourceData su true
                    connection.IsXmlSourceData = true;
                    Console.WriteLine("Updated IsXmlSourceData value: " + connection.IsXmlSourceData);
                    
                    // Reimposta IsXmlSourceData su false
                    connection.IsXmlSourceData = false;
                    Console.WriteLine("Final IsXmlSourceData value: " + connection.IsXmlSourceData);
                    
                    // Salva la cartella di lavoro
                    workbook.Save("WebQueryConnectionIsXmlSourceDataDemo.xlsx");
                }
                else
                {
                    Console.WriteLine("No web query connections found in the workbook.");
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


