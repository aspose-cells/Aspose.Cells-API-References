---
title: "SettablePivotGlobalizationSettings.SetTextOfEmptyData"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettablePivotGlobalizationSettings. Définit le texte de l'étiquette vide dans le tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells/settablepivotglobalizationsettings/settextofemptydata/
---
## SettablePivotGlobalizationSettings.SetTextOfEmptyData method

Définit le texte de l'étiquette "(blank)" dans le tableau croisé dynamique.

```csharp
public void SetTextOfEmptyData(string text)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| texte | String | Le texte des données vides |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfEmptyDataWithStringDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple (facultatif, juste pour le contexte)
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);

            // Créer une instance de SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Définissez un texte personnalisé pour les cellules de données vides dans un tableau croisé dynamique
                settings.SetTextOfEmptyData("(no data)");

                // Vérifier le changement
                string emptyDataText = settings.GetTextOfEmptyData();
                Console.WriteLine($"Custom text for empty data: {emptyDataText}");

                // (Optionnel) Enregistrez le classeur – même si nous n'avons pas créé de tableau croisé dynamique,
                // cela montre que le classeur peut encore être enregistré après la manipulation des paramètres.
                workbook.Save("SetTextOfEmptyDataDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfEmptyData: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


