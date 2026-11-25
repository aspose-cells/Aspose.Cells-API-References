---
title: "WebQueryConnection.EditPage"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WebQueryConnection. L'URL della pagina web destinata all'utente che mostra i dati della query web. Questo URL viene conservato nel caso in cui sourceDatatrue e url siano stati reindirizzati a un file XML. In tal modo la pagina destinata all'utente può essere mostrata nell'interfaccia e i dati XML possono essere recuperati in background."
type: docs
url: /it/net/aspose.cells.externalconnections/webqueryconnection/editpage/
---
## WebQueryConnection.EditPage property

L'URL della pagina web destinata all'utente che mostra i dati della query web. Questo URL è conservato nel caso in cui sourceData=\"true\" e l'url sia stato reindirizzato per fare riferimento a un file XML. Allora la pagina destinata all'utente può essere mostrata nell'interfaccia, e i dati XML possono essere recuperati in background.

```csharp
[Obsolete("Use WebQueryConnection.EditWebPage property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string EditPage { get; set; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, utilizza la proprietà WebQueryConnection.EditWebPage. Questa proprietà sarà rimossa tra 12 mesi a partire da ottobre 2017. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyEditPageDemo
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
                    // Mostra il valore iniziale di EditPage
                    Console.WriteLine("Initial EditPage value: " + connection.EditPage);
                    
                    // Imposta EditPage a un nuovo URL (poiché è leggibile e scrivibile)
                    connection.EditPage = "https://example.com/editpage";
                    Console.WriteLine("Updated EditPage value: " + connection.EditPage);
                    
                    // Salva la cartella di lavoro
                    workbook.Save("WebQueryConnectionEditPageDemo.xlsx");
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


