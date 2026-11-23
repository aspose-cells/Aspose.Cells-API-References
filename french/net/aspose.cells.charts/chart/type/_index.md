---
title: "Chart.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Chart propriété. Obtient ou définit le type d'un graphique"
type: docs
url: /fr/net/aspose.cells.charts/chart/type/
---
## Chart.Type property

Obtient ou définit le type d'un graphique.

```csharp
public ChartType Type { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Ajouter un graphique radar
            int chartIndex = sheet.Charts.Add(ChartType.Radar, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Démontrer l'utilisation de la propriété Type
            Console.WriteLine("Chart type is: " + chart.Type);
            
            // Changer le type de graphique en Column
            chart.Type = ChartType.Column;
            Console.WriteLine("Chart type changed to: " + chart.Type);
        }
    }
}
```

### Voir aussi

* enum [ChartType](../../charttype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


