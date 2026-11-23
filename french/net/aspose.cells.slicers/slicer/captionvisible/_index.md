---
title: "Slicer.CaptionVisible"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Slicer. Renvoie ou définit si l’en-tête affichant la légende du slicer est visible. La valeur par défaut est true"
type: docs
url: /fr/net/aspose.cells.slicers/slicer/captionvisible/
---
## Slicer.CaptionVisible property

Renvoie ou définit si l’en-tête affichant la légende du slicer est visible. La valeur par défaut est true

```csharp
[Obsolete("Use Slicer.ShowCaption property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool CaptionVisible { get; set; }
```

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété [`ShowCaption`](../showcaption/) . Cette propriété sera supprimée 12 mois plus tard, à compter de janvier 2026. Aspose s’excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerPropertyCaptionVisibleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Créer un tableau croisé dynamique
            int pivotIndex = workbook.Worksheets[0].PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = workbook.Worksheets[0].PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Ajouter un segmenteur
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "A1", "FruitSlicer");
            Slicer slicer = worksheet.Slicers[slicerIndex];

            // Définir les propriétés du slicer, y compris CaptionVisible
            slicer.Caption = "Fruit Selection";
            slicer.CaptionVisible = true; // Show the caption header
            slicer.NumberOfColumns = 2;
            slicer.StyleType = SlicerStyleType.SlicerStyleLight1;

            // Enregistrez le classeur
            workbook.Save("SlicerCaptionVisibleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


