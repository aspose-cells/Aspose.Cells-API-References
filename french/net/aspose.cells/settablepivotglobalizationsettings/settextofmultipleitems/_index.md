---
title: "SettablePivotGlobalizationSettings.SetTextOfMultipleItems"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettablePivotGlobalizationSettings. Définit le texte de l'étiquette Multiple Items dans le tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells/settablepivotglobalizationsettings/settextofmultipleitems/
---
## SettablePivotGlobalizationSettings.SetTextOfMultipleItems method

Définit le texte de l'étiquette "(Multiple Items)" dans le tableau croisé dynamique.

```csharp
public void SetTextOfMultipleItems(string text)
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

    public class SettablePivotGlobalizationSettingsMethodSetTextOfMultipleItemsWithStringDemo
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
                // Définissez un texte personnalisé pour l'étiquette "(Multiple Items)" dans un tableau croisé dynamique
                settings.SetTextOfMultipleItems("(Multiple Items Edited)");

                // Récupérez et affichez le texte mis à jour
                string currentText = settings.GetTextOfMultipleItems();
                Console.WriteLine($"Current text of '(Multiple Items)' label: {currentText}");

                // (Facultatif) Enregistrez le classeur – aucune table croisée dynamique n'est requise pour cette démonstration
                workbook.Save("SetTextOfMultipleItemsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfMultipleItems: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


