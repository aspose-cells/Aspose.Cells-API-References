---
title: "WebQueryConnection.HtmlFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WebQueryConnection. Come gestire la formattazione dalla sorgente HTML quando si importano i dati della query web nel foglio di lavoro. Rilevante quando sourceData è True"
type: docs
url: /it/net/aspose.cells.externalconnections/webqueryconnection/htmlformat/
---
## WebQueryConnection.HtmlFormat property

Come gestire la formattazione dalla sorgente HTML quando si importano i dati della query web nel foglio di lavoro. Rilevante quando sourceData è True.

```csharp
public HtmlFormatHandlingType HtmlFormat { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyHtmlFormatDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi alla prima connessione di query web esistente (se presente)
            // Oppure crea una nuova caricando un file con connessioni web
            if (workbook.DataConnections.Count > 0)
            {
                try
                {
                    WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[0];
                    
                    // Mostra il valore iniziale di HtmlFormat
                    Console.WriteLine("Initial HtmlFormat value: " + connection.HtmlFormat);
                    
                    // Imposta HtmlFormat su Rtf (dimostrando l'operazione di scrittura)
                    connection.HtmlFormat = HtmlFormatHandlingType.Rtf;
                    Console.WriteLine("Updated HtmlFormat value: " + connection.HtmlFormat);
                    
                    // Imposta HtmlFormat su None
                    connection.HtmlFormat = HtmlFormatHandlingType.None;
                    Console.WriteLine("Final HtmlFormat value: " + connection.HtmlFormat);
                    
                    // Salva la cartella di lavoro con la connessione di query web
                    workbook.Save("WebQueryConnectionHtmlFormatDemo.xlsx");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error: {ex.Message}");
                }
            }
            else
            {
                Console.WriteLine("No web query connections found in the workbook.");
            }
        }
    }
}
```

### Vedi anche

* enum [HtmlFormatHandlingType](../../htmlformathandlingtype/)
* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


