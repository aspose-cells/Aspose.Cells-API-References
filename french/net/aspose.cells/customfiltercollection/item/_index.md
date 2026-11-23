---
title: "CustomFilterCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CustomFilterCollection. Obtient le filtre personnalisé à l'indice spécifié"
type: docs
url: /fr/net/aspose.cells/customfiltercollection/item/
---
## CustomFilterCollection indexer

Obtient le filtre personnalisé à l'index spécifié.

```csharp
public CustomFilter this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFilterCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].Value = "Numbers";
            worksheet.Cells["A2"].Value = 10;
            worksheet.Cells["A3"].Value = 20;
            worksheet.Cells["A4"].Value = 30;
            worksheet.Cells["A5"].Value = 40;
            worksheet.Cells["A6"].Value = 50;

            try
            {
                // Créer une nouvelle CustomFilterCollection
                CustomFilterCollection filters = new CustomFilterCollection();

                // Accédez à la propriété Item (lecture seule) à l'aide de l'indexeur
                // Comme la collection est vide, nous allons simplement démontrer l'accès à la propriété
                // Dans un scénario réel, vous ajouteriez d'abord des filtres par d'autres moyens
                if (filters.Count > 0)
                {
                    CustomFilter firstFilter = filters[0];
                    Console.WriteLine($"First filter operator: {firstFilter.FilterOperatorType}");
                    Console.WriteLine($"First filter criteria: {firstFilter.Criteria}");
                }
                else
                {
                    Console.WriteLine("No filters in collection to demonstrate Item property");
                }

                // Enregistrez le classeur
                workbook.Save("CustomFilterCollectionItemDemo.xlsx");
                Console.WriteLine("CustomFilterCollection Item property demonstrated successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating Item property: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [CustomFilter](../../customfilter/)
* class [CustomFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


