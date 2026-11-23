---
title: "Slicer.Width"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Slicer. Retourne ou définit la largeur du slicer spécifié en points"
type: docs
url: /fr/net/aspose.cells.slicers/slicer/width/
---
## Slicer.Width property

Retourne ou définit la largeur du slicer spécifié, en points.

```csharp
[Obsolete("Use Shape.WidthPt property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double Width { get; set; }
```

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété Shape.WidthPt. Cette propriété sera supprimée 12 mois plus tard, à partir de mai 2025. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerPropertyWidthDemo
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
            PivotTableCollection pivotTables = workbook.Worksheets[0].PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Ajouter un segmenteur
            int slicerIndex = worksheet.Slicers.Add(pivotTable, 0, 0, "FruitSlicer");
            Slicer slicer = worksheet.Slicers[slicerIndex];
            
            // Méthode correcte pour ajouter une connexion pivot au slicer
            slicer.AddPivotConnection(pivotTable);

            // Définir les propriétés du slicer, y compris la largeur
            slicer.Caption = "Fruit Selection";
            slicer.Width = 150; // Setting the width in points
            slicer.Height = 200;

            // Enregistrez le classeur
            workbook.Save("SlicerWidthDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


