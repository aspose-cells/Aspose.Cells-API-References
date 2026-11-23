---
title: "Enum SlicerStyleType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Slicers.SlicerStyleType enum. Spécifiez le style de la vue du segmenteur"
type: docs
url: /fr/net/aspose.cells.slicers/slicerstyletype/
---
## SlicerStyleType enumeration

Spécifiez le style de la vue du slicer.

```csharp
public enum SlicerStyleType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| SlicerStyleLight1 | `0` | style clair intégré un |
| SlicerStyleLight2 | `1` | style clair intégré deux |
| SlicerStyleLight3 | `2` | style clair intégré trois |
| SlicerStyleLight4 | `3` | style clair intégré quatre |
| SlicerStyleLight5 | `4` | style clair intégré cinq |
| SlicerStyleLight6 | `5` | style clair intégré six |
| SlicerStyleOther1 | `6` | autre style intégré un |
| SlicerStyleOther2 | `7` | autre style intégré deux |
| SlicerStyleDark1 | `8` | style sombre intégré un |
| SlicerStyleDark2 | `9` | style sombre intégré deux |
| SlicerStyleDark3 | `10` | style sombre intégré trois |
| SlicerStyleDark4 | `11` | style sombre intégré quatre |
| SlicerStyleDark5 | `12` | style sombre intégré cinq |
| SlicerStyleDark6 | `13` | style sombre intégré six |
| Custom | `14` | style défini par l'utilisateur, non pris en charge pour le moment |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicersClassSlicerStyleTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Créer des données d'exemple pour le tableau croisé dynamique
            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["A4"].Value = "Banana";
            sheet.Cells["A5"].Value = "Apple";
            sheet.Cells["B1"].Value = "Quantity";
            sheet.Cells["B2"].Value = 10;
            sheet.Cells["B3"].Value = 15;
            sheet.Cells["B4"].Value = 8;
            sheet.Cells["B5"].Value = 12;

            // Créer un tableau croisé dynamique
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Data, 1);

            // Ajouter un slicer
            int slicerIndex = sheet.Slicers.Add(pivot, "G1", pivot.BaseFields[0]);
            Slicer slicer = sheet.Slicers[slicerIndex];
            
            // Définir le style du segment
            slicer.StyleType = SlicerStyleType.SlicerStyleDark1;
            slicer.NumberOfColumns = 2;

            // Enregistrez le classeur
            wb.Save("SlicerStyleTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Slicers](../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../)


