---
title: "WebQueryConnection.EditWebPage"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WebQueryConnection. L'URL della pagina web destinata all'utente che mostra i dati della query web. Questo URL viene conservato nel caso in cui sourceDatatrue e url siano stati reindirizzati a un file XML. In tal modo la pagina destinata all'utente può essere mostrata nell'interfaccia e i dati XML possono essere recuperati in background."
type: docs
url: /it/net/aspose.cells.externalconnections/webqueryconnection/editwebpage/
---
## WebQueryConnection.EditWebPage property

L'URL della pagina web destinata all'utente che mostra i dati della query web. Questo URL è conservato nel caso in cui sourceData=\"true\" e l'url sia stato reindirizzato per fare riferimento a un file XML. Allora la pagina destinata all'utente può essere mostrata nell'interfaccia, e i dati XML possono essere recuperati in background.

```csharp
public string EditWebPage { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyEditWebPageDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Accedi alla prima connessione di query web esistente (se presente)
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Imposta il valore iniziale di EditWebPage
                    connection.EditWebPage = "https://example.com/user-facing-page.html";
                    Console.WriteLine("Initial EditWebPage value: " + connection.EditWebPage);
                    
                    // Aggiorna il valore di EditWebPage
                    connection.EditWebPage = "https://example.com/updated-user-page.html";
                    Console.WriteLine("Updated EditWebPage value: " + connection.EditWebPage);
                    
                    // Salva la cartella di lavoro con la connessione di query web
                    workbook.Save("WebQueryConnectionEditWebPageDemo.xlsx");
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


