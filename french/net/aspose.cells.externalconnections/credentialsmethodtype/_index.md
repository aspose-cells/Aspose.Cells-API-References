---
title: "Enum CredentialsMethodType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.ExternalConnections.CredentialsMethodType enum. Spécifie la méthode d'identification utilisée pour l'accès au serveur"
type: docs
url: /fr/net/aspose.cells.externalconnections/credentialsmethodtype/
---
## CredentialsMethodType enumeration

Spécifie la méthode d'identifiants utilisée pour l'accès au serveur.

```csharp
public enum CredentialsMethodType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Integrated | `0` | Authentification intégrée |
| None | `1` | Aucune identification |
| Prompt | `2` | Demander les identifiants |
| Stored | `3` | Identifiants stockés |

### Exemples

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
                // Démontrer toutes les valeurs d'énumération de CredentialsMethodType
                Console.WriteLine("Available CredentialsMethodType values:");
                
                foreach (CredentialsMethodType method in Enum.GetValues(typeof(CredentialsMethodType)))
                {
                    Console.WriteLine($"{method} ({(int)method}) - {GetMethodDescription(method)}");
                }

                // Afficher un exemple d'utilisation avec une valeur spécifique
                CredentialsMethodType selectedMethod = CredentialsMethodType.Integrated;
                Console.WriteLine($"\nSelected method: {selectedMethod}");
                
                // Démontrer l'utilisation du switch
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

### Voir aussi

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


