---
title: "SettableChartGlobalizationSettings.SetLegendIncreaseName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettableChartGlobalizationSettings. Définit le nom d'augmentation pour la légende"
type: docs
url: /fr/net/aspose.cells/settablechartglobalizationsettings/setlegendincreasename/
---
## SettableChartGlobalizationSettings.SetLegendIncreaseName method

Définit le nom de increase pour la légende

```csharp
public void SetLegendIncreaseName(string name)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | nom dépendant local |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodSetLegendIncreaseNameWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données minimales pour le contexte
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Item 1";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["B2"].Value = 100;

            try
            {
                // Créer une instance de SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Définir un nom d'augmentation de légende personnalisé
                settings.SetLegendIncreaseName("Custom Increase Label");

                // Vérifiez le paramètre en récupérant la valeur
                string legendIncreaseName = settings.GetLegendIncreaseName();
                Console.WriteLine("Legend Increase Name set to: " + legendIncreaseName);

                // Enregistrez le classeur
                workbook.Save("SetLegendIncreaseNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetLegendIncreaseName: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


