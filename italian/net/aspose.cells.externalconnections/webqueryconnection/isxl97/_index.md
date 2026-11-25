---
title: "WebQueryConnection.IsXl97"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "WebQueryConnection proprietà. Questa flag esiste per compatibilità retroattiva con file di foglio di calcolo più vecchi esistenti ed è impostata su true se questa query web è stata creata in Microsoft Excel 97. Questo è un attributo opzionale che può essere ignorato"
type: docs
url: /it/net/aspose.cells.externalconnections/webqueryconnection/isxl97/
---
## WebQueryConnection.IsXl97 property

Questo flag esiste per compatibilità retroattiva con file di foglio di calcolo più vecchi esistenti, ed è impostato su true se questa query web è stata creata in Microsoft Excel 97. Questo è un attributo opzionale che può essere ignorato.

```csharp
public bool IsXl97 { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsXl97Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Crea un foglio di lavoro con alcuni dati per rendere l'esempio significativo
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].Value = "Sample Data";
                
                // Crea una connessione di query web caricandola da un file esistente o creandola correttamente
                // Poiché non possiamo creare WebQueryConnection direttamente, accederemo a una esistente
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Visualizza il valore iniziale di IsXl97
                    Console.WriteLine("Initial IsXl97 value: " + connection.IsXl97);
                    
                    // Imposta IsXl97 su true (poiché è leggibile e scrivibile)
                    connection.IsXl97 = true;
                    Console.WriteLine("Updated IsXl97 value: " + connection.IsXl97);
                    
                    // Reimposta IsXl97 su false
                    connection.IsXl97 = false;
                    Console.WriteLine("Final IsXl97 value: " + connection.IsXl97);
                    
                    // Salva la cartella di lavoro
                    workbook.Save("WebQueryConnectionIsXl97Demo.xlsx");
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


