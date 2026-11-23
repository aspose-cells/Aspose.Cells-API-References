---
title: "ChartFrame.Background"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartFrame. Obtient et définit le mode d'affichage de l'arrière-plan. Cette propriété n'est valide que dans Excel 2003 ou les versions antérieures."
type: docs
url: /fr/net/aspose.cells.charts/chartframe/background/
---
## ChartFrame.Background property

Obtient et définit le mode d'affichage de l'arrière-plan. Cette propriété n'est valide que dans Excel 2003 ou les versions antérieures.

```csharp
[Obsolete("Use ChartFrame.Area.FillFormat.FillType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public BackgroundMode Background { get; set; }
```

### Remarques

NOTE : Cet élément est maintenant obsolète. À la place, veuillez utiliser la propriété ChartFrame.Area.FillFormat.FillType. Par exemple, si vous devez définir BackgroundMode sur Opaque, vous pouvez utiliser le code suivant : Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Cette propriété sera supprimée 12 mois plus tard, à compter de JANVIER 2012. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyBackgroundDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
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

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Configurer les données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Configurer les étiquettes de données avec les paramètres d'arrière-plan
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowValue = true;
            dataLabels.Background = BackgroundMode.Transparent;

            // Enregistrez le classeur
            workbook.Save("ChartBackgroundDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [BackgroundMode](../../backgroundmode/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


