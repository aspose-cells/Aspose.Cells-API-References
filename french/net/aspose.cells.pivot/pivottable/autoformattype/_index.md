---
title: "PivotTable.AutoFormatType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Obtient et définit le type de formatage automatique du PivotTable"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/autoformattype/
---
## PivotTable.AutoFormatType property

Obtient et définit le type de format automatique du PivotTable.

```csharp
public PivotTableAutoFormatType AutoFormatType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyAutoFormatTypeDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Product");
            worksheet.Cells["C1"].PutValue("Sales");
            
            worksheet.Cells["A2"].PutValue("Electronics");
            worksheet.Cells["B2"].PutValue("Laptop");
            worksheet.Cells["C2"].PutValue(1200);
            
            worksheet.Cells["A3"].PutValue("Electronics");
            worksheet.Cells["B3"].PutValue("Phone");
            worksheet.Cells["C3"].PutValue(800);
            
            worksheet.Cells["A4"].PutValue("Furniture");
            worksheet.Cells["B4"].PutValue("Chair");
            worksheet.Cells["C4"].PutValue(150);
            
            // Créer un tableau croisé dynamique
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:C4", "E5", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Ajouter des champs aux zones
            pivotTable.AddFieldToArea(PivotFieldType.Row, pivotTable.BaseFields["Category"]);
            pivotTable.AddFieldToArea(PivotFieldType.Column, pivotTable.BaseFields["Product"]);
            pivotTable.AddFieldToArea(PivotFieldType.Data, pivotTable.BaseFields["Sales"]);
            
            // Démontrer la propriété AutoFormatType
            pivotTable.IsAutoFormat = true;
            pivotTable.AutoFormatType = PivotTableAutoFormatType.Report6;
            
            // Enregistrez le classeur
            workbook.Save("PivotTableAutoFormatTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [PivotTableAutoFormatType](../../pivottableautoformattype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


