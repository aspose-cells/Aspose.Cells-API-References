---
title: "ExternalConnectionCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExternalConnectionCollection‑Eigenschaft. Ruft das ExternalConnection‑Element am angegebenen Index ab."
type: docs
url: /de/net/aspose.cells.externalconnections/externalconnectioncollection/item/
---
## ExternalConnectionCollection indexer (1 of 2)

Ruft das [`ExternalConnection`](../../externalconnection/) Element am angegebenen Index ab.

```csharp
public ExternalConnection this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der nullbasierte Index des Elements. |

### Rückgabewert

Das Element am angegebenen Index.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            try
            {
                // Greife auf die Sammlung externer Verbindungen zu
                ExternalConnectionCollection connections = workbook.DataConnections;

                // Überprüfe, ob es irgendwelche Verbindungen gibt
                if (connections.Count > 0)
                {
                    // Demonstriere den Zugriff auf ein Element per Index (Lesevorgang)
                    ExternalConnection connection = connections[0];

                    // Zeige Verbindungsinformationen an
                    Console.WriteLine($"Connection Name: {connection.Name}");
                    Console.WriteLine($"Connection Type: {connection.Type}");
                    Console.WriteLine($"Connection ID: {connection.ConnectionId}");
                }
                else
                {
                    Console.WriteLine("No external connections available to demonstrate Item property");
                }

                // Speichere die Arbeitsmappe
                workbook.Save("ExternalConnectionItemDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [ExternalConnection](../../externalconnection/)
* class [ExternalConnectionCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)

---

## ExternalConnectionCollection indexer (2 of 2)

Ruft das [`ExternalConnection`](../../externalconnection/) Element mit dem angegebenen Namen ab.

```csharp
public ExternalConnection this[string connectionName] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| connectionName | der Name der Datenverbindung |

### Rückgabewert

Das Element mit dem angegebenen Namen.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Greife auf die Sammlung externer Verbindungen zu
                ExternalConnectionCollection connections = workbook.DataConnections;
                
                // Füge eine Beispielverbindung hinzu (falls für die Demonstration erforderlich)
                // Dies setzt voraus, dass die Sammlung das Hinzufügen von Verbindungen erlaubt
                // connections.Add(new ExternalConnection());
                
                // Demonstriere den Zugriff auf ein Element nach Namen (Leseoperation)
                // Hinweis: In einem realen Szenario bräuchtest du tatsächliche Verbindungsnamen
                if (connections.Count > 0)
                {
                    // Erhalte den ersten Verbindungsnamen (falls verfügbar)
                    string connectionName = connections[0].Name;
                    
                    // Greife auf die Item-Eigenschaft zu
                    ExternalConnection connection = connections[connectionName];
                    
                    // Zeige Verbindungsinformationen an
                    Console.WriteLine($"Connection Name: {connection.Name}");
                    Console.WriteLine($"Connection Type: {connection.Type}");
                }
                else
                {
                    Console.WriteLine("No external connections available to demonstrate Item property");
                }
                
                // Speichere die Arbeitsmappe
                workbook.Save("ExternalConnectionDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [ExternalConnection](../../externalconnection/)
* class [ExternalConnectionCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


