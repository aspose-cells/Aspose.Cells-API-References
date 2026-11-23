---
title: "Chart.SubTitle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Chart. Obtient le sous-titre du graphique. S'applique uniquement aux fichiers ODS"
type: docs
url: /fr/net/aspose.cells.charts/chart/subtitle/
---
## Chart.SubTitle property

Obtient le sous-titre du graphique. S'applique uniquement aux fichiers ODS.

```csharp
public Title SubTitle { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertySubTitleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
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

            // Ajouter un graphique et définir sa plage de données
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Définir le titre principal
            chart.Title.Text = "Main Chart Title";

            // Définir le sous-titre
            chart.SubTitle.Text = "Chart Subtitle";
            chart.SubTitle.Font.Size = 12;
            chart.SubTitle.Font.IsBold = true;

            // Enregistrez le classeur
            workbook.Save("ChartWithSubtitle.xlsx");
        }
    }
}
```

### Voir aussi

* class [Title](../../title/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


