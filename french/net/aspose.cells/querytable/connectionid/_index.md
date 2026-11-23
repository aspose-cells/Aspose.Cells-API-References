---
title: "QueryTable.ConnectionId"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété QueryTable. Obtient l'identifiant de connexion du tableau de requête"
type: docs
url: /fr/net/aspose.cells/querytable/connectionid/
---
## QueryTable.ConnectionId property

Obtient l'identifiant de connexion de la table de requête.

```csharp
public int ConnectionId { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyConnectionIdDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour simuler un scénario de tableau de requête
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Sample Data");

            try
            {
                // Vérifiez s'il existe des tables de requête dans la feuille de calcul
                if (worksheet.QueryTables.Count > 0)
                {
                    // Obtenez la première table de requête
                    QueryTable queryTable = worksheet.QueryTables[0];

                    // Afficher la valeur de la propriété ConnectionId (lecture seule)
                    Console.WriteLine("Query Table ConnectionId: " + queryTable.ConnectionId);

                    // Afficher d'autres propriétés associées pour le contexte
                    Console.WriteLine("Query Table Name: " + queryTable.Name);
                    Console.WriteLine("External Connection: " +
                        (queryTable.ExternalConnection != null ? queryTable.ExternalConnection.Name : "None"));
                }
                else
                {
                    Console.WriteLine("No query tables found in the worksheet.");
                }

                // Enregistrez le classeur
                workbook.Save("ConnectionIdDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


