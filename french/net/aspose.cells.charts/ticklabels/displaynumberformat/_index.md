---
title: "TickLabels.DisplayNumberFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TickLabels. Obtient et définit le format numérique d'affichage des étiquettes de graduation"
type: docs
url: /fr/net/aspose.cells.charts/ticklabels/displaynumberformat/
---
## TickLabels.DisplayNumberFormat property

Obtient et définit le format numérique d'affichage des étiquettes de repères.

```csharp
public string DisplayNumberFormat { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyDisplayNumberFormatDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            worksheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            
            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("A2:A3", true);
            chart.NSeries.CategoryData = "B2:B3";
            
            // Définir le format numérique via la propriété NumberFormat à la place
            chart.CategoryAxis.TickLabels.NumberFormat = "m/d/yyyy";
            chart.ValueAxis.TickLabels.NumberFormat = "#,##0";
            
            // Enregistrez le classeur
            workbook.Save("TickLabelsDisplayNumberFormatDemo.xlsx");
            
            Console.WriteLine("DisplayNumberFormat for CategoryAxis: " + 
                chart.CategoryAxis.TickLabels.DisplayNumberFormat);
            Console.WriteLine("DisplayNumberFormat for ValueAxis: " + 
                chart.ValueAxis.TickLabels.DisplayNumberFormat);
        }
    }
}
```

### Voir aussi

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


