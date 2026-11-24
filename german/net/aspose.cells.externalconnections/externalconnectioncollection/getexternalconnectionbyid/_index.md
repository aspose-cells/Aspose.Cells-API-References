---
title: "ExternalConnectionCollection.GetExternalConnectionById"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExternalConnectionCollection‑Methode. Ruft das ExternalConnection‑Element mit der angegebenen ID ab."
type: docs
url: /de/net/aspose.cells.externalconnections/externalconnectioncollection/getexternalconnectionbyid/
---
## ExternalConnectionCollection.GetExternalConnectionById method

Ruft das [`ExternalConnection`](../../externalconnection/) Element mit der angegebenen ID ab.

```csharp
public ExternalConnection GetExternalConnectionById(int connId)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| connId | Int32 | ID der externen Verbindung |

### Rückgabewert

Das Element mit der angegebenen ID.

### Beispiele

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
            // Erstelle eine neue Arbeitsmappe mit Beispiel‑Datenverbindungen
            Workbook workbook = new Workbook();
            
            // Rufe die Sammlung externer Verbindungen ab
            ExternalConnectionCollection dataConns = workbook.DataConnections;

            // Erstelle und füge Verbindungen mit den richtigen API‑Methoden hinzu
            // Hinweis: In der realen Anwendung würden Sie typischerweise vorhandene Verbindungen abrufen
            // statt neue Verbindungen auf diese Weise zu erstellen
            int connectionId1 = 1;
            int connectionId2 = 2;
            
            // Hole eine bestimmte Verbindung nach ID (ist zunächst null).
            ExternalConnection specificConn = dataConns.GetExternalConnectionById(connectionId1);
            
            if (specificConn == null)
            {
                Console.WriteLine($"No connection found with ID {connectionId1}");
                // In der realen Anwendung würden Sie mit vorhandenen Verbindungen arbeiten
                // oder sie über die richtigen API‑Methoden erstellen
            }
            else
            {
                Console.WriteLine($"Found connection: ID={specificConn.ConnectionId}, Name={specificConn.Name}");
                specificConn.Name = "ModifiedConnection";
            }

            // Speichere die Arbeitsmappe
            workbook.Save("ExternalConnectionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ExternalConnection](../../externalconnection/)
* class [ExternalConnectionCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


