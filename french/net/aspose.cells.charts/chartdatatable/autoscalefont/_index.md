---
title: "ChartDataTable.AutoScaleFont"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartDataTable. Vrai si le texte de l'objet change de taille de police lorsque la taille de l'objet change. La valeur par défaut est Vrai"
type: docs
url: /fr/net/aspose.cells.charts/chartdatatable/autoscalefont/
---
## ChartDataTable.AutoScaleFont property

Vrai si le texte de l'objet change de taille de police lorsque la taille de l'objet change. La valeur par défaut est Vrai.

```csharp
public bool AutoScaleFont { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyAutoScaleFontDemo
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

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Activer le tableau de données
            chart.ShowDataTable = true;
            
            // Accéder aux propriétés du tableau de données du graphique
            // Manière correcte d'obtenir ChartDataTable lorsque ShowDataTable est vrai
            ChartDataTable dataTable = chart.ChartDataTable;
            
            // Démontrer la propriété AutoScaleFont
            dataTable.AutoScaleFont = false; // Disable auto-scaling
            Console.WriteLine("AutoScaleFont (false): " + dataTable.AutoScaleFont);
            
            dataTable.AutoScaleFont = true; // Enable auto-scaling
            Console.WriteLine("AutoScaleFont (true): " + dataTable.AutoScaleFont);

            // Enregistrez le classeur
            workbook.Save("ChartDataTableAutoScaleFontDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


