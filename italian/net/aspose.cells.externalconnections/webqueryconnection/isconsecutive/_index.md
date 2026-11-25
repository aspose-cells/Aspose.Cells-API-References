---
title: "WebQueryConnection.IsConsecutive"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WebQueryConnection. Flag che indica se i delimitatori consecutivi devono essere trattati come un unico delimitatore"
type: docs
url: /it/net/aspose.cells.externalconnections/webqueryconnection/isconsecutive/
---
## WebQueryConnection.IsConsecutive property

Flag che indica se i delimitatori consecutivi devono essere trattati come un unico delimitatore.

```csharp
public bool IsConsecutive { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsConsecutiveDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Crea una connessione di query web accedendo alla prima connessione
            // (presumendo che sia disponibile almeno una connessione)
            WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[0];
            
            try
            {
                // Mostra il valore iniziale di IsConsecutive (predefinito)
                Console.WriteLine("Initial IsConsecutive value: " + connection.IsConsecutive);
                
                // Imposta IsConsecutive su true
                connection.IsConsecutive = true;
                Console.WriteLine("Updated IsConsecutive value: " + connection.IsConsecutive);
                
                // Reimposta IsConsecutive su false
                connection.IsConsecutive = false;
                Console.WriteLine("Final IsConsecutive value: " + connection.IsConsecutive);
                
                // Salva la cartella di lavoro con la connessione di query web
                workbook.Save("WebQueryConnectionIsConsecutiveDemo.xlsx");
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


