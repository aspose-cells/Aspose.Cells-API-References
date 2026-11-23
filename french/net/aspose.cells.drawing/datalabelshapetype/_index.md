---
title: "Énumération DataLabelShapeType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.DataLabelShapeType enum. Spécifie la géométrie de forme prédéfinie qui doit être utilisée pour un graphique"
type: docs
url: /fr/net/aspose.cells.drawing/datalabelshapetype/
---
## DataLabelShapeType enumeration

Spécifie la géométrie de forme prédéfinie qui doit être utilisée pour un graphique.

```csharp
public enum DataLabelShapeType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Rect | `0` | Représente la forme rectangulaire. |
| RoundRect | `1` | Représente la forme de rectangle arrondi. |
| Ellipse | `2` | Représente la forme d'ellipse. |
| RightArrowCallout | `3` | Représente la forme d'appel de flèche droite. |
| DownArrowCallout | `4` | Représente la forme d'appel de flèche vers le bas. |
| LeftArrowCallout | `5` | Représente la forme d'appel de flèche gauche. |
| UpArrowCallout | `6` | Représente la forme d'appel de flèche vers le haut. |
| WedgeRectCallout | `7` | Représente la forme d'appel de rectangle en coin. |
| WedgeRoundRectCallout | `8` | Représente la forme d'appel de rectangle arrondi en coin. |
| WedgeEllipseCallout | `9` | Représente la forme d'appel d'ellipse en coin. |
| LineCallout | `10` | Représente la forme d'appel de ligne. |
| BentLineCallout | `11` | Représente la forme d'appel de ligne coudée. |
| LineWithAccentBarCallout | `12` | Représente la forme d'appel de ligne avec barre d'accent. |
| BentLineWithAccentBarCallout | `13` | Représente la forme d'appel de ligne coudée avec barre d'accent. |
| Line | `14` | Ce type n'est utilisé que pour le traitement spécial de fichiers. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class DataLabelShapeTypeDemo
    {
        public static void DataLabelShapeTypeExample()
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

            // Activer les étiquettes de données pour la série.
            series.DataLabels.ShowValue = true;
            series.DataLabels.ShapeType = DataLabelShapeType.RoundRect;

            // Enregistrez le classeur
            workbook.Save("DataLabelShapeTypeExample.xlsx");
            workbook.Save("DataLabelShapeTypeExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


