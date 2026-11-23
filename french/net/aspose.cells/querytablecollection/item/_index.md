---
title: "QueryTableCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété QueryTableCollection. Obtient la table de requête par l'index spécifique"
type: docs
url: /fr/net/aspose.cells/querytablecollection/item/
---
## QueryTableCollection indexer

Obtient la querytable à l'index spécifié.

```csharp
public QueryTable this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice. |

### Valeur de retour

La table de requête

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTableCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Accéder à la QueryTableCollection
            QueryTableCollection queryTables = worksheet.QueryTables;

            try
            {
                // Vérifier s'il existe des QueryTables
                if (queryTables.Count > 0)
                {
                    // Accéder à la première QueryTable en utilisant la propriété Item
                    QueryTable firstQueryTable = queryTables[0];
                    Console.WriteLine("First QueryTable accessed successfully.");

                    // Afficher certaines propriétés de la QueryTable
                    Console.WriteLine("QueryTable Name: " + firstQueryTable.Name);
                }
                else
                {
                    Console.WriteLine("No QueryTables found in the worksheet.");
                }

                // Enregistrez le classeur
                workbook.Save("QueryTableItemDemo.xlsx");
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

* class [QueryTable](../../querytable/)
* class [QueryTableCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


