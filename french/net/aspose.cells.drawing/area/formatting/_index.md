---
title: "Area.Formatting"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Area. Représente le formatage de la zone"
type: docs
url: /fr/net/aspose.cells.drawing/area/formatting/
---
## Area.Formatting property

Représente le formatage de la zone.

```csharp
public FormattingType Formatting { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class AreaPropertyFormattingDemo
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
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accéder à la zone du graphique et définir le formatage
            ChartArea chartArea = chart.ChartArea;
            chartArea.Area.Formatting = FormattingType.None;

            // Enregistrez le classeur
            workbook.Save("AreaPropertyFormattingDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* enum [FormattingType](../../../aspose.cells.charts/formattingtype/)
* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


