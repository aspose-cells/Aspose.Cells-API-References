---
title: "ExternalConnection.ConnectionId"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExternalConnection. Spécifie l'identifiant unique de cette connexion"
type: docs
url: /fr/net/aspose.cells.externalconnections/externalconnection/connectionid/
---
## ExternalConnection.ConnectionId property

Spécifie l'identifiant unique de cette connexion.

```csharp
[Obsolete("Use ExternalConnection.Id property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int ConnectionId { get; }
```

### Remarques

NOTE: Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété ExternalConnection.Id. Cette propriété sera supprimée 12 mois plus tard depuis octobre 2024. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyConnectionIdDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            try
            {
                // Accéder à la première connexion externe (le classeur est fourni avec des connexions par défaut)
                ExternalConnection connection = workbook.DataConnections[0];

                // Afficher la valeur ConnectionId (propriété en lecture seule)
                Console.WriteLine("ConnectionId value: " + connection.ConnectionId);

                // Afficher la valeur Id pour comparaison (également en lecture seule)
                Console.WriteLine("Id value: " + connection.Id);

                // Montrer que les deux propriétés sont en lecture seule en essayant de les afficher
                Console.WriteLine("ConnectionId and Id are both read-only properties");
                Console.WriteLine("ConnectionId: " + connection.ConnectionId + ", Id: " + connection.Id);

                // Enregistrez le classeur
                workbook.Save("ConnectionIdDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


