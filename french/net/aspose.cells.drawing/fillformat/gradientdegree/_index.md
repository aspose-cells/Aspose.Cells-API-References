---
title: "FillFormat.GradientDegree"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FillFormat. Retourne le degré du dégradé pour le remplissage spécifié. S’applique uniquement à Excel 2007"
type: docs
url: /fr/net/aspose.cells.drawing/fillformat/gradientdegree/
---
## FillFormat.GradientDegree property

Renvoie le degré du dégradé pour le remplissage spécifié. S'applique uniquement à Excel 2007.

```csharp
public double GradientDegree { get; }
```

### Remarques

Ne peut être qu’une valeur comprise entre 0,0 (sombre) et 1,0 (clair).

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyGradientDegreeDemo
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
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Définir le remplissage en dégradé pour la première série
            Aspose.Cells.Drawing.FillFormat fillFormat = chart.NSeries[0].Area.FillFormat;
            fillFormat.SetTwoColorGradient(Color.Red, Color.Blue, Aspose.Cells.Drawing.GradientStyleType.Horizontal, 2);
            
            // Afficher le degré du dégradé
            Console.WriteLine("Gradient Degree: " + fillFormat.GradientDegree);

            // Enregistrez le classeur
            workbook.Save("GradientDegreeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


