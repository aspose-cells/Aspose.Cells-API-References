---
title: "Workbook.DataConnections"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Workbook. Obtient la collection ExternalConnection"
type: docs
url: /fr/net/aspose.cells/workbook/dataconnections/
---
## Workbook.DataConnections property

Obtient la collection [`ExternalConnection`](../../../aspose.cells.externalconnections/externalconnection/).

```csharp
public ExternalConnectionCollection DataConnections { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookPropertyDataConnectionsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Créer une feuille de calcul d’exemple
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données pour rendre l’exemple significatif
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Accéder à la propriété DataConnections
                var dataConnections = workbook.DataConnections;

                // Afficher la valeur actuelle de la propriété (opération de lecture)
                Console.WriteLine("DataConnections count: " + dataConnections.Count);

                // Itérer à travers les connexions si elles existent
                for (int i = 0; i < dataConnections.Count; i++)
                {
                    var connection = dataConnections[i];
                    Console.WriteLine($"Connection {i + 1}: {connection.Name}");
                }

                // Afficher comment la propriété affecte le comportement
                Console.WriteLine("DataConnections has been demonstrated");

                // Enregistrer le résultat
                workbook.Save("DataConnectionsDemo.xlsx");
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

* class [ExternalConnectionCollection](../../../aspose.cells.externalconnections/externalconnectioncollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


