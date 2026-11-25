---
title: "Enum CredentialsMethodType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.ExternalConnections.CredentialsMethodType enum. Specifica il metodo di credenziali utilizzato per l'accesso al server"
type: docs
url: /it/net/aspose.cells.externalconnections/credentialsmethodtype/
---
## CredentialsMethodType enumeration

Specifica il metodo Credentials utilizzato per l'accesso al server.

```csharp
public enum CredentialsMethodType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Integrated | `0` | Autenticazione integrata |
| None | `1` | Nessuna credenziale |
| Prompt | `2` | Richiedi credenziali |
| Stored | `3` | Credenziali memorizzate |

### Esempi

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
                // Dimostra tutti i valori enum di CredentialsMethodType
                Console.WriteLine("Available CredentialsMethodType values:");
                
                foreach (CredentialsMethodType method in Enum.GetValues(typeof(CredentialsMethodType)))
                {
                    Console.WriteLine($"{method} ({(int)method}) - {GetMethodDescription(method)}");
                }

                // Mostra un utilizzo pratico con un valore specifico
                CredentialsMethodType selectedMethod = CredentialsMethodType.Integrated;
                Console.WriteLine($"\nSelected method: {selectedMethod}");
                
                // Dimostra l'uso del switch
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

### Vedi anche

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


