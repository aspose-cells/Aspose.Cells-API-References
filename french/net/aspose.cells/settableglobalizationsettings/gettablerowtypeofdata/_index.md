---
title: "SettableGlobalizationSettings.GetTableRowTypeOfData"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettableGlobalizationSettings. Obtient le nom du type des lignes de tableau qui constituent la région de données de la table référencée. La valeur par défaut est Data, ainsi dans la formule Data représente la région de données de la table"
type: docs
url: /fr/net/aspose.cells/settableglobalizationsettings/gettablerowtypeofdata/
---
## SettableGlobalizationSettings.GetTableRowTypeOfData method

Obtient le nom du type des lignes de tableau qui comprend la région de données du tableau référencé. La valeur par défaut est "Data", donc dans la formule "#Data" représente la région de données du tableau.

```csharp
public override string GetTableRowTypeOfData()
```

### Valeur de retour

le nom du type des lignes de tableau

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class SettableGlobalizationSettingsMethodGetTableRowTypeOfDataDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
                settings.SetTableRowTypeOfData("CustomData");
                string rowType = settings.GetTableRowTypeOfData();
                Console.WriteLine($"TableRowTypeOfData: {rowType}");

                workbook.Settings.GlobalizationSettings = settings;

                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["A3"].PutValue("Orange");
                worksheet.Cells["B1"].PutValue("Price");
                worksheet.Cells["B2"].PutValue(5.5);
                worksheet.Cells["B3"].PutValue(3.8);

                int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
                ListObject table = worksheet.ListObjects[tableIndex];
                table.DisplayName = "Inventory"; // Changed from Name to DisplayName
                
                worksheet.Cells["B4"].Formula = "=SUM(Inventory[#CustomData][Price])";
                
                workbook.CalculateFormula();
                Console.WriteLine($"Total price: {worksheet.Cells["B4"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("MethodGetTableRowTypeOfDataDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


