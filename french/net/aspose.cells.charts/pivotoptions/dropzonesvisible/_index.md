---
title: "PivotOptions.DropZonesVisible"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotOptions. Spécifie si des contrôles de tableau croisé dynamique peuvent apparaître sur le graphique croisé dynamique"
type: docs
url: /fr/net/aspose.cells.charts/pivotoptions/dropzonesvisible/
---
## PivotOptions.DropZonesVisible property

Spécifie si des contrôles de pivot peuvent apparaître sur le graphique pivot.

```csharp
public bool DropZonesVisible { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotOptionsPropertyDropZonesVisibleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B5"].PutValue(40);

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("=A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Créer un graphique lié au tableau croisé dynamique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 7, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.PivotSource = "PivotTable1";

            // Configurer les options de tableau croisé dynamique avec DropZonesVisible
            PivotOptions pivotOptions = chart.PivotOptions;
            pivotOptions.DropZonesVisible = true;

            workbook.Save("PivotOptionsDropZonesVisibleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


