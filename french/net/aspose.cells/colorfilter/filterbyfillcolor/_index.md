---
title: "ColorFilter.FilterByFillColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ColorFilter. Indique si le filtre s'applique à la couleur de remplissage des cellules"
type: docs
url: /fr/net/aspose.cells/colorfilter/filterbyfillcolor/
---
## ColorFilter.FilterByFillColor property

Indique si le filtrage se fait par la couleur de remplissage de la cellule.

```csharp
public bool FilterByFillColor { get; set; }
```

### Remarques

Vrai : couleur de remplissage de la cellule ; Faux : couleur de police de la cellule.

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ColorFilterPropertyFilterByFillColorDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ajouter des données d'exemple avec différentes couleurs de remplissage
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue("Data1");
            cells["A3"].PutValue("Data2");
            cells["A4"].PutValue("Data3");

            // Définir les couleurs de remplissage
            Style style1 = cells["A2"].GetStyle();
            style1.ForegroundColor = Color.Red;
            style1.Pattern = BackgroundType.Solid;
            cells["A2"].SetStyle(style1);

            Style style2 = cells["A3"].GetStyle();
            style2.ForegroundColor = Color.Blue;
            style2.Pattern = BackgroundType.Solid;
            cells["A3"].SetStyle(style2);

            Style style3 = cells["A4"].GetStyle();
            style3.ForegroundColor = Color.Green;
            style3.Pattern = BackgroundType.Solid;
            cells["A4"].SetStyle(style3);

            // Appliquer le filtre automatique
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;

            // Créer un filtre de couleur pour la couleur de remplissage
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            filter.AddFillColorFilter(0, BackgroundType.Solid, color, null);
            filter.Refresh();

            // Vérifier les paramètres du filtre
            FilterColumn filterColumn = filter.FilterColumns[0];
            ColorFilter colorFilter = filterColumn.Filter as ColorFilter;
            
            // Démontrer la propriété FilterByFillColor
            Console.WriteLine("FilterByFillColor: " + colorFilter.FilterByFillColor); // Should be True
            Console.WriteLine("Filtered rows:");
            for (int row = 1; row <= 3; row++)
            {
                Console.WriteLine($"Row {row} hidden: {cells.IsRowHidden(row)}");
            }
        }
    }
}
```

### Voir aussi

* class [ColorFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


