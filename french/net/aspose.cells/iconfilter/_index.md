---
title: "Classe IconFilter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.IconFilter. Représente le filtre d'icône"
type: docs
url: /fr/net/aspose.cells/iconfilter/
---
## IconFilter class

Représente le filtre d'icônes.

```csharp
public class IconFilter
```

## Propriétés

| Nom | Description |
| --- | --- |
| [IconId](../../aspose.cells/iconfilter/iconid/) { get; set; } | Obtient et définit l'index basé sur zéro d'une icône dans un jeu d'icônes. |
| [IconSetType](../../aspose.cells/iconfilter/iconsettype/) { get; set; } | Obtient et définit quel jeu d'icônes est utilisé pour ce critère de filtre. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassIconFilterDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Remplissez des données d'exemple
                for (int i = 0; i < 10; i++)
                {
                    worksheet.Cells[i, 0].PutValue(i * 10);
                }

                // Créez un filtre automatique
                worksheet.AutoFilter.Range = "A1:A10";
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
                filterColumn.FilterType = FilterType.IconFilter;

                // Obtenez le filtre d'icône
                IconFilter iconFilter = (IconFilter)filterColumn.Filter;

                // Définir les propriétés du filtre d'icône
                iconFilter.IconSetType = IconSetType.Arrows3;
                iconFilter.IconId = 1; // Filter for middle arrow

                Console.WriteLine($"IconFilter created with IconSetType: {iconFilter.IconSetType} and IconId: {iconFilter.IconId}");

                // Enregistrez le classeur
                workbook.Save("IconFilterDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with icon filter applied.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with IconFilter: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


