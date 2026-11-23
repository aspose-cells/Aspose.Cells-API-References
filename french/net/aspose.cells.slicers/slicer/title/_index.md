---
title: "Slicer.Title"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Slicer. Spécifie le titre de l'objet Slicer actuel"
type: docs
url: /fr/net/aspose.cells.slicers/slicer/title/
---
## Slicer.Title property

Spécifie le titre de l'objet Slicer actuel.

```csharp
[Obsolete("Use Shape.Title property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string Title { get; set; }
```

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété [`Title`](../../../aspose.cells.drawing/shape/title/). Cette propriété sera supprimée 12 mois plus tard, à compter de janvier 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerPropertyTitleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 20;

            // Créer un tableau croisé dynamique
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "C1", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            pivotTable.CalculateData();

            // Ajouter un slicer
            SlicerCollection slicers = worksheet.Slicers;
            int slicerIndex = slicers.Add(pivotTable, "A1", "Fruit");
            Slicer slicer = slicers[slicerIndex];
            
            // Définir le titre du slicer
            slicer.Title = "Fruit Selection Slicer";
            
            // Enregistrez le classeur
            workbook.Save("SlicerTitleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


