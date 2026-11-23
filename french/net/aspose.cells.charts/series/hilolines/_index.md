---
title: "Series.HiLoLines"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Series. Retourne un objet HiLoLines qui représente les lignes haut-bas pour une série sur un graphique en courbes. S'applique uniquement aux graphiques en courbes"
type: docs
url: /fr/net/aspose.cells.charts/series/hilolines/
---
## Series.HiLoLines property

Renvoie un objet HiLoLines qui représente les lignes haut-bas pour une série sur un graphique en courbes. S'applique uniquement aux graphiques en courbes.

```csharp
public Line HiLoLines { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class SeriesPropertyHiLoLinesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["A5"].PutValue("Q4");

            worksheet.Cells["B1"].PutValue("High");
            worksheet.Cells["B2"].PutValue(120);
            worksheet.Cells["B3"].PutValue(90);
            worksheet.Cells["B4"].PutValue(150);
            worksheet.Cells["B5"].PutValue(110);

            worksheet.Cells["C1"].PutValue("Low");
            worksheet.Cells["C2"].PutValue(80);
            worksheet.Cells["C3"].PutValue(60);
            worksheet.Cells["C4"].PutValue(100);
            worksheet.Cells["C5"].PutValue(70);

            // Ajouter un graphique linéaire
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 6, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données du graphique
            chart.NSeries.Add("B1:B5", true);
            chart.NSeries.Add("C1:C5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Activer HiLoLines pour la première série
            Series series = chart.NSeries[0];
            series.HasHiLoLines = true;

            // Accéder et modifier les propriétés HiLoLines
            Line hiLoLines = series.HiLoLines;
            Console.WriteLine("HiLoLines visibility: " + hiLoLines.IsVisible);

            // Personnaliser l'apparence de HiLoLines
            hiLoLines.Color = System.Drawing.Color.Red;
            hiLoLines.Weight = WeightType.MediumLine;
            hiLoLines.DashType = MsoLineDashStyle.DashDot;
            hiLoLines.IsVisible = true;

            // Enregistrer le résultat
            workbook.Save("SeriesPropertyHiLoLinesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Line](../../../aspose.cells.drawing/line/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


