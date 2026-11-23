---
title: "SettableChartGlobalizationSettings.GetLegendDecreaseName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettableChartGlobalizationSettings. Obtient le nom de Diminution pour la légende"
type: docs
url: /fr/net/aspose.cells/settablechartglobalizationsettings/getlegenddecreasename/
---
## SettableChartGlobalizationSettings.GetLegendDecreaseName method

Obtient le nom de Decrease pour la légende

```csharp
public override string GetLegendDecreaseName()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetLegendDecreaseNameDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données simples pour le contexte (optionnel)
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // Créer un graphique (optionnel, juste pour avoir un classeur complet)
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Instancier l'objet des paramètres de mondialisation
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Définir une étiquette de diminution de légende personnalisée
                settings.SetLegendDecreaseName("Custom Decrease Label");

                // Récupérer l'étiquette en utilisant GetLegendDecreaseName
                string legendDecreaseName = settings.GetLegendDecreaseName();

                Console.WriteLine("Legend Decrease Name: " + legendDecreaseName);

                // Enregistrer le classeur (les paramètres ne sont pas directement attachés au graphique dans cette démo)
                workbook.Save("GetLegendDecreaseNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetLegendDecreaseName: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


