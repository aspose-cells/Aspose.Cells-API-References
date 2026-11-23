---
title: "Enum MapChartLabelLayout"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.Charts.MapChartLabelLayout. Représente la disposition des étiquettes des cartes graphiques"
type: docs
url: /fr/net/aspose.cells.charts/mapchartlabellayout/
---
## MapChartLabelLayout enumeration

Représente la disposition des étiquettes du graphique cartographique.

```csharp
public enum MapChartLabelLayout
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| BestFitOnly | `0` | Seul le meilleur ajustement est utilisé. |
| ShowAll | `1` | Affiche toutes les étiquettes. |
| None | `2` | Il n'y a aucune étiquette. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class MapChartLabelLayoutDemo
    {
        public static void MapChartLabelLayoutExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique cartographique
            worksheet.Cells["A1"].PutValue("Country");
            worksheet.Cells["A2"].PutValue("USA");
            worksheet.Cells["A3"].PutValue("Canada");
            worksheet.Cells["A4"].PutValue("Mexico");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(150);

            // Ajouter un graphique cartographique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Map, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données pour le graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accédez aux propriétés de mise en page des séries
            SeriesLayoutProperties layoutProperties = chart.NSeries[0].LayoutProperties;

            // Définir la disposition des étiquettes du graphique cartographique
            layoutProperties.MapLabelLayout = MapChartLabelLayout.ShowAll;

            // Enregistrez le classeur
            workbook.Save("MapChartLabelLayoutExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


