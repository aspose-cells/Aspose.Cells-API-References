---
title: "Classe AdvancedFilter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.AdvancedFilter. Représente les paramètres du filtre avancé"
type: docs
url: /fr/net/aspose.cells/advancedfilter/
---
## AdvancedFilter class

Représente les paramètres du filtre avancé.

```csharp
public class AdvancedFilter
```

## Propriétés

| Nom | Description |
| --- | --- |
| [CopyToRange](../../aspose.cells/advancedfilter/copytorange/) { get; } | Obtient la plage où copier le résultat de ce filtre avancé. |
| [CriteriaRange](../../aspose.cells/advancedfilter/criteriarange/) { get; } | Obtient la plage de critères de ce filtre avancé. |
| [ListRange](../../aspose.cells/advancedfilter/listrange/) { get; } | Obtient la plage de la liste de ce filtre avancé. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassAdvancedFilterDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Remplissez les données d'exemple pour la plage de la liste
                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["B1"].PutValue("Price");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["B2"].PutValue(1.5);
                worksheet.Cells["A3"].PutValue("Banana");
                worksheet.Cells["B3"].PutValue(0.8);
                worksheet.Cells["A4"].PutValue("Orange");
                worksheet.Cells["B4"].PutValue(1.2);

                // Remplissez la plage de critères
                worksheet.Cells["D1"].PutValue("Product");
                worksheet.Cells["D2"].PutValue("Apple");

                // Obtenez l'instance AdvancedFilter de la feuille de calcul
                AdvancedFilter advancedFilter = worksheet.GetAdvancedFilter();

                // Affichez les propriétés en lecture seule
                Console.WriteLine("List Range: " + advancedFilter.ListRange);
                Console.WriteLine("Criteria Range: " + advancedFilter.CriteriaRange);
                Console.WriteLine("Copy To Range: " + advancedFilter.CopyToRange);

                // Enregistrez le classeur
                workbook.Save("AdvancedFilterDemo.xlsx");
                Console.WriteLine("AdvancedFilter demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in AdvancedFilter demonstration: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


