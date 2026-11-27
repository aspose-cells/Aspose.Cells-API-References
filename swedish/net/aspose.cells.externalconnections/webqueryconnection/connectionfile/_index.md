---
title: "WebQueryConnection.ConnectionFile"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebQueryConnection‑egenskap. Hämtar anslutningsfilen"
type: docs
url: /sv/net/aspose.cells.externalconnections/webqueryconnection/connectionfile/
---
## WebQueryConnection.ConnectionFile property

Hämtar anslutningsfilen.

```csharp
public override string ConnectionFile { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Skapa ett exempelarbetsblad med webbförfrågningsdata
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].Value = "Sample Web Query Data";
                
                // Hämta den första befintliga webbförfrågningsanslutningen (om någon)
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Visa ConnectionFile‑värdet (skrivskyddad egenskap)
                    Console.WriteLine("ConnectionFile value: " + connection.ConnectionFile);
                    
                    // Spara arbetsboken
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

### Se även

* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


