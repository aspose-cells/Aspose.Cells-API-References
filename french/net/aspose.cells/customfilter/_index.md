---
title: "Classe CustomFilter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.CustomFilter class. Représente le filtre personnalisé"
type: docs
url: /fr/net/aspose.cells/customfilter/
---
## CustomFilter class

Représente le filtre personnalisé.

```csharp
public class CustomFilter
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Criteria](../../aspose.cells/customfilter/criteria/) { get; set; } | Obtient et définit les critères. |
| [FilterOperatorType](../../aspose.cells/customfilter/filteroperatortype/) { get; set; } | Obtient et définit le type d'opérateur de filtre. |

## Méthodes

| Nom | Description |
| --- | --- |
| [SetCriteria](../../aspose.cells/customfilter/setcriteria/)(FilterOperatorType, object) | Définit les critères du filtre. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassCustomFilterDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Ajouter des données d'exemple à la feuille de calcul
                worksheet.Cells["A1"].PutValue("Values");
                worksheet.Cells["A2"].PutValue(10);
                worksheet.Cells["A3"].PutValue(20);
                worksheet.Cells["A4"].PutValue(30);
                worksheet.Cells["A5"].PutValue(40);

                // Applique le filtre automatique à la plage
                worksheet.AutoFilter.Range = "A1:A5";
                AutoFilter filter = worksheet.AutoFilter;

                // Appliquez un filtre personnalisé pour obtenir une instance CustomFilter
                filter.Custom(0, FilterOperatorType.GreaterThan, 25);

                // Obtenez le premier filtre personnalisé de la collection de filtres
                CustomFilter customFilter = ((CustomFilterCollection)filter.FilterColumns[0].Filter)[0];

                // Affichez les propriétés du filtre
                Console.WriteLine("Filter Operator: " + customFilter.FilterOperatorType);
                Console.WriteLine("Criteria Value: " + customFilter.Criteria);

                // Modifiez les critères du filtre en utilisant la méthode SetCriteria
                customFilter.SetCriteria(FilterOperatorType.LessThan, 35);

                // Affichez les propriétés du filtre mises à jour
                Console.WriteLine("Updated Filter Operator: " + customFilter.FilterOperatorType);
                Console.WriteLine("Updated Criteria Value: " + customFilter.Criteria);

                // Enregistrez le classeur
                workbook.Save("CustomFilterDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with CustomFilter: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


