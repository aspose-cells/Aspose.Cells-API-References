---
title: "WebQueryConnection.IsXl2000"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "WebQueryConnection proprietà. Questa flag esiste per compatibilità retroattiva con file di foglio di calcolo più vecchi esistenti ed è impostata su true se questa query web è stata aggiornata in un'applicazione di foglio di calcolo più recente o uguale a Microsoft Excel 2000. Questo è un attributo opzionale che può essere ignorato"
type: docs
url: /it/net/aspose.cells.externalconnections/webqueryconnection/isxl2000/
---
## WebQueryConnection.IsXl2000 property

Questo flag esiste per compatibilità retroattiva con file di foglio di calcolo più vecchi esistenti, ed è impostato su true se questa query web è stata aggiornata in un'applicazione di foglio di calcolo più recente o uguale a Microsoft Excel 2000. Questo è un attributo opzionale che può essere ignorato.

```csharp
public bool IsXl2000 { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsXl2000Demo
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
                    // Visualizza il valore iniziale di IsXl2000
                    Console.WriteLine("Initial IsXl2000 value: " + connection.IsXl2000);

                    // Imposta IsXl2000 su true (poiché è leggibile e scrivibile)
                    connection.IsXl2000 = true;
                    Console.WriteLine("Updated IsXl2000 value: " + connection.IsXl2000);

                    // Reimposta IsXl2000 su false
                    connection.IsXl2000 = false;
                    Console.WriteLine("Final IsXl2000 value: " + connection.IsXl2000);

                    // Salva la cartella di lavoro
                    workbook.Save("WebQueryConnectionIsXl2000Demo.xlsx");
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


