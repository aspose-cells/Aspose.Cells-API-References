---
title: "Enum CredentialsMethodType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ExternalConnections.CredentialsMethodType Enum. Gibt die für den Serverzugriff verwendete Anmeldemethode an"
type: docs
url: /de/net/aspose.cells.externalconnections/credentialsmethodtype/
---
## CredentialsMethodType enumeration

Gibt die Anmeldemethode an, die für den Serverzugriff verwendet wird.

```csharp
public enum CredentialsMethodType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Integrated | `0` | Integrierte Authentifizierung |
| None | `1` | Keine Anmeldeinformationen |
| Prompt | `2` | Anmeldeinformationen abfragen |
| Stored | `3` | Gespeicherte Anmeldeinformationen |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassCredentialsMethodTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Demonstriere alle Enum-Werte von CredentialsMethodType
                Console.WriteLine("Available CredentialsMethodType values:");
                
                foreach (CredentialsMethodType method in Enum.GetValues(typeof(CredentialsMethodType)))
                {
                    Console.WriteLine($"{method} ({(int)method}) - {GetMethodDescription(method)}");
                }

                // Zeige praktische Anwendung mit einem konkreten Wert
                CredentialsMethodType selectedMethod = CredentialsMethodType.Integrated;
                Console.WriteLine($"\nSelected method: {selectedMethod}");
                
                // Demonstriere die Verwendung von Switch
                switch (selectedMethod)
                {
                    case CredentialsMethodType.Integrated:
                        Console.WriteLine("Using integrated authentication");
                        break;
                    case CredentialsMethodType.None:
                        Console.WriteLine("No credentials will be used");
                        break;
                    case CredentialsMethodType.Prompt:
                        Console.WriteLine("User will be prompted for credentials");
                        break;
                    case CredentialsMethodType.Stored:
                        Console.WriteLine("Using stored credentials");
                        break;
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating CredentialsMethodType: {ex.Message}");
            }
        }

        private static string GetMethodDescription(CredentialsMethodType method)
        {
            return method switch
            {
                CredentialsMethodType.Integrated => "Integrated Authentication",
                CredentialsMethodType.None => "No Credentials",
                CredentialsMethodType.Prompt => "Prompt Credentials",
                CredentialsMethodType.Stored => "Stored Credentials",
                _ => "Unknown method"
            };
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


