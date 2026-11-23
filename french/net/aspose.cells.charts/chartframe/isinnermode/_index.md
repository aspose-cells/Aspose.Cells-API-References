---
title: "ChartFrame.IsInnerMode"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartFrame. Indique si la taille de la zone de tracé inclut les marques de graduation et les libellés d'axe. False spécifie que la taille doit déterminer la taille de la zone de tracé, les marques de graduation et les libellés d'axe"
type: docs
url: /fr/net/aspose.cells.charts/chartframe/isinnermode/
---
## ChartFrame.IsInnerMode property

Indique si la taille de la zone de tracé inclut les marques de graduation et les étiquettes d'axe. False spécifie que la taille doit déterminer la taille de la zone de tracé, les marques de graduation et les étiquettes d'axe.

```csharp
public bool IsInnerMode { get; set; }
```

### Remarques

Uniquement pour le fichier Xlsx.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyIsInnerModeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajouter un graphique
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accéder au cadre du graphique et démontrer IsInnerMode
            Aspose.Cells.Charts.ChartFrame chartFrame = chart.ChartArea;
            chartFrame.IsInnerMode = true; // Set to use inner mode
            
            // Définir quelques propriétés de base pour montrer l'effet
            chartFrame.Border.Color = Color.Blue;
            chartFrame.Border.Style = Aspose.Cells.Drawing.LineType.Solid;
            chartFrame.Area.ForegroundColor = Color.LightYellow;

            workbook.Save("ChartFrameIsInnerModeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


