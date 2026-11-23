---
title: "Enum SparklineAxisMinMaxType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Charts.SparklineAxisMinMaxType enum. Représente les types de valeurs minimale et maximale pour l'axe vertical du sparkline"
type: docs
url: /fr/net/aspose.cells.charts/sparklineaxisminmaxtype/
---
## SparklineAxisMinMaxType enumeration

Représente les types de valeurs minimale et maximale pour l'axe vertical de la sparkline.

```csharp
public enum SparklineAxisMinMaxType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| AutoIndividual | `0` | Automatique pour chaque sparkline. |
| Group | `1` | Identique pour tous les sparklines du groupe. |
| Custom | `2` | Valeur personnalisée pour le sparkline. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class SparklineAxisMinMaxTypeDemo
    {
        public static void SparklineAxisMinMaxTypeExample()
        {
            // Créer un classeur et une feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données à la feuille de calcul
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);

            // Définir la CellArea
            CellArea cellArea = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Ajoute un groupe de sparklines à la feuille de calcul
            int sparklineGroupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, cellArea);
            SparklineGroup sparklineGroup = worksheet.SparklineGroups[sparklineGroupIndex];
            sparklineGroup.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);

            // Définir les propriétés du groupe de sparkline
            sparklineGroup.VerticalAxisMaxValueType = SparklineAxisMinMaxType.Group;
            sparklineGroup.VerticalAxisMinValueType = SparklineAxisMinMaxType.AutoIndividual;

            // Créer CellsColor
            CellsColor highPointColor = workbook.CreateCellsColor();
            highPointColor.Color = Color.Green;
            sparklineGroup.HighPointColor = highPointColor;

            CellsColor lowPointColor = workbook.CreateCellsColor();
            lowPointColor.Color = Color.Red;
            sparklineGroup.LowPointColor = lowPointColor;

            // Définir des propriétés supplémentaires
            sparklineGroup.ShowHighPoint = true;
            sparklineGroup.ShowLowPoint = true;
            sparklineGroup.LineWeight = 1.0;

            // Enregistrez le classeur
            workbook.Save("SparklineAxisMinMaxTypeExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


