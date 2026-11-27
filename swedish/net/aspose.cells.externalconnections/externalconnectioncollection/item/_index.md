---
title: "ExternalConnectionCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalConnectionCollection-egenskap. Hämtar elementet ExternalConnection på det angivna indexet"
type: docs
url: /sv/net/aspose.cells.externalconnections/externalconnectioncollection/item/
---
## ExternalConnectionCollection indexer (1 of 2)

Hämtar elementet [`ExternalConnection`](../../externalconnection/) på det angivna indexet.

```csharp
public ExternalConnection this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Det nollbaserade indexet för elementet. |

### Returvärde

Elementet på det angivna indexet.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            try
            {
                // Kom åt den externa anslutningssamlingen
                ExternalConnectionCollection connections = workbook.DataConnections;

                // Kontrollera om det finns några anslutningar
                if (connections.Count > 0)
                {
                    // Demonstrera åtkomst till ett objekt via index (läsoperation)
                    ExternalConnection connection = connections[0];

                    // Visa anslutningsinformation
                    Console.WriteLine($"Connection Name: {connection.Name}");
                    Console.WriteLine($"Connection Type: {connection.Type}");
                    Console.WriteLine($"Connection ID: {connection.ConnectionId}");
                }
                else
                {
                    Console.WriteLine("No external connections available to demonstrate Item property");
                }

                // Spara arbetsboken
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

### Se även

* class [ExternalConnection](../../externalconnection/)
* class [ExternalConnectionCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)

---

## ExternalConnectionCollection indexer (2 of 2)

Hämtar [`ExternalConnection`](../../externalconnection/)‑elementet med det angivna namnet.

```csharp
public ExternalConnection this[string connectionName] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| connectionName | namnet på datakopplingen |

### Returvärde

Elementet med det angivna namnet.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Kom åt den externa anslutningssamlingen
                ExternalConnectionCollection connections = workbook.DataConnections;
                
                // Lägg till en exempelanslutning (om det behövs för demonstration)
                // Detta förutsätter att samlingen tillåter att lägga till anslutningar
                // connections.Add(new ExternalConnection());
                
                // Demonstrera åtkomst till ett objekt via namn (läsoperation)
                // Obs: I ett verkligt scenario skulle du behöva faktiska anslutningsnamn
                if (connections.Count > 0)
                {
                    // Hämta det första anslutningsnamnet (om tillgängligt)
                    string connectionName = connections[0].Name;
                    
                    // Åtkomst till egenskapen Item
                    ExternalConnection connection = connections[connectionName];
                    
                    // Visa anslutningsinformation
                    Console.WriteLine($"Connection Name: {connection.Name}");
                    Console.WriteLine($"Connection Type: {connection.Type}");
                }
                else
                {
                    Console.WriteLine("No external connections available to demonstrate Item property");
                }
                
                // Spara arbetsboken
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

### Se även

* class [ExternalConnection](../../externalconnection/)
* class [ExternalConnectionCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


