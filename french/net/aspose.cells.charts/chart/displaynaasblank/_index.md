---
title: "Chart.DisplayNaAsBlank"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Chart. Indique s’il faut afficher N/A comme une valeur vide"
type: docs
url: /fr/net/aspose.cells.charts/chart/displaynaasblank/
---
## Chart.DisplayNaAsBlank property

Indique s'il faut afficher #N/A comme une valeur vide.

```csharp
public bool DisplayNaAsBlank { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyDisplayNaAsBlankDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d’exemple avec quelques valeurs NA
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(double.NaN); // NA value
            worksheet.Cells["B4"].PutValue(30);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Définir la propriété DisplayNaAsBlank
            chart.DisplayNaAsBlank = true;

            // Enregistrez le classeur
            workbook.Save("output.xlsx");

            // Vérifier la propriété
            Console.WriteLine("DisplayNaAsBlank is set to: " + chart.DisplayNaAsBlank);
        }
    }
}
```

### Voir aussi

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


