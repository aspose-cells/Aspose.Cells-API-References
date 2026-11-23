---
title: "Classe ColorFilter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.ColorFilter. Représente le paramètre de filtrage de la plage par couleur"
type: docs
url: /fr/net/aspose.cells/colorfilter/
---
## ColorFilter class

Représente le paramètre de filtrage de la plage par couleur.

```csharp
public class ColorFilter
```

## Propriétés

| Nom | Description |
| --- | --- |
| [FilterByFillColor](../../aspose.cells/colorfilter/filterbyfillcolor/) { get; set; } | Indique si le filtrage se fait par la couleur de remplissage de la cellule. |

## Méthodes

| Nom | Description |
| --- | --- |
| [GetColor](../../aspose.cells/colorfilter/getcolor/)(WorksheetCollection) | Obtient la couleur de ce filtre. |

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassColorFilterDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple avec différentes couleurs
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Red");
            cells["A2"].PutValue("Green");
            cells["A3"].PutValue("Blue");
            cells["A4"].PutValue("Red");
            
            // Appliquez des couleurs aux cellules
            Style style1 = workbook.CreateStyle();
            style1.ForegroundColor = Color.Red;
            style1.Pattern = BackgroundType.Solid;
            cells["A1"].SetStyle(style1);
            cells["A4"].SetStyle(style1);
            
            Style style2 = workbook.CreateStyle();
            style2.ForegroundColor = Color.Green;
            style2.Pattern = BackgroundType.Solid;
            cells["A2"].SetStyle(style2);
            
            Style style3 = workbook.CreateStyle();
            style3.ForegroundColor = Color.Blue;
            style3.Pattern = BackgroundType.Solid;
            cells["A3"].SetStyle(style3);
            
            // Créez un filtre automatique
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Créez un filtre de couleur pour les cellules rouges
            CellsColor cr = workbook.CreateCellsColor();
            cr.Color = Color.Red;
            filter.AddFillColorFilter(0, BackgroundType.Solid, cr, cr);
            filter.Refresh();
            
            // Vérifiez les lignes filtrées
            Console.WriteLine("Row 1 hidden: " + cells.IsRowHidden(0));
            Console.WriteLine("Row 2 hidden: " + cells.IsRowHidden(1));
            Console.WriteLine("Row 3 hidden: " + cells.IsRowHidden(2));
            Console.WriteLine("Row 4 hidden: " + cells.IsRowHidden(3));
            
            // Accédez au filtre de couleur
            FilterColumn fc = filter.FilterColumns[0];
            ColorFilter cf = fc.Filter as ColorFilter;
            
            Console.WriteLine("Filter by fill color: " + cf.FilterByFillColor);
            Console.WriteLine("Filter color: " + cf.GetColor(workbook.Worksheets));
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


