---
title: "LegendEntry.IsTextNoFill"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LegendEntry. Obtient ou définit l'absence de remplissage du texte"
type: docs
url: /fr/net/aspose.cells.charts/legendentry/istextnofill/
---
## LegendEntry.IsTextNoFill property

Obtient ou définit aucun remplissage du texte.

```csharp
public bool IsTextNoFill { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendEntryPropertyIsTextNoFillDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");

            // Ajouter un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B2", true);
            chart.NSeries.CategoryData = "C1:C2";

            // Accéder à l'entrée de légende et définir IsTextNoFill
            LegendEntry legendEntry = chart.NSeries[0].LegendEntry;
            legendEntry.IsTextNoFill = true; // Text will have no fill
            
            // Enregistrez le classeur
            workbook.Save("LegendEntryIsTextNoFillDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


