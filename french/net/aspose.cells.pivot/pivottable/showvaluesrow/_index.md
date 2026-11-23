---
title: "PivotTable.ShowValuesRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "PivotTable property. Indique si la ligne des valeurs est affichée"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/showvaluesrow/
---
## PivotTable.ShowValuesRow property

Indique si la ligne des valeurs est affichée.

```csharp
public bool ShowValuesRow { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowValuesRowDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Créer un tableau croisé dynamique
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Configurer le tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit as row
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Quantity as data
            
            // Démontrer la propriété ShowValuesRow
            Console.WriteLine("Initial ShowValuesRow: " + pivotTable.ShowValuesRow);
            pivotTable.ShowValuesRow = true;
            Console.WriteLine("After setting to true: " + pivotTable.ShowValuesRow);
            
            // Enregistrez le classeur
            workbook.Save("PivotTableShowValuesRowDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


