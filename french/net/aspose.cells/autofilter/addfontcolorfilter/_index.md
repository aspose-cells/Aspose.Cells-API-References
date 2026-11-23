---
title: "AutoFilter.AddFontColorFilter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode AutoFilter. Ajoute un filtre de couleur de police"
type: docs
url: /fr/net/aspose.cells/autofilter/addfontcolorfilter/
---
## AutoFilter.AddFontColorFilter method

Ajoute un filtre de couleur de police.

```csharp
public void AddFontColorFilter(int fieldIndex, CellsColor color)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | Le décalage entier du champ sur lequel vous souhaitez baser le filtre (à partir de la gauche de la liste ; le champ le plus à gauche est le champ 0). |
| color | CellsColor | L'objet [`CellsColor`](../../cellscolor/). |

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodAddFontColorFilterWithInt32CellsColorDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple avec différentes couleurs de police
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue("Item 1");
            cells["A3"].PutValue("Item 2");
            cells["A4"].PutValue("Item 3");
            
            // Définir les couleurs de police
            Style style = cells["A2"].GetStyle();
            style.Font.Color = Color.Red;
            cells["A2"].SetStyle(style);
            
            style = cells["A3"].GetStyle();
            style.Font.Color = Color.Blue;
            cells["A3"].SetStyle(style);
            
            style = cells["A4"].GetStyle();
            style.Font.Color = Color.Green;
            cells["A4"].SetStyle(style);

            // Appliquer le filtre automatique
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Créer un filtre de couleur pour la police rouge
            CellsColor cr = workbook.CreateCellsColor();
            cr.Color = Color.Red;
            
            // Ajouter un filtre de couleur de police
            filter.AddFontColorFilter(0, cr);
            filter.Refresh();
            
            // Enregistrez le classeur
            workbook.Save("AutoFilterFontColorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CellsColor](../../cellscolor/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


