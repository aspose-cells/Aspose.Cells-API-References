---
title: "DataLabels.Number"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataLabels. Obtient et définit le format numérique intégré"
type: docs
url: /fr/net/aspose.cells.charts/datalabels/number/
---
## DataLabels.Number property

Obtient et définit le format de nombre intégré.

```csharp
public int Number { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyNumberDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Bar, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Obtenez la première série et activez les étiquettes de données
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            
            // Accéder aux propriétés des étiquettes de données
            DataLabels dataLabels = series.DataLabels;
            
            // Démontrer l'utilisation de la propriété Number
            Console.WriteLine("Original Number format: " + dataLabels.NumberFormat);
            Console.WriteLine("Original Number property value: " + dataLabels.Number);
            
            // Modifier le format numérique
            dataLabels.Number = 2; // Currency format
            dataLabels.NumberFormat = "$#,##0.00";
            
            Console.WriteLine("Modified Number format: " + dataLabels.NumberFormat);
            Console.WriteLine("Modified Number property value: " + dataLabels.Number);

            // Enregistrez le classeur
            workbook.Save("DataLabelsNumberDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


