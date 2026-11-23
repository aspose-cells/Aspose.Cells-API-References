---
title: "TickLabels.Offset"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TickLabels. Obtient et définit la distance des libellés par rapport à l'axe des catégories. Cela s'applique uniquement à l'axe des catégories x"
type: docs
url: /fr/net/aspose.cells.charts/ticklabels/offset/
---
## TickLabels.Offset property

Obtient et définit la distance des étiquettes par rapport à l'axe des catégories. Cela s'applique uniquement à l'axe des catégories (x).

```csharp
public int Offset { get; set; }
```

### Remarques

La distance par défaut est de 100 pour cent, ce qui représente l'espacement par défaut entre les libellés d'axe et la ligne d'axe. La valeur peut être un pourcentage entier de 0 à 1000, relatif à la taille de police du libellé d'axe.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyOffsetDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Ajoutez un graphique
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accéder à l'axe des valeurs
            Axis valueAxis = chart.ValueAxis;
            
            // Définir le décalage des TickLabels
            valueAxis.TickLabels.Offset = 50; // 50% offset from default position

            // Enregistrez le classeur
            workbook.Save("TickLabelsOffsetDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


