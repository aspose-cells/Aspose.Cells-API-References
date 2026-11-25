---
title: "WebQueryConnection.ConnectionFile"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WebQueryConnection. Ottiene il file di connessione"
type: docs
url: /it/net/aspose.cells.externalconnections/webqueryconnection/connectionfile/
---
## WebQueryConnection.ConnectionFile property

Ottiene il file di connessione.

```csharp
public override string ConnectionFile { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyConnectionFileDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Crea un foglio di lavoro di esempio con i dati della query web
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].Value = "Sample Web Query Data";
                
                // Ottieni la prima connessione di query web esistente (se presente)
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Mostra il valore di ConnectionFile (proprietà di sola lettura)
                    Console.WriteLine("ConnectionFile value: " + connection.ConnectionFile);
                    
                    // Salva la cartella di lavoro
                    workbook.Save("WebQueryConnectionFileDemo.xlsx");
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


