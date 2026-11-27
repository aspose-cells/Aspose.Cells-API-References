---
title: "ExternalConnection.KeepAlive"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalConnection-egenskap. Sant när kalkylprogrammet ska göra ansträngningar för att hålla anslutningen öppen. När falskt ska programmet stänga anslutningen efter att informationen hämtats"
type: docs
url: /sv/net/aspose.cells.externalconnections/externalconnection/keepalive/
---
## ExternalConnection.KeepAlive property

True när kalkylbladsapplikationen bör göra ansträngningar för att hålla anslutningen öppen. När false ska applikationen stänga anslutningen efter att informationen har hämtats.

```csharp
public bool KeepAlive { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyKeepAliveDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Åtkomst till den första externa anslutningen (förutsatt att en sådan finns)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Visa det aktuella KeepAlive-värdet
                Console.WriteLine("Initial KeepAlive value: " + connection.KeepAlive);
                
                // Växla KeepAlive‑värdet eftersom det är läs‑skriv
                connection.KeepAlive = !connection.KeepAlive;
                Console.WriteLine("Updated KeepAlive value: " + connection.KeepAlive);
                
                // Spara arbetsboken med de ändrade anslutningsinställningarna
                workbook.Save("KeepAliveDemo.xlsx");
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


