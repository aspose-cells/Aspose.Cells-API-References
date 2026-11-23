---
title: "SettableChartGlobalizationSettings.SetAxisTitleName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettableChartGlobalizationSettings. Définit le nom du titre pour l'axe"
type: docs
url: /fr/net/aspose.cells/settablechartglobalizationsettings/setaxistitlename/
---
## SettableChartGlobalizationSettings.SetAxisTitleName method

Définit le nom du Title pour l'axe

```csharp
public void SetAxisTitleName(string name)
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

    public class SettableChartGlobalizationSettingsMethodSetAxisTitleNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données minimales pour le contexte
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Créer une instance de SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Définir un nom de titre d'axe personnalisé
                settings.SetAxisTitleName("Custom Axis Title");

                // Vérifiez le paramètre en récupérant le nom du titre de l'axe
                string axisTitleName = settings.GetAxisTitleName();
                Console.WriteLine("Axis Title Name: " + axisTitleName);

                // Enregistrez le classeur
                workbook.Save("SetAxisTitleNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetAxisTitleName: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


