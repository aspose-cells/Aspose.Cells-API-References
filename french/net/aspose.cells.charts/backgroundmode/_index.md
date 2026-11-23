---
title: "Enum BackgroundMode"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Charts.BackgroundMode enum. Représente le mode d'affichage de l'arrière-plan"
type: docs
url: /fr/net/aspose.cells.charts/backgroundmode/
---
## BackgroundMode enumeration

Représente le mode d'affichage de l'arrière-plan.

```csharp
public enum BackgroundMode
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Automatic | `0` | Automatique |
| Opaque | `1` | Opaque |
| Transparent | `2` | Transparent |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class BackgroundModeDemo
    {
        public static void BackgroundModeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Obtenez la référence de la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            
            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ajoutez NSeries (source de données du graphique) au graphique allant de la cellule "A1" à "B3"
            chart.NSeries.Add("A1:B3", true);
            
            // Accéder à la zone du graphique
            ChartArea chartArea = chart.ChartArea;

            // Définir la couleur de premier plan de la zone du graphique
            chartArea.Area.ForegroundColor = Color.Yellow;

            // Définir le mode d'arrière-plan de la zone du graphique
            chartArea.BackgroundMode = BackgroundMode.Opaque;
            chartArea.Area.Transparency = 0.8;           
            
            
            // Définir l'ombre de la zone du graphique
            chartArea.Shadow = true;
            
            // Enregistrez le classeur
            workbook.Save("BackgroundModeExample.xlsx");
            workbook.Save("BackgroundModeExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


