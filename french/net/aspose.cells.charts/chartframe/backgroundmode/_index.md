---
title: "ChartFrame.BackgroundMode"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartFrame. Obtient et définit le mode d'affichage de l'arrière-plan. Cette propriété n'est valide que dans Excel 2003 ou les versions antérieures."
type: docs
url: /fr/net/aspose.cells.charts/chartframe/backgroundmode/
---
## ChartFrame.BackgroundMode property

Obtient et définit le mode d'affichage de l'arrière-plan. Cette propriété n'est valide que dans Excel 2003 ou les versions antérieures.

```csharp
[Obsolete("Use ChartFrame.Area.FillFormat.FillType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public BackgroundMode BackgroundMode { get; set; }
```

### Remarques

NOTE: Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété ChartFrame.Area.FillFormat.FillType. Par exemple, si vous devez définir le BackgroundMode sur Opaque, vous pouvez utiliser le code suivant : Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Cette propriété sera supprimée 12 mois plus tard, à partir de février 2026. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyBackgroundModeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Orange");
            sheet.Cells["A4"].PutValue("Banana");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["B3"].PutValue(30);
            sheet.Cells["B4"].PutValue(20);

            // Ajoutez un graphique
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Définir les données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Démontrer la propriété BackgroundMode
            chart.ChartArea.BackgroundMode = Aspose.Cells.Charts.BackgroundMode.Transparent;
            chart.PlotArea.BackgroundMode = Aspose.Cells.Charts.BackgroundMode.Automatic;

            // Enregistrez le classeur
            workbook.Save("ChartBackgroundModeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [BackgroundMode](../../backgroundmode/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


