---
title: "PivotTable.SaveData"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Indique si les données du rapport du tableau croisé dynamique sont enregistrées avec le classeur"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/savedata/
---
## PivotTable.SaveData property

Indique si les données du rapport du PivotTable sont enregistrées avec le classeur.

```csharp
public bool SaveData { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertySaveDataDemo
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
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Démontrer la propriété SaveData
            Console.WriteLine("SaveData before setting: " + pivotTable.SaveData);
            pivotTable.SaveData = false; // Disable saving pivot data with file
            Console.WriteLine("SaveData after setting: " + pivotTable.SaveData);
            
            // Enregistrez le classeur
            workbook.Save("PivotTable_SaveData_Demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


