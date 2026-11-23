---
title: "FilterColumn.DynamicFilter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FilterColumn. Obtient DynamicFilter pour filtrer avec des critères dynamiques"
type: docs
url: /fr/net/aspose.cells/filtercolumn/dynamicfilter/
---
## FilterColumn.DynamicFilter property

Obtient `DynamicFilter` pour filtrer avec des critères dynamiques.

```csharp
public DynamicFilter DynamicFilter { get; }
```

### Remarques

Avant d'utiliser cette propriété, veuillez vous assurer que [`FilterType`](../filtertype/) est DynamicFilter, sinon null sera retourné.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyDynamicFilterDemo
    {
        public static void Run()
        {
            try
            {
                // Créer un nouveau classeur
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Ajoutez des données d'exemple
                worksheet.Cells["A1"].PutValue("Date");
                worksheet.Cells["A2"].PutValue(DateTime.Now.AddDays(-10));
                worksheet.Cells["A3"].PutValue(DateTime.Now.AddDays(-5));
                worksheet.Cells["A4"].PutValue(DateTime.Now);

                // Appliquer le filtre automatique
                worksheet.AutoFilter.Range = "A1:A4";

                // Obtenir la colonne de filtre
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // Accéder à la propriété DynamicFilter (lecture seule)
                DynamicFilter dynamicFilter = filterColumn.DynamicFilter;

                // Afficher les propriétés DynamicFilter
                if (dynamicFilter != null)
                {
                    Console.WriteLine("DynamicFilter is not null");
                    Console.WriteLine("DynamicFilterType: " + dynamicFilter.DynamicFilterType);
                    Console.WriteLine("Value: " + dynamicFilter.Value);
                    Console.WriteLine("MaxValue: " + dynamicFilter.MaxValue);
                }
                else
                {
                    Console.WriteLine("DynamicFilter is null (no dynamic filter applied)");
                }

                // Enregistrez le classeur
                workbook.Save("DynamicFilterDemo.xlsx");
                Console.WriteLine("DynamicFilter demonstration completed successfully.");
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

* class [DynamicFilter](../../dynamicfilter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


