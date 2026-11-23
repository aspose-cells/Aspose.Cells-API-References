---
title: "Enum ConnectionParameterType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.ExternalConnections.ConnectionParameterType enum. Spécifie le type de paramètre de la connexion externe."
type: docs
url: /fr/net/aspose.cells.externalconnections/connectionparametertype/
---
## ConnectionParameterType enumeration

Spécifie le type de paramètre de la connexion externe

```csharp
public enum ConnectionParameterType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Cell | `0` | Obtenez la valeur du paramètre à partir d'une cellule à chaque rafraîchissement. |
| Prompt | `1` | Invite l'utilisateur à chaque rafraîchissement à fournir une valeur de paramètre. |
| Value | `2` | Utilisez une valeur constante à chaque rafraîchissement pour la valeur du paramètre. |

### Exemples

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
                // Démontrer la création et l'utilisation des valeurs d'énumération ConnectionParameterType.
                ConnectionParameterType cellParam = ConnectionParameterType.Cell;
                ConnectionParameterType promptParam = ConnectionParameterType.Prompt;
                ConnectionParameterType valueParam = ConnectionParameterType.Value;

                // Afficher les valeurs d'énumération
                Console.WriteLine("Connection Parameter Types:");
                Console.WriteLine($"Cell: {cellParam}");
                Console.WriteLine($"Prompt: {promptParam}");
                Console.WriteLine($"Value: {valueParam}");

                // Démontrer l'utilisation dans une instruction switch.
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

### Voir aussi

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


