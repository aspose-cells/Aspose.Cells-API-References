---
title: "ChartTextFrame.TextHorizontalAlignment"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartTextFrame. Obtient et définit l'alignement horizontal du texte"
type: docs
url: /fr/net/aspose.cells.charts/charttextframe/texthorizontalalignment/
---
## ChartTextFrame.TextHorizontalAlignment property

Obtient et définit l'alignement horizontal du texte.

```csharp
public TextAlignmentType TextHorizontalAlignment { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyTextHorizontalAlignmentDemo
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

            // Ajouter un graphique et définir sa plage de données
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Obtenir le titre du graphique et définir les propriétés
            Title title = chart.Title;
            title.Text = "Sample Chart Title";
            
            // Démontrer la propriété TextHorizontalAlignment
            title.TextHorizontalAlignment = TextAlignmentType.Center;
            Console.WriteLine("Title horizontal alignment set to: " + title.TextHorizontalAlignment);

            // Enregistrez le classeur
            workbook.Save("ChartTextHorizontalAlignmentDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


