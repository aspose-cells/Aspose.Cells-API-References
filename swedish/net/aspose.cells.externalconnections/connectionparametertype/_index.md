---
title: "Enum ConnectionParameterType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ExternalConnections.ConnectionParameterType‑enum. Anger parametertypen för extern anslutning"
type: docs
url: /sv/net/aspose.cells.externalconnections/connectionparametertype/
---
## ConnectionParameterType enumeration

Anger parametertypen för extern anslutning

```csharp
public enum ConnectionParameterType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Cell | `0` | Hämta parametervärdet från en cell vid varje uppdatering. |
| Prompt | `1` | Be användaren om ett parametervärde vid varje uppdatering. |
| Value | `2` | Använd ett konstant värde vid varje uppdatering för parametervärdet. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassConnectionParameterTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Demonstrera hur man skapar och använder enum‑värden för ConnectionParameterType
                ConnectionParameterType cellParam = ConnectionParameterType.Cell;
                ConnectionParameterType promptParam = ConnectionParameterType.Prompt;
                ConnectionParameterType valueParam = ConnectionParameterType.Value;

                // Visa enum‑värden
                Console.WriteLine("Connection Parameter Types:");
                Console.WriteLine($"Cell: {cellParam}");
                Console.WriteLine($"Prompt: {promptParam}");
                Console.WriteLine($"Value: {valueParam}");

                // Demonstrera användning i ett switch‑uttryck
                ConnectionParameterType testParam = ConnectionParameterType.Prompt;
                switch (testParam)
                {
                    case ConnectionParameterType.Cell:
                        Console.WriteLine("Parameter will get value from a cell");
                        break;
                    case ConnectionParameterType.Prompt:
                        Console.WriteLine("Parameter will prompt user for value");
                        break;
                    case ConnectionParameterType.Value:
                        Console.WriteLine("Parameter will use constant value");
                        break;
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating ConnectionParameterType: {ex.Message}");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


