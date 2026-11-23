---
title: "Slicer.LockedPosition"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Slicer. Indique si le slicer spécifié peut être déplacé ou redimensionné via l'interface utilisateur"
type: docs
url: /fr/net/aspose.cells.slicers/slicer/lockedposition/
---
## Slicer.LockedPosition property

Indique si le slicer spécifié peut être déplacé ou redimensionné via l'interface utilisateur.

```csharp
public bool LockedPosition { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerPropertyLockedPositionDemo
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

            // Créer une collection de tableaux croisés dynamiques
            PivotTableCollection pivotTables = worksheet.PivotTables;
            
            // Créer un tableau croisé dynamique
            int pivotIndex = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Ajouter le champ de ligne
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");

            // Ajouter le champ de données
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Créer une collection de slicers
            SlicerCollection slicers = worksheet.Slicers;
            
            // Ajouter un slicer pour le tableau croisé dynamique
            int slicerIndex = slicers.Add(pivotTable, "A1", "Fruit");
            Slicer slicer = slicers[slicerIndex];

            // Définir les propriétés du segmenteur
            slicer.Caption = "Fruit Slicer";
            slicer.NumberOfColumns = 2;
            slicer.WidthPixel = 200;
            slicer.HeightPixel = 150;

            // Démontrer la propriété LockedPosition
            slicer.LockedPosition = true; // Lock the slicer position
            Console.WriteLine("Slicer position locked: " + slicer.LockedPosition);

            // Modifier LockedPosition à false pour permettre le déplacement
            slicer.LockedPosition = false;
            Console.WriteLine("Slicer position locked: " + slicer.LockedPosition);

            // Enregistrez le classeur
            workbook.Save("SlicerLockedPositionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


