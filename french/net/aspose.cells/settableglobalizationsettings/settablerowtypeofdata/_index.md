---
title: "SettableGlobalizationSettings.SetTableRowTypeOfData"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettableGlobalizationSettings. Définit le nom du type des lignes de tableau qui composent la région de données du tableau référencé"
type: docs
url: /fr/net/aspose.cells/settableglobalizationsettings/settablerowtypeofdata/
---
## SettableGlobalizationSettings.SetTableRowTypeOfData method

Définit le nom du type des lignes de tableau qui comprennent la région de données du tableau référencé.

```csharp
public void SetTableRowTypeOfData(string name)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | le nom du type des lignes de tableau |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class SettableGlobalizationSettingsMethodSetTableRowTypeOfDataWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer un tableau
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(30);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(25);

            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.ShowTotals = true;
            table.ListColumns[1].TotalsCalculation = TotalsCalculation.Sum;

            // Créer des paramètres de mondialisation
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Définir un nom personnalisé pour les lignes de données dans le tableau
                settings.SetTableRowTypeOfData("MyDataRegion");
                
                // Appliquer les paramètres au classeur
                workbook.Settings.GlobalizationSettings = settings;

                Console.WriteLine("Table row type of data set to: MyDataRegion");
                Console.WriteLine("In formulas, '#MyDataRegion' will now represent the data region instead of '#Data'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTableRowTypeOfData method: {ex.Message}");
            }

            // Enregistrez le classeur
            workbook.Save("SetTableRowTypeOfDataDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


