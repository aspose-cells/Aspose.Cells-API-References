---
title: "ColorFilter.GetColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ColorFilter. Obtient la couleur de ce filtre"
type: docs
url: /fr/net/aspose.cells/colorfilter/getcolor/
---
## ColorFilter.GetColor method

Obtient la couleur de ce filtre.

```csharp
public Color GetColor(WorksheetCollection sheets)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| feuilles | WorksheetCollection |  |

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ColorFilterMethodGetColorWithWorksheetCollectionDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["A4"].PutValue("Item 3");
            
            // Créez un filtre automatique
            worksheet.AutoFilter.Range = "A1:A4";
            
            // Créer un filtre de couleur
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            worksheet.AutoFilter.AddFillColorFilter(0, BackgroundType.Solid, color, color);
            worksheet.AutoFilter.Refresh();
            
            // Obtenir le filtre de couleur et vérifier sa couleur
            FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
            ColorFilter colorFilter = filterColumn.Filter as ColorFilter;
            
            if (colorFilter != null)
            {
                Color retrievedColor = colorFilter.GetColor(workbook.Worksheets);
                Console.WriteLine("Filter color: " + retrievedColor.ToString());
            }
        }
    }
}
```

### Voir aussi

* class [WorksheetCollection](../../worksheetcollection/)
* class [ColorFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


