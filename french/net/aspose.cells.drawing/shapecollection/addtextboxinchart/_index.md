---
title: "ShapeCollection.AddTextBoxInChart"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeCollection. Ajoute une zone de texte au graphique"
type: docs
url: /fr/net/aspose.cells.drawing/shapecollection/addtextboxinchart/
---
## ShapeCollection.AddTextBoxInChart method

Ajoute une zone de texte au graphique.

```csharp
public TextBox AddTextBoxInChart(int top, int left, int height, int width)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| haut | Int32 | Représente le décalage vertical de la zone de texte depuis le coin supérieur gauche, en unités de 1/4000 de la zone du graphique. |
| gauche | Int32 | Représente le décalage vertical de la zone de texte depuis le coin supérieur gauche, en unités de 1/4000 de la zone du graphique. |
| hauteur | Int32 | Représente la hauteur de la zone de texte, en unités de 1/4000 de la zone du graphique. |
| largeur | Int32 | Représente la largeur de la zone de texte, en unités de 1/4000 de la zone du graphique. |

### Valeur de retour

Un objet TextBox.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddTextBoxInChartWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart waterfallChart = worksheet.Charts[chartIndex];

            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Categories");
            cells["A2"].PutValue("Start");
            cells["A3"].PutValue("Positive Value 1");
            cells["A4"].PutValue("Negative Value 1");
            cells["A5"].PutValue("Positive Value 2");
            cells["A6"].PutValue("End");
            waterfallChart.NSeries.CategoryData = "A2:A6";

            cells["B1"].PutValue("Values");
            cells["B2"].PutValue(0);
            cells["B3"].PutValue(20);
            cells["B4"].PutValue(-10);
            cells["B5"].PutValue(15);
            cells["B6"].PutValue(25);
            waterfallChart.NSeries.Add("B2:B6", true);

            Shape textBox = waterfallChart.Shapes.AddTextBoxInChart(100, 100, 200, 50);
            textBox.Text = "Sample TextBox in Chart";
            textBox.Font.Color = Color.Blue;

            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [TextBox](../../textbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


