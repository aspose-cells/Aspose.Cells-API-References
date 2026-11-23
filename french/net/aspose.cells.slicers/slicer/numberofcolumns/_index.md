---
title: "Slicer.NumberOfColumns"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Slicer. Renvoie ou définit le nombre de colonnes du slicer. La valeur par défaut est 1"
type: docs
url: /fr/net/aspose.cells.slicers/slicer/numberofcolumns/
---
## Slicer.NumberOfColumns property

Renvoie ou définit le nombre de colonnes du slicer. La valeur par défaut est 1.

```csharp
public int NumberOfColumns { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerPropertyNumberOfColumnsDemo
    {
        public static void Run()
        {
            // Créer un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Créer des données d'exemple pour le tableau croisé dynamique
            cells["A1"].Value = "Category";
            cells["B1"].Value = "Product";
            cells["A2"].Value = "Fruits";
            cells["B2"].Value = "Apple";
            cells["A3"].Value = "Fruits";
            cells["B3"].Value = "Banana";
            cells["A4"].Value = "Vegetables";
            cells["B4"].Value = "Carrot";

            // Créer un tableau croisé dynamique - stocker l’index puis obtenir l’objet PivotTable
            int pivotIndex = sheet.PivotTables.Add("D1", "A1:B4", "PivotTable");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Product");
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Ajouter un slicer connecté au tableau croisé dynamique
            int slicerIndex = sheet.Slicers.Add(pivotTable, "Category", "Slicer1");
            Slicer slicer = sheet.Slicers[slicerIndex];

            // Configurer les propriétés du slicer
            slicer.Caption = "Product Categories";
            slicer.TopPixel = 50;
            slicer.LeftPixel = 50;
            slicer.HeightPixel = 150;
            slicer.WidthPixel = 200;

            // Démontrer la propriété NumberOfColumns
            slicer.NumberOfColumns = 2;

            // Enregistrez le classeur
            workbook.Save("SlicerDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


