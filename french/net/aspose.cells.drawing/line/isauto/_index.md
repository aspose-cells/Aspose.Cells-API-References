---
title: "Line.IsAuto"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Line. Indique si ce style de ligne est attribué automatiquement"
type: docs
url: /fr/net/aspose.cells.drawing/line/isauto/
---
## Line.IsAuto property

Indique si ce style de ligne est attribué automatiquement.

```csharp
public bool IsAuto { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class LinePropertyIsAutoDemo
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
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            try
            {
                // Ajouter un graphique linéaire
                int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
                Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

                // Définir la plage de données du graphique
                chart.NSeries.Add("B2:B3", true);
                chart.NSeries.CategoryData = "A2:A3";

                // Accéder aux propriétés de ligne de la série
                Aspose.Cells.Charts.Series series = chart.NSeries[0];
                Line line = series.Border;

                // Afficher la valeur actuelle de IsAuto
                Console.WriteLine("Initial IsAuto value: " + line.IsAuto);

                // Définir IsAuto sur true
                line.IsAuto = true;
                Console.WriteLine("After setting to true, IsAuto value: " + line.IsAuto);

                // Définir IsAuto sur false
                line.IsAuto = false;
                Console.WriteLine("After setting to false, IsAuto value: " + line.IsAuto);

                // Enregistrez le classeur
                workbook.Save("IsAutoDemo.xlsx");
                Console.WriteLine("IsAuto property has been demonstrated successfully.");
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


