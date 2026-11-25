---
title: "WebQueryConnection.IsTextDates"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "WebQueryConnection proprietà. Flag che indica se le date devono essere importate nelle celle del foglio di lavoro come testo anziché come date"
type: docs
url: /it/net/aspose.cells.externalconnections/webqueryconnection/istextdates/
---
## WebQueryConnection.IsTextDates property

Flag che indica se le date devono essere importate nelle celle del foglio di lavoro come testo anziché come date.

```csharp
public bool IsTextDates { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsTextDatesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Accedi al primo foglio di lavoro
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Crea una connessione di query web caricandola da un file esistente
                // oppure accedendo a una connessione esistente
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Visualizza il valore iniziale di IsTextDates
                    Console.WriteLine("Initial IsTextDates value: " + connection.IsTextDates);
                    
                    // Imposta IsTextDates su true
                    connection.IsTextDates = true;
                    Console.WriteLine("Updated IsTextDates value: " + connection.IsTextDates);
                    
                    // Reimposta IsTextDates su false
                    connection.IsTextDates = false;
                    Console.WriteLine("Final IsTextDates value: " + connection.IsTextDates);
                    
                    // Salva la cartella di lavoro con la connessione di query web
                    workbook.Save("WebQueryConnectionIsTextDatesDemo.xlsx");
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


