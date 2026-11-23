---
title: "Classe Line"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.Line. Encapsule l'objet qui représente le format de ligne"
type: docs
url: /fr/net/aspose.cells.drawing/line/
---
## Line class

Encapsule l'objet qui représente le format de ligne.

```csharp
public class Line
```

## Propriétés

| Nom | Description |
| --- | --- |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength/) { get; set; } | Spécifie la longueur de la pointe de flèche pour le début d'une ligne. |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth/) { get; set; } | Spécifie la largeur de la pointe de flèche pour le début d'une ligne. |
| [BeginType](../../aspose.cells.drawing/line/begintype/) { get; set; } | Spécifie une pointe de flèche pour le début d'une ligne. |
| [CapType](../../aspose.cells.drawing/line/captype/) { get; set; } | Spécifie les embouts de fin. |
| [Color](../../aspose.cells.drawing/line/color/) { get; set; } | Représente la couleur de la ligne. |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype/) { get; set; } | Spécifie le type de ligne composé |
| [DashType](../../aspose.cells.drawing/line/dashtype/) { get; set; } | Spécifie le type de ligne en pointillé |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength/) { get; set; } | Spécifie la longueur de la pointe de flèche pour la fin d'une ligne. |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth/) { get; set; } | Spécifie la largeur de la pointe de flèche pour la fin d'une ligne. |
| [EndType](../../aspose.cells.drawing/line/endtype/) { get; set; } | Spécifie une pointe de flèche pour la fin d'une ligne. |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype/) { get; set; } | Obtient ou définit le type de format. |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill/) { get; } | Représente le remplissage en dégradé. |
| [IsAuto](../../aspose.cells.drawing/line/isauto/) { get; set; } | Indique si ce style de ligne est attribué automatiquement. |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor/) { get; } | Indique si la couleur de la ligne est attribuée automatiquement. |
| [IsVisible](../../aspose.cells.drawing/line/isvisible/) { get; set; } | Représente si la ligne est visible. |
| [JoinType](../../aspose.cells.drawing/line/jointype/) { get; set; } | Spécifie les extrémités de jointure. |
| [Style](../../aspose.cells.drawing/line/style/) { get; set; } | Représente le style de la ligne. |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor/) { get; set; } | Obtient et définit la couleur du thème. |
| [Transparency](../../aspose.cells.drawing/line/transparency/) { get; set; } | Renvoie ou définit le degré de transparence de la ligne sous forme d'une valeur de 0.0 (opaque) à 1.0 (transparent). |
| [Weight](../../aspose.cells.drawing/line/weight/) { get; set; } | Obtient ou définit le [`WeightType`](../weighttype/) de la ligne. |
| [WeightPt](../../aspose.cells.drawing/line/weightpt/) { get; set; } | Obtient ou définit le poids de la ligne en points. |
| [WeightPx](../../aspose.cells.drawing/line/weightpx/) { get; set; } | Obtient ou définit le poids de la ligne en unités de pixels. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassLineDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            Cells cells = sheet.Cells;
            cells[0,1].PutValue("Income");
            cells[1,0].PutValue("Company A");
            cells[2,0].PutValue("Company B");
            cells[3,0].PutValue("Company C");
            cells[1,1].PutValue(10000);
            cells[2,1].PutValue(20000);
            cells[3,1].PutValue(30000);
            
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 9, 9, 21, 15);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            chart.NSeries.Add("B1:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            chart.NSeries[0].Border.Style = LineType.Dot;
            chart.NSeries[0].Border.Color = Color.Red;
            chart.NSeries[0].Marker.MarkerStyle = ChartMarkerType.Triangle;
            chart.NSeries[0].Border.Weight = WeightType.MediumLine;
            
            workbook.Save("LineChartDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


