---
title: "Enumération TextureType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.Drawing.TextureType. Représente le type de texture prédéfini"
type: docs
url: /fr/net/aspose.cells.drawing/texturetype/
---
## TextureType enumeration

Représente le type de texture prédéfini.

```csharp
public enum TextureType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| BlueTissuePaper | `0` | Représente le type de texture Blue Tissue Paper. |
| Bouquet | `1` | Représente le type de texture Bouquet. |
| BrownMarble | `2` | Représente le type de texture Brown Marble. |
| Canvas | `3` | Représente le type de texture Canvas. |
| Cork | `4` | Représente le type de texture Cork. |
| Denim | `5` | Représente le type de texture Denim. |
| FishFossil | `6` | Représente le type de texture Fish Fossil. |
| Granite | `7` | Représente le type de texture Granite. |
| GreenMarble | `8` | Représente le type de texture Green Marble. |
| MediumWood | `9` | Représente le type de texture Medium Wood. |
| Newsprint | `10` | Représente le type de texture Newsprint. |
| Oak | `11` | Représente le type de texture Oak. |
| PaperBag | `12` | Représente le type de texture Paper Bag. |
| Papyrus | `13` | Représente le type de texture Papyrus. |
| Parchment | `14` | Représente le type de texture Parchment. |
| PinkTissuePaper | `15` | Représente le type de texture Pink Tissue Paper. |
| PurpleMesh | `16` | Représente le type de texture Purple Mesh. |
| RecycledPaper | `17` | Représente le type de texture Recycled Paper. |
| Sand | `18` | Représente le type de texture Sand. |
| Stationery | `19` | Représente le type de texture Stationery. |
| Walnut | `20` | Représente le type de texture Walnut Droplets. |
| WaterDroplets | `21` | Représente le type de texture Water Droplets. |
| WhiteMarble | `22` | Représente le type de texture White Marble. |
| WovenMat | `23` | Représente le type de texture Woven Mat. |
| Unknown | `24` | Représente le type de texture Unknown. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassTextureTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            sheet.Cells["A1"].PutValue("Item");
            sheet.Cells["A2"].PutValue("Product A");
            sheet.Cells["A3"].PutValue("Product B");
            sheet.Cells["A4"].PutValue("Product C");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["B4"].PutValue(3000);

            // Ajoutez un graphique
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accédez à la première série et définissez la texture pour un point
            ChartPoint point = chart.NSeries[0].Points[2];
            point.Area.FillFormat.Texture = TextureType.Stationery;

            // Enregistrez le classeur
            workbook.Save("TextureTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


