---
title: "DynamicFilter.DynamicFilterType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DynamicFilter. Obtient et définit le type de ce filtre dynamique"
type: docs
url: /fr/net/aspose.cells/dynamicfilter/dynamicfiltertype/
---
## DynamicFilter.DynamicFilterType property

Obtient et définit le type de ce filtre dynamique.

```csharp
public DynamicFilterType DynamicFilterType { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DynamicFilterPropertyDynamicFilterTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple avec des dates
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 15));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 20));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 10));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 4, 5));

            try
            {
                // Créez un filtre automatique
                worksheet.AutoFilter.Range = "A1:A5";

                // Appliquer le filtre dynamique pour les dates de mars
                worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.March);

                // Obtenir l'instance DynamicFilter
                DynamicFilter filter = (DynamicFilter)worksheet.AutoFilter.FilterColumns[0].Filter;

                // Afficher la valeur actuelle de DynamicFilterType
                Console.WriteLine("Current DynamicFilterType: " + filter.DynamicFilterType);

                // Modifier le type de filtre pour afficher les dates d'avril
                filter.DynamicFilterType = DynamicFilterType.April;

                // Afficher la valeur mise à jour de DynamicFilterType
                Console.WriteLine("Updated DynamicFilterType: " + filter.DynamicFilterType);

                // Appliquer le filtre
                worksheet.AutoFilter.Refresh();

                // Enregistrer le résultat
                workbook.Save("DynamicFilterTypeDemo.xlsx");
                Console.WriteLine("DynamicFilterType has been demonstrated successfully.");
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

* enum [DynamicFilterType](../../dynamicfiltertype/)
* class [DynamicFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


