---
title: "FillFormat.Pattern"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FillFormat. Représente un motif d'affichage des zones"
type: docs
url: /fr/net/aspose.cells.drawing/fillformat/pattern/
---
## FillFormat.Pattern property

Représente le motif d'affichage d'une zone.

```csharp
public FillPattern Pattern { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyPatternDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue(50);
            sheet.Cells["A2"].PutValue(100);
            sheet.Cells["A3"].PutValue(150);

            // Ajoutez un graphique
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = sheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("A1:A3", true);

            // Accéder à la première série et à son premier point
            ChartPoint point = chart.NSeries[0].Points[0];
            
            // Définir le motif de remplissage pour la zone du point
            point.Area.FillFormat.Pattern = FillPattern.DottedGrid;
            
            // Enregistrez le classeur
            workbook.Save("FillFormatPatternDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [FillPattern](../../fillpattern/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


