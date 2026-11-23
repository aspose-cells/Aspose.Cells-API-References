---
title: "SettableChartGlobalizationSettings.GetChartTitleName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettableChartGlobalizationSettings. Obtient le nom du titre du graphique"
type: docs
url: /fr/net/aspose.cells/settablechartglobalizationsettings/getcharttitlename/
---
## SettableChartGlobalizationSettings.GetChartTitleName method

Obtient le nom de Chart Title

```csharp
public override string GetChartTitleName()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetChartTitleNameDemo
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

                // Définissez un nom de titre de graphique personnalisé
                settings.SetChartTitleName("Custom Chart Title");

                // Obtenez le nom du titre du graphique en utilisant GetChartTitleName
                string chartTitleName = settings.GetChartTitleName();

                // Afficher le résultat
                Console.WriteLine("Chart Title Name: " + chartTitleName);

                // Enregistrez le classeur
                workbook.Save("GetChartTitleNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetChartTitleName: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


