---
title: "Line.BeginType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Line. Spécifie une pointe de flèche pour le début d'une ligne"
type: docs
url: /fr/net/aspose.cells.drawing/line/begintype/
---
## Line.BeginType property

Spécifie une pointe de flèche pour le début d'une ligne.

```csharp
public MsoArrowheadStyle BeginType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyBeginTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Ajouter un graphique linéaire
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la source de données du graphique
            chart.NSeries.Add("A1:A3", true);

            // Obtenir la première série et configurer ses propriétés de ligne
            Series series = chart.NSeries[0];
            series.Border.BeginType = MsoArrowheadStyle.Arrow;
            series.Border.EndType = MsoArrowheadStyle.ArrowDiamond;
            series.Border.Color = Color.Red;
            series.Border.Weight = WeightType.MediumLine;

            // Enregistrez le classeur
            workbook.Save("LinePropertyBeginTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [MsoArrowheadStyle](../../msoarrowheadstyle/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


