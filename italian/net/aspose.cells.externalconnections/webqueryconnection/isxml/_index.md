---
title: "WebQueryConnection.IsXml"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WebQueryConnection. true se la sorgente della query web è XML anziché HTML, altrimenti false"
type: docs
url: /it/net/aspose.cells.externalconnections/webqueryconnection/isxml/
---
## WebQueryConnection.IsXml property

true se la sorgente della query web è XML (invece di HTML), altrimenti false.

```csharp
public bool IsXml { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsXmlDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Accedi alla prima connessione dati (supponendo che sia una WebQueryConnection)
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Mostra il valore iniziale di IsXml
                    Console.WriteLine("Initial IsXml value: " + connection.IsXml);
                    
                    // Imposta IsXml a true (poiché è leggibile e scrivibile)
                    connection.IsXml = true;
                    Console.WriteLine("Updated IsXml value: " + connection.IsXml);
                    
                    // Imposta IsXml nuovamente a false
                    connection.IsXml = false;
                    Console.WriteLine("Final IsXml value: " + connection.IsXml);
                    
                    // Salva la cartella di lavoro
                    workbook.Save("WebQueryConnectionIsXmlDemo.xlsx");
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


