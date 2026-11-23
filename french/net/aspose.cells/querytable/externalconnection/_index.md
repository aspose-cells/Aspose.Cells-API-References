---
title: "QueryTable.ExternalConnection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété QueryTable. Obtient la connexion externe associée"
type: docs
url: /fr/net/aspose.cells/querytable/externalconnection/
---
## QueryTable.ExternalConnection property

Obtient la connexion externe associée.

```csharp
public ExternalConnection ExternalConnection { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class QueryTablePropertyExternalConnectionDemo
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

                    // Accéder à la propriété ExternalConnection (lecture seule)
                    ExternalConnection externalConnection = queryTable.ExternalConnection;

                    // Afficher les informations sur la connexion externe
                    if (externalConnection != null)
                    {
                        Console.WriteLine("External Connection ID: " + externalConnection.Id);
                        Console.WriteLine("External Connection Name: " + externalConnection.Name);
                        Console.WriteLine("External Connection Type: " + externalConnection.ClassType);
                        Console.WriteLine("Connection String: " + externalConnection.ConnectionString);
                        Console.WriteLine("Refresh on Load: " + externalConnection.RefreshOnLoad);
                    }
                    else
                    {
                        Console.WriteLine("No external connection associated with this query table.");
                    }

                    // Afficher d'autres propriétés du tableau de requête pour le contexte
                    Console.WriteLine("Query Table Name: " + queryTable.Name);
                    Console.WriteLine("Connection ID: " + queryTable.ConnectionId);
                }
                else
                {
                    Console.WriteLine("No query tables found in the worksheet.");
                }

                // Enregistrez le classeur
                workbook.Save("ExternalConnectionDemo.xlsx");
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

* class [ExternalConnection](../../../aspose.cells.externalconnections/externalconnection/)
* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


