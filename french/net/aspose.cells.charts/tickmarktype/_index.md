---
title: "Énumération TickMarkType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Charts.TickMarkType enum. Représente le type de repère pour l'axe spécifié"
type: docs
url: /fr/net/aspose.cells.charts/tickmarktype/
---
## TickMarkType enumeration

Représente le type de graduation pour l'axe spécifié.

```csharp
public enum TickMarkType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Cross | `0` | Le type de repère est Cross. |
| Inside | `1` | Le type de repère est Inside. |
| None | `2` | Le type de repère est None. |
| Outside | `3` | Le type de repère est Outside |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TickMarkTypeDemo
    {
        public static void TickMarkTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ajoutez NSeries (source de données du graphique) au graphique allant de la cellule "A1" à "B3"
            chart.NSeries.Add("A1:B3", true);

            // Accédez à l'axe des valeurs du graphique
            Axis valueAxis = chart.ValueAxis;

            // Définissez le type de repère majeur sur Cross
            valueAxis.MajorTickMark = TickMarkType.Cross;

            // Définissez le type de repère mineur sur Inside
            valueAxis.MinorTickMark = TickMarkType.Inside;

            // Définir la valeur maximale de l'axe des valeurs
            valueAxis.MaxValue = 200;

            // Définir la valeur minimale de l'axe des valeurs
            valueAxis.MinValue = 0;

            // Définir l'unité principale
            valueAxis.MajorUnit = 25;

            // Enregistrez le classeur
            workbook.Save("TickMarkTypeExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


