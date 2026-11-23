---
title: "DataLabels.Text"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataLabels. Obtient ou définit le texte de l'étiquette de données"
type: docs
url: /fr/net/aspose.cells.charts/datalabels/text/
---
## DataLabels.Text property

Obtient ou définit le texte de l'étiquette de données.

```csharp
public override string Text { get; set; }
```

### Remarques

Fonctionne uniquement lorsque c'est une étiquette de données d'un point de graphique.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyTextDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["A4"].PutValue("Product C");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Activer les étiquettes de données
            for (int i = 0; i < chart.NSeries.Count; i++)
            {
                Aspose.Cells.Charts.Series series = chart.NSeries[i];
                series.DataLabels.ShowValue = true;
                
                // Personnaliser le texte de l'étiquette de données
                for (int j = 0; j < series.Points.Count; j++)
                {
                    series.Points[j].DataLabels.Text = $"+{series.Points[j].YValue}";
                }
            }

            // Enregistrez le classeur
            workbook.Save("DataLabelsTextDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


