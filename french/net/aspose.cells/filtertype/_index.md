---
title: "Énumération FilterType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.FilterType enum. Le type de filtre"
type: docs
url: /fr/net/aspose.cells/filtertype/
---
## FilterType enumeration

Le type de filtre.

```csharp
public enum FilterType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| ColorFilter | `0` | Filtrer par couleur de remplissage de la cellule. |
| CustomFilters | `1` | Type de filtre personnalisé. |
| DynamicFilter | `2` | Type de filtre dynamique. |
| MultipleFilters | `3` | Lorsque plusieurs valeurs sont sélectionnées pour filtrer, ou lorsqu'un groupe de valeurs de date est sélectionné pour filtrer, cet élément regroupe ces critères ensemble. |
| IconFilter | `4` | Filtrer par icône du formatage conditionnel. |
| Top10 | `5` | Filtre Top 10. |
| None | `6` | Pas de filtre. |

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFilterTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Color");
            worksheet.Cells["A2"].PutValue("Red");
            worksheet.Cells["A3"].PutValue("Green");
            worksheet.Cells["A4"].PutValue("Blue");
            
            // Créez un filtre automatique
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Créer un filtre de couleur
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            
            // Ajouter un filtre de couleur à la colonne
            filter.AddFillColorFilter(0, BackgroundType.Solid, color, color);
            filter.Refresh();
            
            // Vérifier le type de filtre
            FilterColumn filterColumn = filter.FilterColumns[0];
            Console.WriteLine("Filter Type: " + filterColumn.FilterType);
            
            // Vérifier les propriétés du filtre de couleur
            if (filterColumn.FilterType == FilterType.ColorFilter)
            {
                ColorFilter colorFilter = filterColumn.Filter as ColorFilter;
                Console.WriteLine("Filter by fill color: " + colorFilter.FilterByFillColor);
                Console.WriteLine("Filter color: " + colorFilter.GetColor(workbook.Worksheets));
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


