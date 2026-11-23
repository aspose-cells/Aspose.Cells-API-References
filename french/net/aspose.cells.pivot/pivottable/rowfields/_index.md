---
title: "PivotTable.RowFields"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Retourne une PivotFieldCollection qui sont actuellement affichées comme champs de ligne"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/rowfields/
---
## PivotTable.RowFields property

Retourne une [`PivotFieldCollection`](../../pivotfieldcollection/) qui sont actuellement affichées comme champs de ligne.

```csharp
public PivotFieldCollection RowFields { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyRowFieldsDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Bike";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            
            cells["A3"].Value = "Bike";
            cells["B3"].Value = "South";
            cells["C3"].Value = 800;
            
            cells["A4"].Value = "Car";
            cells["B4"].Value = "North";
            cells["C4"].Value = 1500;
            
            cells["A5"].Value = "Car";
            cells["B5"].Value = "South";
            cells["C5"].Value = 1200;

            // Créer un tableau croisé dynamique
            int pivotIndex = sheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Ajouter des champs de ligne
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Region");
            
            // Ajouter le champ de données
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Démontrer la propriété RowFields
            Console.WriteLine("Row Fields Count: " + pivotTable.RowFields.Count);
            Console.WriteLine("First Row Field Name: " + pivotTable.RowFields[0].Name);
            Console.WriteLine("Second Row Field Name: " + pivotTable.RowFields[1].Name);
            
            // Enregistrez le classeur
            workbook.Save("PivotTableRowFieldsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


