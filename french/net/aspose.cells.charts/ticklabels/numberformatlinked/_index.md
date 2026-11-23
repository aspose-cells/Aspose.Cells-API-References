---
title: "TickLabels.NumberFormatLinked"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TickLabels. Vrai si le format numérique est lié aux cellules de sorte que le format numérique change dans les libellés lorsqu'il change dans les cellules"
type: docs
url: /fr/net/aspose.cells.charts/ticklabels/numberformatlinked/
---
## TickLabels.NumberFormatLinked property

Vrai si le format de nombre est lié aux cellules (de sorte que le format de nombre change dans les étiquettes lorsqu'il change dans les cellules).

```csharp
public bool NumberFormatLinked { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyNumberFormatLinkedDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(100);
            worksheet.Cells["A2"].PutValue(200);
            worksheet.Cells["A3"].PutValue(300);
            worksheet.Cells["A4"].PutValue(400);
            
            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la source de données du graphique
            chart.NSeries.Add("A1:A4", true);
            
            // Accéder aux libellés d'échelle de l'axe des valeurs
            Aspose.Cells.Charts.TickLabels tickLabels = chart.ValueAxis.TickLabels;
            
            // Démontrer la propriété NumberFormatLinked
            Console.WriteLine("NumberFormatLinked (default): " + tickLabels.NumberFormatLinked);
            
            // Modifier la propriété
            tickLabels.NumberFormatLinked = false;
            Console.WriteLine("NumberFormatLinked after change: " + tickLabels.NumberFormatLinked);
            
            // Enregistrez le classeur
            workbook.Save("TickLabelsNumberFormatLinkedDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


