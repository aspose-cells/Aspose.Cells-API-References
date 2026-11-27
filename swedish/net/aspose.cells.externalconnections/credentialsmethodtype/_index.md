---
title: "Enum CredentialsMethodType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ExternalConnections.CredentialsMethodType enum. Anger vilken autentiseringsmetod som används för serveråtkomst"
type: docs
url: /sv/net/aspose.cells.externalconnections/credentialsmethodtype/
---
## CredentialsMethodType enumeration

Anger metod för autentiseringsuppgifter som används för serveråtkomst.

```csharp
public enum CredentialsMethodType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Integrated | `0` | Integrerad autentisering |
| None | `1` | Inga autentiseringsuppgifter |
| Prompt | `2` | Begär autentiseringsuppgifter |
| Stored | `3` | Lagrade autentiseringsuppgifter |

### Exempel

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
                // Visa alla enum‑värden för CredentialsMethodType
                Console.WriteLine("Available CredentialsMethodType values:");
                
                foreach (CredentialsMethodType method in Enum.GetValues(typeof(CredentialsMethodType)))
                {
                    Console.WriteLine($"{method} ({(int)method}) - {GetMethodDescription(method)}");
                }

                // Visa praktisk användning med ett specifikt värde
                CredentialsMethodType selectedMethod = CredentialsMethodType.Integrated;
                Console.WriteLine($"\nSelected method: {selectedMethod}");
                
                // Visa användning av switch
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

### Se även

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


