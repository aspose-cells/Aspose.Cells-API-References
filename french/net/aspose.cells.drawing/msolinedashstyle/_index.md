---
title: "Énumération MsoLineDashStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.Drawing.MsoLineDashStyle. Représente le style des lignes pointillées"
type: docs
url: /fr/net/aspose.cells.drawing/msolinedashstyle/
---
## MsoLineDashStyle enumeration

Représente le style des lignes pointillées.

```csharp
public enum MsoLineDashStyle
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Dash | `0` | Représente une ligne en tirets. |
| DashDot | `1` | Représente une ligne tiret-point. |
| DashDotDot | `2` | Représente une ligne tiret-point-point. |
| DashLongDash | `3` | Représente une ligne tiret long‑tiret court. |
| DashLongDashDot | `4` | Représente une ligne tiret long‑tiret court‑point. |
| RoundDot | `5` | Représente une ligne à points ronds. |
| Solid | `6` | Représente une ligne pleine. |
| SquareDot | `7` | Représente une ligne à points carrés. |
| Custom | `8` | Style de tiret personnalisé. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoLineDashStyleDemo
    {
        public static void MsoLineDashStyleExample()
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

            // Accéder à l'axe de catégorie principal
            Axis categoryAxis = chart.CategoryAxis;

            // Définir le style de tiret des lignes de grille majeures
            categoryAxis.MajorGridLines.DashType = MsoLineDashStyle.DashDot;

            // Définir le style de tiret des lignes de grille mineures
            categoryAxis.MinorGridLines.DashType = MsoLineDashStyle.DashLongDashDot;

            // Enregistrez le classeur
            workbook.Save("MsoLineDashStyleExample.xlsx");

            // Afficher les résultats
            Console.WriteLine("Chart with custom dash styles for gridlines created successfully.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


