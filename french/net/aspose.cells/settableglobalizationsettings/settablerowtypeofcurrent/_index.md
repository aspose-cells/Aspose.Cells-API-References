---
title: "SettableGlobalizationSettings.SetTableRowTypeOfCurrent"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettableGlobalizationSettings. Définit le nom du type des lignes de tableau qui comprend la ligne actuelle dans la table référencée"
type: docs
url: /fr/net/aspose.cells/settableglobalizationsettings/settablerowtypeofcurrent/
---
## SettableGlobalizationSettings.SetTableRowTypeOfCurrent method

Définit le nom du type des lignes de tableau qui comprennent la ligne actuelle du tableau référencé.

```csharp
public void SetTableRowTypeOfCurrent(string name)
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

    public class SettableGlobalizationSettingsMethodSetTableRowTypeOfCurrentWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer un tableau
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Price");
            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue("2.5");
            cells["A3"].PutValue("Banana");
            cells["B3"].PutValue("1.5");
            
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.ShowTotals = true;
            table.ListColumns[1].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;

            // Créer des paramètres de mondialisation
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            try
            {
                // Définissez un nom personnalisé pour le type de ligne actuelle
                settings.SetTableRowTypeOfCurrent("CurrentItem");
                
                // Appliquer les paramètres au classeur
                workbook.Settings.GlobalizationSettings = settings;

                // Vérifiez le paramètre en récupérant la valeur
                string currentRowType = settings.GetTableRowTypeOfCurrent();
                Console.WriteLine($"Current row type name set to: {currentRowType}");

                // Enregistrez le classeur
                workbook.Save("SetTableRowTypeOfCurrentDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTableRowTypeOfCurrent method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


