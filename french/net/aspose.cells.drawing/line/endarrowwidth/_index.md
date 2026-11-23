---
title: "Line.EndArrowWidth"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Line. Spécifie la largeur de la pointe de flèche pour la fin d'une ligne"
type: docs
url: /fr/net/aspose.cells.drawing/line/endarrowwidth/
---
## Line.EndArrowWidth property

Spécifie la largeur de la pointe de flèche pour la fin d'une ligne.

```csharp
public MsoArrowheadWidth EndArrowWidth { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LinePropertyEndArrowWidthDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le graphique en ligne
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["B3"].PutValue(6);

            // Ajouter un graphique linéaire
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la source de données du graphique
            chart.NSeries.Add("A1:B3", true);

            // Configurer les propriétés de ligne pour la première série
            Series series = chart.NSeries[0];
            series.Border.EndArrowWidth = MsoArrowheadWidth.Wide;
            series.Border.EndType = MsoArrowheadStyle.Arrow;

            // Enregistrez le classeur
            workbook.Save("LinePropertyEndArrowWidthDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [MsoArrowheadWidth](../../msoarrowheadwidth/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


