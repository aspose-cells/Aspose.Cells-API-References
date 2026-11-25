---
title: "WebQueryConnection.Url"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WebQueryConnection. URL da utilizzare per aggiornare i dati esterni"
type: docs
url: /it/net/aspose.cells.externalconnections/webqueryconnection/url/
---
## WebQueryConnection.Url property

URL da utilizzare per aggiornare dati esterni.

```csharp
public string Url { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyUrlDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una connessione di query web aggiungendola alla raccolta
            // La raccolta probabilmente creerà e restituirà l'oggetto connessione
            WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[workbook.DataConnections.Count];

            // Imposta l'URL iniziale per la query web
            connection.Url = "https://example.com/data.html";
            Console.WriteLine("Initial URL: " + connection.Url);

            // Modifica l'URL a una fonte diversa
            connection.Url = "https://example.com/updated-data.xml";
            Console.WriteLine("Updated URL: " + connection.Url);

            // Configura la connessione per analizzare dati XML
            connection.IsXml = true;

            // Aggiorna la connessione dati (normalmente recupererebbe i dati dall'URL)
            // Nota: L'accesso web reale richiederebbe connettività di rete
            // workbook.RefreshAllConnections();

            // Salva la cartella di lavoro con la connessione di query web
            workbook.Save("WebQueryConnectionUrlDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


