---
title: "WebQueryConnection.IsHtmlTables"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WebQueryConnection. Flag che indica se le query web devono funzionare solo su tabelle HTML"
type: docs
url: /it/net/aspose.cells.externalconnections/webqueryconnection/ishtmltables/
---
## WebQueryConnection.IsHtmlTables property

Flag che indica se le query web devono funzionare solo su tabelle HTML.

```csharp
public bool IsHtmlTables { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsHtmlTablesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();

            try
            {
                // Crea una connessione di query web tramite l'indicizzatore della raccolta
                WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[workbook.DataConnections.Count];

                Console.WriteLine("Initial IsHtmlTables: " + connection.IsHtmlTables);
                
                connection.IsHtmlTables = true;
                Console.WriteLine("Updated IsHtmlTables: " + connection.IsHtmlTables);

                workbook.Save("IsHtmlTablesDemo.xlsx");
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


