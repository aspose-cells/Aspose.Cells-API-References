---
title: "Line.EndArrowLength"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Line. Spécifie la longueur de la pointe de flèche pour l'extrémité d'une ligne"
type: docs
url: /fr/net/aspose.cells.drawing/line/endarrowlength/
---
## Line.EndArrowLength property

Spécifie la longueur de la pointe de flèche pour la fin d'une ligne.

```csharp
public MsoArrowheadLength EndArrowLength { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class LinePropertyEndArrowLengthDemo
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
                // Ajoutez un graphique pour démontrer les propriétés de ligne
                int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 15, 5);
                Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("A1:B3", true);

                // Obtenez les propriétés de ligne à partir de la bordure de la série du graphique
                Line line = chart.NSeries[0].Border;

                // Définir un type de pointe de flèche pour démontrer EndArrowLength
                line.EndType = MsoArrowheadStyle.Arrow;

                // Afficher la valeur actuelle de EndArrowLength
                Console.WriteLine("Current EndArrowLength: " + line.EndArrowLength);

                // Définir une nouvelle valeur pour EndArrowLength
                line.EndArrowLength = MsoArrowheadLength.Long;
                Console.WriteLine("Updated EndArrowLength: " + line.EndArrowLength);

                // Enregistrez le classeur
                workbook.Save("EndArrowLengthDemo.xlsx");
                Console.WriteLine("EndArrowLength property demonstrated successfully.");
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

* enum [MsoArrowheadLength](../../msoarrowheadlength/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


