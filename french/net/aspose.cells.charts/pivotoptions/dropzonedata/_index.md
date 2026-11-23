---
title: "PivotOptions.DropZoneData"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotOptions. Spécifie si un contrôle pour chaque champ de tableau croisé dynamique sur l'axe des données du tableau croisé dynamique source apparaît sur le graphique lorsque dropZonesVisible est défini sur true"
type: docs
url: /fr/net/aspose.cells.charts/pivotoptions/dropzonedata/
---
## PivotOptions.DropZoneData property

Spécifie si un contrôle pour chaque champ de PivotTable sur l'axe des données du PivotTable source apparaît sur le graphique lorsque dropZonesVisible est défini sur true.

```csharp
public bool DropZoneData { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PivotOptionsPropertyDropZoneDataDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Books");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Electronics");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Books");
            worksheet.Cells["B4"].PutValue(1500);

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "SalesPivot");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Créer un graphique lié au tableau croisé dynamique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 7, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.PivotSource = "SalesPivot";

            // Configurer les options de tableau croisé dynamique avec DropZoneData activé
            PivotOptions pivotOptions = chart.PivotOptions;
            pivotOptions.DropZoneData = true;
            pivotOptions.DropZonesVisible = true;

            // Enregistrer le résultat
            workbook.Save("PivotOptionsDropZoneDataDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


