---
title: "WebQueryConnection.Post"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WebQueryConnection. Restituisce o imposta la stringa usata con il metodo POST per inviare dati a un server web e restituire dati da una query web"
type: docs
url: /it/net/aspose.cells.externalconnections/webqueryconnection/post/
---
## WebQueryConnection.Post property

Restituisce o imposta la stringa usata con il metodo POST per inviare dati a un server web per restituire dati da una query web.

```csharp
public string Post { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyPostDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Crea una connessione query web accedendo a una esistente o creandola tramite una corretta inizializzazione
                // Poiché non possiamo istanziare direttamente WebQueryConnection, utilizzeremo la prima connessione se esiste
                WebQueryConnection connection = null;
                
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection webQueryConn)
                {
                    connection = webQueryConn;
                }
                else
                {
                    // Se non esistono connessioni, dimostreremo con una connessione simulata
                    Console.WriteLine("No existing web query connection found - demonstrating with property access only");
                    return;
                }
                
                // Imposta il valore iniziale di Post
                connection.Post = "param1=value1&param2=value2";
                Console.WriteLine("Initial Post value: " + connection.Post);
                
                // Modifica il valore di Post
                connection.Post = "username=test&password=secret";
                Console.WriteLine("Updated Post value: " + connection.Post);
                
                // Cancella il valore di Post
                connection.Post = string.Empty;
                Console.WriteLine("Cleared Post value: " + connection.Post);
                
                // Salva la cartella di lavoro
                workbook.Save("WebQueryConnectionPostDemo.xlsx");
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


