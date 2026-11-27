---
title: "ExternalConnectionCollection.GetExternalConnectionById"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalConnectionCollection-metod. Hämtar elementet ExternalConnection med det angivna id:t"
type: docs
url: /sv/net/aspose.cells.externalconnections/externalconnectioncollection/getexternalconnectionbyid/
---
## ExternalConnectionCollection.GetExternalConnectionById method

Hämtar elementet [`ExternalConnection`](../../externalconnection/) med det angivna id:t.

```csharp
public ExternalConnection GetExternalConnectionById(int connId)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| connId | Int32 | externt anslutnings-id |

### Returvärde

Elementet med det angivna id:t.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionCollectionMethodGetExternalConnectionByIdWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempel på dataanslutningar
            Workbook workbook = new Workbook();
            
            // Hämta den externa anslutningssamlingen
            ExternalConnectionCollection dataConns = workbook.DataConnections;

            // Skapa och lägg till anslutningar med korrekta API-metoder
            // Obs: Vid verklig användning skulle du vanligtvis hämta befintliga anslutningar
            // istället för att skapa nya på detta sätt
            int connectionId1 = 1;
            int connectionId2 = 2;
            
            // Hämta specifik anslutning efter ID (kommer initialt att vara null)
            ExternalConnection specificConn = dataConns.GetExternalConnectionById(connectionId1);
            
            if (specificConn == null)
            {
                Console.WriteLine($"No connection found with ID {connectionId1}");
                // Vid verklig användning skulle du arbeta med befintliga anslutningar
                // eller skapa dem via korrekta API-metoder
            }
            else
            {
                Console.WriteLine($"Found connection: ID={specificConn.ConnectionId}, Name={specificConn.Name}");
                specificConn.Name = "ModifiedConnection";
            }

            // Spara arbetsboken
            workbook.Save("ExternalConnectionDemo.xlsx");
        }
    }
}
```

### Se även

* class [ExternalConnection](../../externalconnection/)
* class [ExternalConnectionCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


