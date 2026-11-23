---
title: "Classe PivotOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Charts.PivotOptions classe. Représente un type complexe qui spécifie les contrôles de pivot qui apparaissent sur le graphique"
type: docs
url: /fr/net/aspose.cells.charts/pivotoptions/
---
## PivotOptions class

Représente un type complexe qui spécifie les contrôles de tableau croisé dynamique qui apparaissent sur le graphique

```csharp
public class PivotOptions
```

## Propriétés

| Nom | Description |
| --- | --- |
| [DropZoneCategories](../../aspose.cells.charts/pivotoptions/dropzonecategories/) { get; set; } | Spécifie si un contrôle pour chaque champ de PivotTable sur l'axe des lignes du PivotTable source apparaît sur le graphique lorsque dropZonesVisible est défini sur true. |
| [DropZoneData](../../aspose.cells.charts/pivotoptions/dropzonedata/) { get; set; } | Spécifie si un contrôle pour chaque champ de PivotTable sur l'axe des données du PivotTable source apparaît sur le graphique lorsque dropZonesVisible est défini sur true. |
| [DropZoneFilter](../../aspose.cells.charts/pivotoptions/dropzonefilter/) { get; set; } | Spécifie si un contrôle pour chaque champ de PivotTable sur l'axe des pages du PivotTable source apparaît sur le graphique lorsque dropZonesVisible est défini sur true. |
| [DropZoneSeries](../../aspose.cells.charts/pivotoptions/dropzoneseries/) { get; set; } | Spécifie si un contrôle pour chaque champ de PivotTable sur l'axe des colonnes du PivotTable source apparaît sur le graphique lorsque dropZonesVisible est défini sur true. |
| [DropZonesVisible](../../aspose.cells.charts/pivotoptions/dropzonesvisible/) { get; set; } | Spécifie si des contrôles de pivot peuvent apparaître sur le graphique pivot. |
| [ShowExpandCollapseFieldButtons](../../aspose.cells.charts/pivotoptions/showexpandcollapsefieldbuttons/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut afficher les boutons d'extension ou de réduction des champs |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotOptionsDemo
    {
        public static void PivotOptionsExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données pour le tableau croisé dynamique
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

            // Ajouter un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("=A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 7, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.PivotSource = "PivotTable1";

            // Accédez aux PivotOptions du graphique
            PivotOptions pivotOptions = chart.PivotOptions;

            // Définissez les propriétés de PivotOptions
            pivotOptions.DropZoneFilter = true;
            pivotOptions.DropZoneCategories = true;
            pivotOptions.DropZoneData = true;
            pivotOptions.DropZoneSeries = true;
            pivotOptions.DropZonesVisible = true;

            // Enregistrez le classeur
            workbook.Save("PivotOptionsExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


