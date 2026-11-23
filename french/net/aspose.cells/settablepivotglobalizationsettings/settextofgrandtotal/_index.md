---
title: "SettablePivotGlobalizationSettings.SetTextOfGrandTotal"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettablePivotGlobalizationSettings. Définit le texte de l'étiquette Grand Total dans le tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells/settablepivotglobalizationsettings/settextofgrandtotal/
---
## SettablePivotGlobalizationSettings.SetTextOfGrandTotal method

Définit le texte de l'étiquette "Grand Total" dans le tableau croisé dynamique.

```csharp
public void SetTextOfGrandTotal(string text)
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

    public class SettablePivotGlobalizationSettingsMethodSetTextOfGrandTotalWithStringDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur (contexte uniquement)
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");

            // Instance de SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Définissez un texte personnalisé pour l'étiquette "Grand Total"
                settings.SetTextOfGrandTotal("My Custom Grand Total");

                // Récupérez le texte de l'étiquette mis à jour pour vérifier la modification
                string grandTotalText = settings.GetTextOfGrandTotal();

                Console.WriteLine($"Grand Total label text: {grandTotalText}");

                // Enregistrez le classeur simplement pour démontrer que le code s'exécute sans erreurs
                workbook.Save("SetTextOfGrandTotalDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfGrandTotal: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


