---
title: "FilterColumn.ColorFilter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FilterColumn. Obtient le ColorFilter pour filtrer les données par couleur"
type: docs
url: /fr/net/aspose.cells/filtercolumn/colorfilter/
---
## FilterColumn.ColorFilter property

Obtient [`ColorFilter`](../../colorfilter/) pour filtrer les données par couleur.

```csharp
public ColorFilter ColorFilter { get; }
```

### Remarques

Définit [`FilterType`](../filtertype/) comme ColorFilter d'abord, sinon Null sera retourné.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyColorFilterDemo
    {
        public static void Run()
        {
            try
            {
                // Créer un nouveau classeur
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Ajouter des données d'exemple avec des couleurs
                worksheet.Cells["A1"].PutValue("Color");
                worksheet.Cells["A2"].PutValue("Red");
                worksheet.Cells["A3"].PutValue("Blue");
                worksheet.Cells["A4"].PutValue("Green");

                // Appliquer le filtre automatique
                worksheet.AutoFilter.Range = "A1:A4";

                // Obtenir la colonne de filtre
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // Accéder à la propriété ColorFilter (lecture seule)
                ColorFilter colorFilter = filterColumn.ColorFilter;

                // Afficher les propriétés du ColorFilter
                if (colorFilter != null)
                {
                    Console.WriteLine("ColorFilter is not null");
                    Console.WriteLine("FilterByFillColor: " + colorFilter.FilterByFillColor);
                }
                else
                {
                    Console.WriteLine("ColorFilter is null (no color filter applied)");
                }

                // Enregistrez le classeur
                workbook.Save("ColorFilterDemo.xlsx");
                Console.WriteLine("ColorFilter demonstration completed successfully.");
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

* class [ColorFilter](../../colorfilter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


