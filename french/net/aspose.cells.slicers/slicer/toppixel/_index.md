---
title: "Slicer.TopPixel"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Slicer. Retourne ou définit le décalage vertical de la forme du slicer par rapport à sa ligne supérieure en pixels"
type: docs
url: /fr/net/aspose.cells.slicers/slicer/toppixel/
---
## Slicer.TopPixel property

Retourne ou définit le décalage vertical de la forme du slicer par rapport à sa ligne supérieure, en pixels.

```csharp
[Obsolete("Use Shape.Top property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int TopPixel { get; set; }
```

### Remarques

REMARQUE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété Shape.Top. Cette propriété sera supprimée 12 mois plus tard, à compter de mai 2025. Aspose s’excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerPropertyTopPixelDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Créer des données d'exemple
            sheet.Cells["A1"].Value = "Product";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["A4"].Value = "Banana";
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 100;
            sheet.Cells["B3"].Value = 200;
            sheet.Cells["B4"].Value = 300;

            // Créer un tableau croisé dynamique et obtenir son indice
            int pivotIndex = sheet.PivotTables.Add("=A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Ajouter un slicer et obtenir son indice
            int slicerIndex = sheet.Slicers.Add(pivotTable, "A6", 0);
            Slicer slicer = sheet.Slicers[slicerIndex];
            
            // Définir la propriété TopPixel
            slicer.TopPixel = 6;
            
            workbook.Save("SlicerTopPixelDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


