---
title: "Axis.Area"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Axis. Obtient la zone"
type: docs
url: /fr/net/aspose.cells.charts/axis/area/
---
## Axis.Area property

Obtient le `Area`.

```csharp
public Area Area { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AxisPropertyAreaDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
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
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Accéder aux propriétés de la zone de l'axe des catégories
            chart.CategoryAxis.Area.BackgroundColor = Color.LightBlue;
            chart.CategoryAxis.Area.ForegroundColor = Color.White;
            chart.CategoryAxis.Area.Formatting = FormattingType.Custom;
            
            // Enregistrez le classeur
            workbook.Save("AxisPropertyAreaDemo_Output.xlsx");
            
            Console.WriteLine("Category Axis Area Background Color: " + chart.CategoryAxis.Area.BackgroundColor);
        }
    }
}
```

### Voir aussi

* class [Area](../../../aspose.cells.drawing/area/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


