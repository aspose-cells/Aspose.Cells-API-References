---
title: "SeriesCollection.IsColorVaried"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SeriesCollection. Représente si la couleur des points est variée"
type: docs
url: /fr/net/aspose.cells.charts/seriescollection/iscolorvaried/
---
## SeriesCollection.IsColorVaried property

Représente si la couleur des points varie.

```csharp
public bool IsColorVaried { get; set; }
```

### Remarques

Fonctionne uniquement pour les graphiques circulaires ou lorsqu'il n'y a qu'une seule série.

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionPropertyIsColorVariedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Données d'exemple
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Region");
            cells["A2"].PutValue("France");
            cells["A3"].PutValue("Germany");
            cells["A4"].PutValue("England");
            cells["A5"].PutValue("USA");
            cells["B1"].PutValue("Sales");
            cells["B2"].PutValue(70000);
            cells["B3"].PutValue(55000);
            cells["B4"].PutValue(30000);
            cells["B5"].PutValue(85000);

            // Créer un graphique
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];
            
            // Ajouter une série
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";
            
            // Définir la propriété IsColorVaried
            chart.NSeries.IsColorVaried = true;
            
            // Enregistrez le classeur
            workbook.Save("SeriesCollectionPropertyIsColorVariedDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


