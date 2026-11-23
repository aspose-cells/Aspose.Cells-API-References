---
title: "Chart.BackWall"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Chart. Renvoie un objet Walls qui représente le mur arrière d'un graphique 3D"
type: docs
url: /fr/net/aspose.cells.charts/chart/backwall/
---
## Chart.BackWall property

Renvoie un objet [`Walls`](../walls/) qui représente le mur arrière d'un graphique 3-D.

```csharp
public Walls BackWall { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPropertyBackWallDemo
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
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["B3"].PutValue(1500);
            worksheet.Cells["B4"].PutValue(1800);

            // Ajouter un graphique à colonnes 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.SetChartDataRange("A1:B4", true);

            // Assurez-vous qu'il s'agit d'un graphique 3D
            if (chart.Is3D)
            {
                // Obtenir l'objet BackWall
                Walls backWall = chart.BackWall;

                // Afficher certaines propriétés du BackWall
                Console.WriteLine("BackWall properties:");
                Console.WriteLine("CenterX: " + backWall.CenterX);
                Console.WriteLine("CenterY: " + backWall.CenterY);
                Console.WriteLine("Width: " + backWall.Width);
                Console.WriteLine("Height: " + backWall.Height);

                // Formater le BackWall
                backWall.FillFormat.SetOneColorGradient(
                    System.Drawing.Color.LightBlue, 
                    0.5, // Changed from GradientStyleType to double for degree parameter
                    Aspose.Cells.Drawing.GradientStyleType.Horizontal, 
                    1); // Changed from 0.5 to int for variant parameter

                // Définir les propriétés de bordure
                backWall.Border.Color = System.Drawing.Color.DarkBlue;
                backWall.Border.Weight = Aspose.Cells.Drawing.WeightType.MediumLine;
            }

            // Enregistrez le classeur
            workbook.Save("ChartPropertyBackWallDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Walls](../../walls/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


