---
title: "Slicer.StyleType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Slicer. Spécifiez le type de style de slicer intégré. Le type par défaut est SlicerStyleLight1"
type: docs
url: /fr/net/aspose.cells.slicers/slicer/styletype/
---
## Slicer.StyleType property

Spécifiez le type de style de segmenteur intégré. Le type par défaut est SlicerStyleLight1.

```csharp
public SlicerStyleType StyleType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerPropertyStyleTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["B4"].PutValue(20);

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Ajouter le champ de ligne
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            // Ajouter un slicer
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "A1", "FruitSlicer");
            Slicer slicer = worksheet.Slicers[slicerIndex];

            // Définir les propriétés du slicer, y compris StyleType
            slicer.StyleType = SlicerStyleType.SlicerStyleDark2;
            slicer.Caption = "Fruit Selection";
            slicer.NumberOfColumns = 2;
            slicer.Width = 200;
            slicer.Height = 100;

            // Enregistrez le classeur
            workbook.Save("SlicerStyleTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [SlicerStyleType](../../slicerstyletype/)
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


