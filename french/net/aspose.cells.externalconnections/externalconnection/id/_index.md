---
title: "ExternalConnection.Id"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExternalConnection. Obtient l’identifiant de la connexion"
type: docs
url: /fr/net/aspose.cells.externalconnections/externalconnection/id/
---
## ExternalConnection.Id property

Obtient l’identifiant de la connexion.

```csharp
public int Id { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyIdDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            try
            {
                // Accéder à la première connexion externe (le classeur est fourni avec des connexions par défaut)
                ExternalConnection connection = workbook.DataConnections[0];

                // Afficher la valeur actuelle de Id (propriété en lecture seule)
                Console.WriteLine("External Connection Id: " + connection.Id);

                // Afficher d'autres propriétés en lecture seule pour le contexte
                Console.WriteLine("Connection Class Type: " + connection.ClassType);
                Console.WriteLine("Connection Name: " + connection.Name);

                // Enregistrez le classeur
                workbook.Save("ExternalConnectionIdDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with connection Id: " + connection.Id);
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


