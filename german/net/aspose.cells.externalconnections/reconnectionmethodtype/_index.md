---
title: "Enum ReConnectionMethodType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ExternalConnections.ReConnectionMethodType‑Enum. Gibt an, was die Tabellenkalkulationsanwendung tun soll, wenn eine Verbindung fehlschlägt"
type: docs
url: /de/net/aspose.cells.externalconnections/reconnectionmethodtype/
---
## ReConnectionMethodType enumeration

Gibt an, was die Tabellenkalkulationsanwendung tun soll, wenn eine Verbindung fehlschlägt.

```csharp
public enum ReConnectionMethodType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Required | `1` | Bei einer Aktualisierung die vorhandenen Verbindungsinformationen verwenden und, falls diese ungültig sind, aktualisierte Verbindungsinformationen aus der externen Verbindungsdatei abrufen, sofern verfügbar. |
| Always | `2` | Bei jeder Aktualisierung die aktualisierten Verbindungsinformationen aus der externen Verbindungsdatei abrufen, falls verfügbar, und diese anstelle der vorhandenen Verbindungsinformationen verwenden. In diesem Fall schlägt die Datenaktualisierung fehl, wenn die externe Verbindungsdatei nicht verfügbar ist. |
| Never | `3` | Nie die aktualisierten Verbindungsinformationen aus der externen Verbindungsdatei abrufen, selbst wenn sie verfügbar ist und selbst wenn die vorhandenen Verbindungsinformationen ungültig sind. |

### Beispiele

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
                // Demonstriere das Erstellen und Verwenden von ReConnectionMethodType-Enum-Werten.
                ReConnectionMethodType method1 = ReConnectionMethodType.Required;
                ReConnectionMethodType method2 = ReConnectionMethodType.Always;
                ReConnectionMethodType method3 = ReConnectionMethodType.Never;

                Console.WriteLine("ReConnectionMethodType values:");
                Console.WriteLine($"Required: {(int)method1}");
                Console.WriteLine($"Always: {(int)method2}");
                Console.WriteLine($"Never: {(int)method3}");

                // Zeige die Verwendung in einer switch-Anweisung.
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

### Siehe auch

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


