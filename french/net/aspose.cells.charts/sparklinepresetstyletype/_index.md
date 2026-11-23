---
title: "Énumération SparklinePresetStyleType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.Charts.SparklinePresetStyleType. Représente les types de style prédéfinis pour les sparkline"
type: docs
url: /fr/net/aspose.cells.charts/sparklinepresetstyletype/
---
## SparklinePresetStyleType enumeration

Représente les types de style prédéfinis pour la sparkline.

```csharp
public enum SparklinePresetStyleType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Style1 | `0` | Style 1 |
| Style2 | `1` | Style 2 |
| Style3 | `2` | Style 3 |
| Style4 | `3` | Style 4 |
| Style5 | `4` | Style 5 |
| Style6 | `5` | Style 6 |
| Style7 | `6` | Style 7 |
| Style8 | `7` | Style 8 |
| Style9 | `8` | Style 9 |
| Style10 | `9` | Style 10 |
| Style11 | `10` | Style 11 |
| Style12 | `11` | Style 12 |
| Style13 | `12` | Style 13 |
| Style14 | `13` | Style 14 |
| Style15 | `14` | Style 15 |
| Style16 | `15` | Style 16 |
| Style17 | `16` | Style 17 |
| Style18 | `17` | Style 18 |
| Style19 | `18` | Style 19 |
| Style20 | `19` | Style 20 |
| Style21 | `20` | Style 21 |
| Style22 | `21` | Style 22 |
| Style23 | `22` | Style 23 |
| Style24 | `23` | Style 24 |
| Style25 | `24` | Style 25 |
| Style26 | `25` | Style 26 |
| Style27 | `26` | Style 27 |
| Style28 | `27` | Style 28 |
| Style29 | `28` | Style 29 |
| Style30 | `29` | Style 30 |
| Style31 | `30` | Style 31 |
| Style32 | `31` | Style 32 |
| Style33 | `32` | Style 33 |
| Style34 | `33` | Style 34 |
| Style35 | `34` | Style 35 |
| Style36 | `35` | Style 36 |
| Custom | `36` | Aucun style prédéfini. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklinePresetStyleTypeDemo
    {
        public static void SparklinePresetStyleTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour les sparklines
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(3);
            worksheet.Cells["D1"].PutValue(4);
            worksheet.Cells["E1"].PutValue(5);
            worksheet.Cells["A2"].PutValue(5);
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["C2"].PutValue(3);
            worksheet.Cells["D2"].PutValue(2);
            worksheet.Cells["E2"].PutValue(1);

            // Définir la CellArea pour les sparklines
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 1;
            ca.StartColumn = 5;
            ca.EndColumn = 5;

            // Ajouter des sparklines à la feuille de calcul
            int idx = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:E2", false, ca);
            SparklineGroup group = worksheet.SparklineGroups[idx];
            group.Sparklines.Add("A1:E1", 0, 5);
            group.Sparklines.Add("A2:E2", 1, 5);

            // Définir le type de style prédéfini du groupe de sparklines
            group.PresetStyle = SparklinePresetStyleType.Style5;

            // Enregistrez le classeur
            workbook.Save("SparklinePresetStyleTypeExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


