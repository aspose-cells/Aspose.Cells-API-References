---
title: "ChartFrame.Area"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartFrame. Obtient la zone"
type: docs
url: /fr/net/aspose.cells.charts/chartframe/area/
---
## ChartFrame.Area property

Obtient le `area`.

```csharp
public virtual Area Area { get; }
```

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyAreaDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accéder à la zone du graphique
            ChartArea chartArea = chart.ChartArea;
            
            // Démontrer la fonctionnalité de la propriété Area
            Area area = chartArea.Area;
            Console.WriteLine("Original Formatting: " + area.Formatting);
            
            // Modifier les propriétés de la zone
            area.Formatting = FormattingType.Custom;
            area.BackgroundColor = Color.LightBlue;
            area.ForegroundColor = Color.DarkBlue;
            area.Transparency = 0.3;
            area.InvertIfNegative = true;

            // Enregistrez le classeur
            workbook.Save("ChartFramePropertyAreaDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Area](../../../aspose.cells.drawing/area/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


