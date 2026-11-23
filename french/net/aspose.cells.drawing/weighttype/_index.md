---
title: "Énumération WeightType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.Drawing.WeightType. Énumère les types de poids pour la bordure d'une image ou la ligne d'un graphique"
type: docs
url: /fr/net/aspose.cells.drawing/weighttype/
---
## WeightType enumeration

Énumère les types de poids pour une bordure d'image ou une ligne de graphique.

```csharp
public enum WeightType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| HairLine | `-1` | Représente le poids d'une ligne fine. |
| MediumLine | `1` | Représente le poids d'une ligne moyenne. |
| SingleLine | `0` | Représente le poids d'une ligne simple. |
| WideLine | `2` | Représente le poids d'une ligne large. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassWeightTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez un graphique et obtenez sa zone de graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 5, 15, 15);
            Chart chart = worksheet.Charts[chartIndex];
            ChartArea chartArea = chart.ChartArea;
            
            // Définissez le type de poids de la bordure
            chartArea.Border.Weight = WeightType.WideLine;
            
            // Vérifiez le type de poids
            Console.WriteLine("Chart Area Border Weight: " + chartArea.Border.Weight);
            
            // Enregistrez le classeur
            workbook.Save("WeightTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


