---
title: "Enum ReConnectionMethodType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.ExternalConnections.ReConnectionMethodType enum. Spécifie ce que l'application de feuille de calcul doit faire lorsqu'une connexion échoue"
type: docs
url: /fr/net/aspose.cells.externalconnections/reconnectionmethodtype/
---
## ReConnectionMethodType enumeration

Spécifie ce que l'application de feuille de calcul doit faire lorsqu'une connexion échoue.

```csharp
public enum ReConnectionMethodType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Required | `1` | Lors du rafraîchissement, utilisez les informations de connexion existantes et, si elles s'avèrent invalides, récupérez les informations de connexion mises à jour, si elles sont disponibles dans le fichier de connexion externe. |
| Always | `2` | À chaque rafraîchissement, récupérez les informations de connexion mises à jour à partir du fichier de connexion externe, si disponible, et utilisez-les à la place des informations de connexion existantes. Dans ce cas, le rafraîchissement des données échouera si le fichier de connexion externe est indisponible. |
| Never | `3` | Ne jamais récupérer les informations de connexion mises à jour à partir du fichier de connexion externe, même si celui-ci est disponible et même si les informations de connexion existantes sont invalides. |

### Exemples

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
                // Démontrer la création et l'utilisation des valeurs d'énumération ReConnectionMethodType.
                ReConnectionMethodType method1 = ReConnectionMethodType.Required;
                ReConnectionMethodType method2 = ReConnectionMethodType.Always;
                ReConnectionMethodType method3 = ReConnectionMethodType.Never;

                Console.WriteLine("ReConnectionMethodType values:");
                Console.WriteLine($"Required: {(int)method1}");
                Console.WriteLine($"Always: {(int)method2}");
                Console.WriteLine($"Never: {(int)method3}");

                // Afficher l'utilisation dans une instruction switch.
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

### Voir aussi

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


