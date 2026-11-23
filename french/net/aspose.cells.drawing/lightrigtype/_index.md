---
title: "Enum LightRigType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.Drawing.LightRigType. Représente un éclairage prédéfini qui peut être appliqué à une forme"
type: docs
url: /fr/net/aspose.cells.drawing/lightrigtype/
---
## LightRigType enumeration

Représente une lumière prédéfinie à droite pouvant être appliquée à une forme

```csharp
public enum LightRigType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Balanced | `0` | Équilibré |
| BrightRoom | `1` | Pièce lumineuse |
| Chilly | `2` | Frais |
| Contrasting | `3` | Contrasté |
| Flat | `4` | Plat |
| Flood | `5` | Inondation |
| Freezing | `6` | Glacial |
| Glow | `7` | Lueur |
| Harsh | `8` | Dur |
| LegacyFlat1 | `9` | LegacyFlat1 |
| LegacyFlat2 | `10` | LegacyFlat2 |
| LegacyFlat3 | `11` | LegacyFlat3 |
| LegacyFlat4 | `12` | LegacyFlat4 |
| LegacyHarsh1 | `13` | LegacyHarsh1 |
| LegacyHarsh2 | `14` | LegacyHarsh2 |
| LegacyHarsh3 | `15` | LegacyHarsh3 |
| LegacyHarsh4 | `16` | LegacyHarsh4 |
| LegacyNormal1 | `17` | LegacyNormal1 |
| LegacyNormal2 | `18` | LegacyNormal2 |
| LegacyNormal3 | `19` | LegacyNormal3 |
| LegacyNormal4 | `20` | LegacyNormal4 |
| Morning | `21` | Matin |
| Soft | `22` | Doux |
| Sunrise | `23` | Lever du soleil |
| Sunset | `24` | Coucher du soleil |
| ThreePoint | `25` | Trois points |
| TwoPoint | `26` | Deux points |
| None | `27` | Pas de dispositif d'éclairage. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class LightRigTypeDemo
    {
        public static void LightRigTypeExample()
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

            // Accéder à la première série du graphique
            Series series = chart.NSeries[0];

            // Accédez aux propriétés de forme de la série
            ShapePropertyCollection shapeProperties = series.ShapeProperties;

            // Vérifiez si la série possède des données de format 3D
            if (shapeProperties.HasFormat3D())
            {
                // Accéder aux propriétés du format 3D
                Format3D format3D = shapeProperties.Format3D;

                // Définissez le type d'éclairage de surface sur Équilibré
                format3D.SurfaceLightingType = LightRigType.Balanced;

                // Définissez l'angle d'éclairage
                format3D.LightingAngle = 45.0;
            }

            // Enregistrez le classeur
            workbook.Save("LightRigTypeExample.xlsx");
            workbook.Save("LightRigTypeExample.pdf");
            // Afficher les résultats
            Console.WriteLine("LightRigType example applied and workbook saved as 'LightRigTypeExample.xlsx'.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


