---
title: "Slicer.Placement"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Slicer. Représente la façon dont l'objet de dessin est attaché aux cellules en dessous. La propriété contrôle le placement d'un objet sur une feuille de calcul."
type: docs
url: /fr/net/aspose.cells.slicers/slicer/placement/
---
## Slicer.Placement property

Représente la façon dont l'objet de dessin est attaché aux cellules en dessous. La propriété contrôle le placement d'un objet sur une feuille de calcul.

```csharp
[Obsolete("Use Shape.Placement property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PlacementType Placement { get; set; }
```

### Remarques

REMARQUE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété [`Placement`](../../../aspose.cells.drawing/shape/placement/). Cette propriété sera supprimée 12 mois plus tard à compter de janvier 2026. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Drawing;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerPropertyPlacementDemo
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
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["B4"].Value = 200;

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Ajouter le champ de ligne
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");

            // Ajouter le champ de données
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Ajouter un slicer pour le tableau croisé dynamique
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "Fruit", "A6");
            Slicer slicer = worksheet.Slicers[slicerIndex];

            // Définir les propriétés du slicer incluant Placement
            slicer.Title = "Fruit Slicer";
            slicer.Placement = PlacementType.MoveAndSize; // Demonstrate Placement property
            slicer.HeightPixel = 200;
            slicer.WidthPixel = 150;

            // Enregistrez le classeur
            workbook.Save("SlicerPlacementDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [PlacementType](../../../aspose.cells.drawing/placementtype/)
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


