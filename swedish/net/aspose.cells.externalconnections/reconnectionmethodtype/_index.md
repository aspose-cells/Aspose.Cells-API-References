---
title: "Enum ReConnectionMethodType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ExternalConnections.ReConnectionMethodType‑enum. Anger vad kalkylbladsapplikationen ska göra när en anslutning misslyckas"
type: docs
url: /sv/net/aspose.cells.externalconnections/reconnectionmethodtype/
---
## ReConnectionMethodType enumeration

Anger vad kalkylbladsapplikationen ska göra när en anslutning misslyckas.

```csharp
public enum ReConnectionMethodType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Required | `1` | Vid uppdatering, använd den befintliga anslutningsinformationen och om den visar sig vara ogiltig, hämta uppdaterad anslutningsinformation, om den finns tillgänglig i den externa anslutningsfilen. |
| Always | `2` | Vid varje uppdatering hämta uppdaterad anslutningsinformation från den externa anslutningsfilen, om den är tillgänglig, och använd den istället för den befintliga anslutningsinformationen. I detta fall kommer datauppdateringen att misslyckas om den externa anslutningsfilen är otillgänglig. |
| Never | `3` | Hämta aldrig uppdaterad anslutningsinformation från den externa anslutningsfilen även om den är tillgänglig och även om den befintliga anslutningsinformationen är ogiltig |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassReConnectionMethodTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Demonstrera hur man skapar och använder enum‑värden för ReConnectionMethodType
                ReConnectionMethodType method1 = ReConnectionMethodType.Required;
                ReConnectionMethodType method2 = ReConnectionMethodType.Always;
                ReConnectionMethodType method3 = ReConnectionMethodType.Never;

                Console.WriteLine("ReConnectionMethodType values:");
                Console.WriteLine($"Required: {(int)method1}");
                Console.WriteLine($"Always: {(int)method2}");
                Console.WriteLine($"Never: {(int)method3}");

                // Visa användning i ett switch‑uttryck
                Console.WriteLine("\nDemonstrating switch usage:");
                TestConnectionMethod(method1);
                TestConnectionMethod(method2);
                TestConnectionMethod(method3);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ReConnectionMethodType: {ex.Message}");
            }
        }

        private static void TestConnectionMethod(ReConnectionMethodType method)
        {
            switch (method)
            {
                case ReConnectionMethodType.Required:
                    Console.WriteLine("Using Required reconnection method");
                    break;
                case ReConnectionMethodType.Always:
                    Console.WriteLine("Using Always reconnection method");
                    break;
                case ReConnectionMethodType.Never:
                    Console.WriteLine("Using Never reconnection method");
                    break;
                default:
                    Console.WriteLine("Unknown reconnection method");
                    break;
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


