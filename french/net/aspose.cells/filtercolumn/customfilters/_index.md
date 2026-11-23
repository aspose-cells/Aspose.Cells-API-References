---
title: "FilterColumn.CustomFilters"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FilterColumn. Obtient CustomFilterCollection pour filtrer les données selon des critères personnalisés"
type: docs
url: /fr/net/aspose.cells/filtercolumn/customfilters/
---
## FilterColumn.CustomFilters property

Obtient [`CustomFilterCollection`](../../customfiltercollection/) pour filtrer les données selon des critères personnalisés.

```csharp
public CustomFilterCollection CustomFilters { get; set; }
```

### Remarques

NOTE : Ce mutateur de cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété [`FilterType`](../filtertype/) en la définissant sur CustomFilters. Cette propriété sera supprimée 12 mois après juin 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyCustomFiltersDemo
    {
        public static void Run()
        {
            try
            {
                // Créer un nouveau classeur
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Ajoutez des données d'exemple
                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["A3"].PutValue("Banana");
                worksheet.Cells["A4"].PutValue("Cherry");
                worksheet.Cells["A5"].PutValue("Date");
                worksheet.Cells["A6"].PutValue("Elderberry");

                // Appliquer le filtre automatique
                worksheet.AutoFilter.Range = "A1:A6";

                // Obtenir la colonne de filtre
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // Créer et définir des filtres personnalisés en utilisant la méthode AutoFilter.Custom
                // Premier filtre : commence par "A"
                worksheet.AutoFilter.Custom(0, FilterOperatorType.BeginsWith, "A", false, FilterOperatorType.None, null);

                // Deuxième filtre : se termine par "y" (relation AND)
                worksheet.AutoFilter.Custom(0, FilterOperatorType.EndsWith, "y", true, FilterOperatorType.None, null);

                // Obtenir les filtres personnalisés de la colonne de filtre
                CustomFilterCollection customFilters = filterColumn.CustomFilters;

                // Afficher les informations des filtres personnalisés
                Console.WriteLine($"Number of custom filters: {customFilters.Count}");
                Console.WriteLine($"Filter relationship (And): {customFilters.And}");

                // Note : CustomFilterCollection n'expose pas les filtres individuels directement
                // via un indexeur, nous ne pouvons donc afficher que les propriétés de la collection
                Console.WriteLine("Custom filters have been applied to the column.");

                // Enregistrez le classeur
                workbook.Save("CustomFiltersDemo.xlsx");
                Console.WriteLine("CustomFilters demonstration completed successfully.");
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

* class [CustomFilterCollection](../../customfiltercollection/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


