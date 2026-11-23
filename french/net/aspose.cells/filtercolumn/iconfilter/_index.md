---
title: "FilterColumn.IconFilter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FilterColumn. Obtient IconFilter pour filtrer les données par icône"
type: docs
url: /fr/net/aspose.cells/filtercolumn/iconfilter/
---
## FilterColumn.IconFilter property

Obtient `IconFilter` pour filtrer les données par icône.

```csharp
public IconFilter IconFilter { get; }
```

### Remarques

Avant d'utiliser cette propriété, veuillez vous assurer que [`FilterType`](../filtertype/) est IconFilter, sinon null sera renvoyé.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyIconFilterDemo
    {
        public static void Run()
        {
            try
            {
                // Créer un nouveau classeur
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Ajouter des données d'exemple avec un format conditionnel utilisant des icônes
                worksheet.Cells["A1"].PutValue("Performance");
                worksheet.Cells["A2"].PutValue(85);
                worksheet.Cells["A3"].PutValue(72);
                worksheet.Cells["A4"].PutValue(93);
                worksheet.Cells["A5"].PutValue(65);

                // Applique le filtre automatique à la plage
                worksheet.AutoFilter.Range = "A1:A5";

                // Obtenir la colonne de filtre
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // Accéder à la propriété IconFilter (lecture seule)
                IconFilter iconFilter = filterColumn.IconFilter;

                // Afficher les propriétés d'IconFilter si elles existent
                if (iconFilter != null)
                {
                    Console.WriteLine("IconFilter is available");
                    Console.WriteLine($"IconSetType: {iconFilter.IconSetType}");
                    Console.WriteLine($"IconId: {iconFilter.IconId}");
                }
                else
                {
                    Console.WriteLine("No IconFilter is currently applied to this column");
                }

                // Enregistrez le classeur
                workbook.Save("IconFilterDemo.xlsx");
                Console.WriteLine("IconFilter demonstration completed successfully.");
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

* class [IconFilter](../../iconfilter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


