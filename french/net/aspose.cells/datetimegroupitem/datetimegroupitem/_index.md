---
title: "DateTimeGroupItem.DateTimeGroupItem"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur DateTimeGroupItem."
type: docs
url: /fr/net/aspose.cells/datetimegroupitem/datetimegroupitem/
---
## DateTimeGroupItem constructor

```csharp
public DateTimeGroupItem(DateTimeGroupingType type, int year, int month, int day, int hour, 
    int minute, int second)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | DateTimeGroupingType |  |
| année | Int32 |  |
| mois | Int32 |  |
| jour | Int32 |  |
| heure | Int32 |  |
| minute | Int32 |  |
| seconde | Int32 |  |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DateTimeGroupItemMethodCtorWithDateTimeGroupingTypeInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur et accéder à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données datetime d'exemple à la colonne A
            worksheet.Cells["A1"].PutValue("Order Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 3, 15, 9, 30, 15));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 4, 20, 14, 15, 45));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 25, 10, 0, 0));
            worksheet.Cells["A5"].PutValue(new DateTime(2024, 3, 1, 8, 45, 30));

            // Appliquer le filtre automatique à la colonne de dates
            worksheet.AutoFilter.Range = "A1:A5";

            try
            {
                // Créer un DateTimeGroupItem pour le groupement de mars 2023
                DateTimeGroupItem groupItem = new DateTimeGroupItem(
                    DateTimeGroupingType.Month, // Group by Month
                    2023,   // Year
                    3,      // Month (March)
                    1,      // Day (ignored in Month grouping)
                    0,      // Hour
                    0,      // Minute
                    0       // Second
                );

                // Configurer le filtre pour afficher les dates de mars 2023
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
                filterColumn.FilterType = FilterType.MultipleFilters;
                filterColumn.Filter = groupItem;

                // Actualiser le filtre pour appliquer les modifications
                worksheet.AutoFilter.Refresh();

                Console.WriteLine("DateTimeGroupItem created and filter applied successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error applying date filter: {ex.Message}");
            }

            // Enregistrer le classeur filtré
            workbook.Save("DateTimeGroupItemConstructorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [DateTimeGroupingType](../../datetimegroupingtype/)
* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


