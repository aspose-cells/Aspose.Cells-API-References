---
title: "Enum GradientPresetType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.Drawing.GradientPresetType. Représente le type de couleur de dégradé prédéfini"
type: docs
url: /fr/net/aspose.cells.drawing/gradientpresettype/
---
## GradientPresetType enumeration

Représente le type de couleur prédéfini du dégradé.

```csharp
public enum GradientPresetType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Brass | `0` | Couleur prédéfinie Laiton |
| CalmWater | `1` | Couleur prédéfinie Eau calme |
| Chrome | `2` | Couleur prédéfinie Chrome |
| ChromeII | `3` | Couleur prédéfinie Chrome II |
| Daybreak | `4` | Couleur prédéfinie Aube |
| Desert | `5` | Couleur prédéfinie Désert |
| EarlySunset | `6` | Couleur prédéfinie Coucher de soleil tôt |
| Fire | `7` | Couleur prédéfinie Feu |
| Fog | `8` | Couleur prédéfinie Brouillard |
| Gold | `9` | Couleur prédéfinie Or |
| GoldII | `10` | Couleur prédéfinie Or II |
| Horizon | `11` | Couleur prédéfinie Horizon |
| LateSunset | `12` | Couleur prédéfinie Coucher de soleil tardif |
| Mahogany | `13` | Couleur prédéfinie Acajou |
| Moss | `14` | Couleur prédéfinie mousse |
| Nightfall | `15` | Couleur prédéfinie crépuscule |
| Ocean | `16` | Couleur prédéfinie océan |
| Parchment | `17` | Couleur prédéfinie parchemin |
| Peacock | `18` | Couleur prédéfinie paon |
| Rainbow | `19` | Couleur prédéfinie arc-en-ciel |
| RainbowII | `20` | Couleur prédéfinie arc-en-ciel II |
| Sapphire | `21` | Couleur prédéfinie saphir |
| Silver | `22` | Couleur prédéfinie argent |
| Wheat | `23` | Couleur prédéfinie blé |
| Unknown | `24` | Couleur prédéfinie inconnue. Seulement pour la couleur prédéfinie (qui n'est identique à aucune couleur prédéfinie connue) dans le classeur modèle. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientPresetTypeDemo
    {
        public static void GradientPresetTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données du graphique
            chart.SetChartDataRange("A1:B4", true);

            // Accéder à l'axe des catégories du graphique
            Axis categoryAxis = chart.CategoryAxis;

            // Accéder au format de remplissage de la zone de l'axe des catégories
            FillFormat fillFormat = categoryAxis.Area.FillFormat;

            // Définir une couleur prédéfinie en dégradé pour le format de remplissage
            fillFormat.SetPresetColorGradient(GradientPresetType.Fire, GradientStyleType.Horizontal, 1);

            // Renvoie le type de couleur prédéfinie en dégradé
            Console.WriteLine("Gradient Preset Color: " + fillFormat.PresetColor);

            // Enregistrez le classeur
            workbook.Save("GradientPresetTypeExample.xlsx");
            workbook.Save("GradientPresetTypeExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


