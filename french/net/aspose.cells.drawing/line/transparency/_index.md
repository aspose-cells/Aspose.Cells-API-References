---
title: "Line.Transparency"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Line. Retourne ou définit le degré de transparence de la ligne sous forme d'une valeur de 0.0 opaque à 1.0 transparent"
type: docs
url: /fr/net/aspose.cells.drawing/line/transparency/
---
## Line.Transparency property

Renvoie ou définit le degré de transparence de la ligne sous forme d'une valeur de 0.0 (opaque) à 1.0 (transparent).

```csharp
public double Transparency { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class LinePropertyTransparencyDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Créer une feuille de calcul d’exemple
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données pour rendre l’exemple significatif
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["B1"].PutValue("Values");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(40);

            try
            {
                // Ajouter un graphique en lignes pour démontrer les propriétés de ligne
                int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
                Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("A1:B3", true);

                // Obtenez les propriétés de ligne à partir de la bordure de la série du graphique
                Line line = chart.NSeries[0].Border;

                // Afficher la valeur actuelle de Transparency
                Console.WriteLine("Current Transparency: " + line.Transparency);

                // Définir une nouvelle valeur de Transparence (0.0 = opaque, 1.0 = clair)
                line.Transparency = 0.5;
                Console.WriteLine("Updated Transparency: " + line.Transparency);

                // Enregistrez le classeur
                workbook.Save("TransparencyDemo.xlsx");
                Console.WriteLine("Transparency property demonstrated successfully.");
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


