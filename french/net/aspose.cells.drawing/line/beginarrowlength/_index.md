---
title: "Line.BeginArrowLength"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Line. Spécifie la longueur de la pointe de flèche pour le début d'une ligne"
type: docs
url: /fr/net/aspose.cells.drawing/line/beginarrowlength/
---
## Line.BeginArrowLength property

Spécifie la longueur de la pointe de flèche pour le début d'une ligne.

```csharp
public MsoArrowheadLength BeginArrowLength { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class LinePropertyBeginArrowLengthDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Préparer des données simples pour un graphique
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

                // Définir le BeginArrowLength sur Long
                seriesLine.BeginArrowLength = MsoArrowheadLength.Long;

                // Lire et afficher la valeur actuelle de BeginArrowLength
                Console.WriteLine("BeginArrowLength value: " + seriesLine.BeginArrowLength);

                // Enregistrez le classeur (optionnel, juste pour compléter la démonstration)
                workbook.Save("BeginArrowLengthDemo.xlsx");
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


