---
title: "SettableChartGlobalizationSettings.GetOtherName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettableChartGlobalizationSettings. Obtient le nom des libellés Autre pour le graphique"
type: docs
url: /fr/net/aspose.cells/settablechartglobalizationsettings/getothername/
---
## SettableChartGlobalizationSettings.GetOtherName method

Obtient le nom des libellés "Other" pour le graphique

```csharp
public override string GetOtherName()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetOtherNameDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données minimales (optionnel, juste pour un classeur complet)
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(120);
            worksheet.Cells["B3"].PutValue(250);

            try
            {
                // Instancier l'objet des paramètres de mondialisation
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Définir un nom personnalisé pour le libellé "Other"
                settings.SetOtherName("Custom Other Label");

                // Récupérer le nom en utilisant GetOtherName
                string otherName = settings.GetOtherName();

                Console.WriteLine("Other Name retrieved: " + otherName);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetOtherName: {ex.Message}");
            }

            // Enregistrer le classeur (les paramètres ne sont pas directement attachés au graphique dans cette démo)
            workbook.Save("GetOtherNameDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


