---
title: "ExternalConnection.RefreshOnLoad"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalConnection-egenskap. Sant om denna anslutning ska uppdateras när filen öppnas, annars falskt"
type: docs
url: /sv/net/aspose.cells.externalconnections/externalconnection/refreshonload/
---
## ExternalConnection.RefreshOnLoad property

True om denna anslutning ska uppdateras när filen öppnas; annars false.

```csharp
public bool RefreshOnLoad { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyRefreshOnLoadDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Åtkomst till den första externa anslutningen (arbetsboken levereras med standardanslutningar)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Visa initialt RefreshOnLoad-värde
                Console.WriteLine("Initial RefreshOnLoad value: " + connection.RefreshOnLoad);
                
                // Demonstrera att sätta egenskapen (eftersom den är läs-skriv)
                connection.RefreshOnLoad = !connection.RefreshOnLoad;
                Console.WriteLine("Updated RefreshOnLoad value: " + connection.RefreshOnLoad);
                
                // Spara arbetsboken med de ändrade anslutningsinställningarna
                workbook.Save("RefreshOnLoadDemo.xlsx");
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

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


