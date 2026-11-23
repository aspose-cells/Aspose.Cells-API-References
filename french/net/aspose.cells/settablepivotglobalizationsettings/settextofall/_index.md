---
title: "SettablePivotGlobalizationSettings.SetTextOfAll"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettablePivotGlobalizationSettings. Définit le texte de l'étiquette All dans le PivotTable"
type: docs
url: /fr/net/aspose.cells/settablepivotglobalizationsettings/settextofall/
---
## SettablePivotGlobalizationSettings.SetTextOfAll method

Définit le texte de l'étiquette "(All)" dans le tableau croisé dynamique.

```csharp
public void SetTextOfAll(string text)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| texte | String | texte personnalisé |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfAllWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Créer un tableau croisé dynamique
            var pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            var pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Créer des paramètres de mondialisation
            var settings = new SettableGlobalizationSettings();
            settings.PivotSettings = new SettablePivotGlobalizationSettings();

            try
            {
                // Appeler la méthode SetTextOfAll pour modifier le texte "(All)"
                ((SettablePivotGlobalizationSettings)settings.PivotSettings).SetTextOfAll("All Products");

                // Appliquer les paramètres au classeur
                workbook.Settings.GlobalizationSettings = settings;
                pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium2;

                Console.WriteLine("SetTextOfAll method executed successfully. Changed '(All)' to 'All Products'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTextOfAll method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("SettablePivotGlobalizationSettingsMethodSetTextOfAllDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


