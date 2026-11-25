---
title: "WebQueryConnection.IsParsePre"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WebQueryConnection. Flag che indica se i dati contenuti nei tag HTML PRE della pagina web vengono analizzati in colonne quando importi la pagina in una tabella di query"
type: docs
url: /it/net/aspose.cells.externalconnections/webqueryconnection/isparsepre/
---
## WebQueryConnection.IsParsePre property

Flag che indica se i dati contenuti nei tag HTML PRE nella pagina web vengono analizzati in colonne quando si importa la pagina in una tabella di query.

```csharp
public bool IsParsePre { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsParsePreDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Crea una nuova connessione di query web utilizzando la connessione esistente dalla cartella di lavoro
                WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[0];
                
                // Mostra il valore iniziale di IsParsePre (predefinito)
                Console.WriteLine("Initial IsParsePre value: " + connection.IsParsePre);
                
                // Imposta IsParsePre su true
                connection.IsParsePre = true;
                Console.WriteLine("Updated IsParsePre value: " + connection.IsParsePre);
                
                // Imposta IsParsePre a false
                connection.IsParsePre = false;
                Console.WriteLine("Final IsParsePre value: " + connection.IsParsePre);
                
                // Salva la cartella di lavoro
                workbook.Save("WebQueryConnectionIsParsePreDemo.xlsx");
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


