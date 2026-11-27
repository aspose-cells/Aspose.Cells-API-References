---
title: "WebQueryConnection.IsSameSettings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebQueryConnection egenskap. Flagga som indikerar om alla tabeller i ett PRE‑block ska parsas med samma breddinställningar som den första raden"
type: docs
url: /sv/net/aspose.cells.externalconnections/webqueryconnection/issamesettings/
---
## WebQueryConnection.IsSameSettings property

Flagga som anger om alla tabeller inom ett PRE-block ska parsas med samma breddinställningar som den första raden.

```csharp
public bool IsSameSettings { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsSameSettingsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Kom åt den första befintliga webbförfrågningsanslutningen om den finns
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Visa initialt värde för IsSameSettings
                    Console.WriteLine("Initial IsSameSettings value: " + connection.IsSameSettings);
                    
                    // Ställ in IsSameSettings till true (eftersom den är läs‑skriv)
                    connection.IsSameSettings = true;
                    Console.WriteLine("Updated IsSameSettings value: " + connection.IsSameSettings);
                    
                    // Ställ in IsSameSettings tillbaka till false
                    connection.IsSameSettings = false;
                    Console.WriteLine("Final IsSameSettings value: " + connection.IsSameSettings);
                    
                    // Spara arbetsboken
                    workbook.Save("WebQueryConnectionIsSameSettingsDemo.xlsx");
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

### Se även

* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


