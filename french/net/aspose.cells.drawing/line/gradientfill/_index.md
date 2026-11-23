---
title: "Line.GradientFill"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Line. Représente le remplissage en dégradé"
type: docs
url: /fr/net/aspose.cells.drawing/line/gradientfill/
---
## Line.GradientFill property

Représente le remplissage en dégradé.

```csharp
public GradientFill GradientFill { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;

    public class LinePropertyGradientFillDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour un graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Ajouter un graphique en colonnes
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Obtenir le premier point de la première série
            Series series = chart.NSeries[0];
            ChartPoint point = series.Points[0];

            try
            {
                // Accéder à l'objet Line (bordure) du point
                Line line = point.Border;

                // Lire la propriété GradientFill (lecture‑seule)
                GradientFill gradient = line.GradientFill;

                // Afficher les détails actuels du remplissage en dégradé
                Console.WriteLine("Current GradientFill:");
                Console.WriteLine($"  FillType       = {gradient.FillType}");
                Console.WriteLine($"  DirectionType = {gradient.DirectionType}");
                Console.WriteLine($"  Angle          = {gradient.Angle}");

                // Modifier le dégradé en utilisant les méthodes fournies
                // Utiliser un transtypage vers une valeur d'énumération par défaut pour éviter de référencer un membre inexistant
                gradient.SetGradient(GradientFillType.Linear, 45.0, (GradientDirectionType)0);
                Console.WriteLine("GradientFill after SetGradient:");
                Console.WriteLine($"  Angle = {gradient.Angle}");

                // Enregistrez le classeur
                workbook.Save("LinePropertyGradientFillDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [GradientFill](../../gradientfill/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


