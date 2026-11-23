---
title: "Line.IsAutomaticColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Line. Indique si la couleur de la ligne est attribuée automatiquement"
type: docs
url: /fr/net/aspose.cells.drawing/line/isautomaticcolor/
---
## Line.IsAutomaticColor property

Indique si la couleur de la ligne est attribuée automatiquement.

```csharp
public bool IsAutomaticColor { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class LinePropertyIsAutomaticColorDemo
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

            try
            {
                // Ajouter un graphique linéaire
                int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
                Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("B2:B3", true);
                chart.NSeries.CategoryData = "A2:A3";

                // Accéder à la ligne (bordure) de la première série
                Line seriesLine = chart.NSeries[0].Border;

                // Lire et afficher la valeur de la propriété IsAutomaticColor
                Console.WriteLine("IsAutomaticColor value: " + seriesLine.IsAutomaticColor);

                // Enregistrez le classeur
                workbook.Save("IsAutomaticColorDemo.xlsx");
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

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


