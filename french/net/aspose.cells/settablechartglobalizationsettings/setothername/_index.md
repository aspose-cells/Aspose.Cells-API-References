---
title: "SettableChartGlobalizationSettings.SetOtherName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettableChartGlobalizationSettings. Définit le nom des autres libellés pour le graphique"
type: docs
url: /fr/net/aspose.cells/settablechartglobalizationsettings/setothername/
---
## SettableChartGlobalizationSettings.SetOtherName method

Définit le nom des libellés "Other" pour le graphique

```csharp
public void SetOtherName(string name)
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

    public class SettableChartGlobalizationSettingsMethodSetOtherNameWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données minimales pour le contexte
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(150);

            try
            {
                // Créer une instance de SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Définir un nom personnalisé pour le libellé "Other"
                settings.SetOtherName("Miscellaneous Items");

                // Vérifiez le paramètre en récupérant la valeur
                string otherName = settings.GetOtherName();
                Console.WriteLine("Other Name set to: " + otherName);

                // Enregistrez le classeur
                workbook.Save("SetOtherNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetOtherName: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


