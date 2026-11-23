---
title: "FilterColumn.Filter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FilterColumn. Obtient et définit la condition de filtrage des données"
type: docs
url: /fr/net/aspose.cells/filtercolumn/filter/
---
## FilterColumn.Filter property

Obtient et définit la condition de filtrage des données.

```csharp
[Obsolete("Use corresponding property according to the filter type instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public object Filter { get; set; }
```

### Remarques

NOTE : Ce membre est maintenant obsolète. A la place, veuillez utiliser la propriété correspondante selon [`FilterType`](../filtertype/). Et pour le type de filtre MultipleFilters, l'objet retourné est désormais [`FilterValueCollection`](../../filtervaluecollection/) au lieu de [`MultipleFilterCollection`](../../multiplefiltercollection/). Cette propriété sera supprimée 12 mois plus tard, a compter d'octobre 2025. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyFilterDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple avec un formatage de couleur
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Color");
            cells["A2"].PutValue("Red");
            cells["A3"].PutValue("Red");
            cells["A4"].PutValue("Blue");
            
            // Formater les cellules avec des couleurs
            Style redStyle = workbook.CreateStyle();
            redStyle.ForegroundColor = Color.Red;
            redStyle.Pattern = BackgroundType.Solid;
            
            Style blueStyle = workbook.CreateStyle();
            blueStyle.ForegroundColor = Color.Blue;
            blueStyle.Pattern = BackgroundType.Solid;
            
            cells["A2"].SetStyle(redStyle);
            cells["A3"].SetStyle(redStyle);
            cells["A4"].SetStyle(blueStyle);
            
            // Appliquer le filtre automatique
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Ajouter un filtre de couleur pour les cellules rouges
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            filter.AddFillColorFilter(0, BackgroundType.Solid, color, color);
            filter.Refresh();
            
            // Accéder à la colonne de filtre et à sa propriété Filter
            FilterColumn fc = filter.FilterColumns[0];
            ColorFilter cf = fc.Filter as ColorFilter;
            
            // Afficher les propriétés du filtre
            Console.WriteLine($"Filter type: {fc.FilterType}");
            Console.WriteLine($"Filter by fill color: {cf.FilterByFillColor}");
            Console.WriteLine($"Filter color: {cf.GetColor(workbook.Worksheets)}");
            
            // Enregistrez le classeur
            workbook.Save("ColorFilterDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


