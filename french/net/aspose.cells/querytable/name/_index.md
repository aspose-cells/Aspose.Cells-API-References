---
title: "QueryTable.Name"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété QueryTable. Obtient le nom du QueryTable"
type: docs
url: /fr/net/aspose.cells/querytable/name/
---
## QueryTable.Name property

Obtient le nom de la querytable.

```csharp
public string Name { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d’exemple pour simuler une table de requête
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");

            try
            {
                // Vérifiez s'il existe des tables de requête dans la feuille de calcul
                if (worksheet.QueryTables.Count > 0)
                {
                    // Obtenez la première table de requête
                    QueryTable queryTable = worksheet.QueryTables[0];

                    // Afficher la valeur de la propriété Name (opération en lecture seule)
                    Console.WriteLine("Query Table Name: " + queryTable.Name);

                    // Afficher d'autres propriétés en lecture seule pour le contexte
                    Console.WriteLine("Connection ID: " + queryTable.ConnectionId);
                    Console.WriteLine("Result Range: " + queryTable.ResultRange.Address);
                }
                else
                {
                    Console.WriteLine("No query tables found in the worksheet.");
                }

                // Enregistrez le classeur
                workbook.Save("QueryTableNameDemo.xlsx");
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


