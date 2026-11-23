---
title: "Enum FillPattern"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.FillPattern enum. Énumère les types de motifs de remplissage de forme"
type: docs
url: /fr/net/aspose.cells.drawing/fillpattern/
---
## FillPattern enumeration

Énumère les types de motifs de remplissage de forme.

```csharp
public enum FillPattern
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Représente aucun arrière-plan. |
| Solid | `1` | Représente le motif plein. |
| Gray5 | `2` | Représente le motif gris à 5%. |
| Gray10 | `3` | Représente le motif gris à 10%. |
| Gray20 | `4` | Représente le motif gris à 20%. |
| Gray30 | `5` | Représente le motif gris à 30%. |
| Gray40 | `6` | Représente le motif gris à 40%. |
| Gray50 | `7` | Représente le motif gris à 50 %. |
| Gray60 | `8` | Représente le motif gris à 60%. |
| Gray70 | `9` | Représente le motif gris à 70%. |
| Gray75 | `10` | Représente le motif gris à 75 %. |
| Gray80 | `11` | Représente le motif gris à 80 %. |
| Gray90 | `12` | Représente le motif gris à 90 %. |
| Gray25 | `13` | Représente le motif gris à 25 %. |
| LightDownwardDiagonal | `14` | Représente le motif diagonal clair descendant. |
| LightUpwardDiagonal | `15` | Représente le motif diagonal clair ascendant. |
| DarkDownwardDiagonal | `16` | Représente le motif diagonal foncé descendant. |
| DarkUpwardDiagonal | `17` | Représente le motif diagonal foncé ascendant. |
| WideDownwardDiagonal | `18` | Représente le motif diagonal large descendant. |
| WideUpwardDiagonal | `19` | Représente le motif diagonal large ascendant. |
| LightVertical | `20` | Représente le motif vertical clair. |
| LightHorizontal | `21` | Représente le motif horizontal clair. |
| NarrowVertical | `22` | Représente le motif vertical étroit. |
| NarrowHorizontal | `23` | Représente le motif horizontal étroit. |
| DarkVertical | `24` | Représente le motif vertical foncé. |
| DarkHorizontal | `25` | Représente le motif horizontal foncé. |
| DashedDownwardDiagonal | `26` | Représente le motif diagonal pointillé descendant. |
| DashedUpwardDiagonal | `27` | Représente le motif diagonal pointillé ascendant. |
| DashedVertical | `28` | Représente le motif vertical pointillé. |
| DashedHorizontal | `29` | Représente le motif horizontal pointillé. |
| SmallConfetti | `30` | Représente le petit motif confetti. |
| LargeConfetti | `31` | Représente le grand motif confetti. |
| ZigZag | `32` | Représente le motif zigzag. |
| Wave | `33` | Représente le motif vague. |
| DiagonalBrick | `34` | Représente le motif de brique diagonale. |
| HorizontalBrick | `35` | Représente le motif de brique horizontale. |
| Weave | `36` | Représente le motif tissé. |
| Plaid | `37` | Représente le motif à carreaux. |
| Divot | `38` | Représente le motif en creux. |
| DottedGrid | `39` | Représente le motif de grille à points. |
| DottedDiamond | `40` | Représente le motif de losange à points. |
| Shingle | `41` | Représente le motif en bardeaux. |
| Trellis | `42` | Représente le motif en treillis. |
| Sphere | `43` | Représente le motif sphérique. |
| SmallGrid | `44` | Représente le petit motif de grille. |
| LargeGrid | `45` | Représente le grand motif de grille. |
| SmallCheckerBoard | `46` | Représente le petit motif de damier. |
| LargeCheckerBoard | `47` | Représente le grand motif de damier. |
| OutlinedDiamond | `48` | Représente le motif de losange contourné. |
| SolidDiamond | `49` | Représente le motif de losange plein. |
| Unknown | `50` | Représente un motif inconnu. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassFillPatternDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Définir le motif de remplissage pour la première série
            Series series = chart.NSeries[0];
            series.Area.FillFormat.Pattern = FillPattern.Plaid;

            // Enregistrez le classeur
            workbook.Save("FillPatternDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


