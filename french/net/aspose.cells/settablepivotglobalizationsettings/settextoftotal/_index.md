---
title: "SettablePivotGlobalizationSettings.SetTextOfTotal"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettablePivotGlobalizationSettings. Définit le texte de l'étiquette Total dans le tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells/settablepivotglobalizationsettings/settextoftotal/
---
## SettablePivotGlobalizationSettings.SetTextOfTotal method

Définit le texte de l'étiquette "Total" dans le tableau croisé dynamique.

```csharp
public void SetTextOfTotal(string text)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| texte | String | texte personnalisé |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfTotalWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter quelques données d'exemple pour le contexte
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["B3"].Value = 200;

            // Créer une instance de SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Obtenez le texte par défaut "Total"
                string defaultTotalText = settings.GetTextOfTotal();
                Console.WriteLine($"Default Total text: {defaultTotalText}");

                // Définissez un texte personnalisé pour "Total"
                settings.SetTextOfTotal("Custom Total Label");

                // Vérifier le changement
                string updatedTotalText = settings.GetTextOfTotal();
                Console.WriteLine($"Updated Total text: {updatedTotalText}");

                // Enregistrez le classeur
                workbook.Save("SetTextOfTotalDemo.xlsx");
                Console.WriteLine("SetTextOfTotal method called successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfTotal: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


