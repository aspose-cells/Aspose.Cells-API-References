---
title: "SettablePivotGlobalizationSettings.GetTextOfMultipleItems"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettablePivotGlobalizationSettings. Obtient le texte de l’étiquette Multiple Items dans le tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells/settablepivotglobalizationsettings/gettextofmultipleitems/
---
## SettablePivotGlobalizationSettings.GetTextOfMultipleItems method

Obtient le texte de l'étiquette "(Multiple Items)" dans le tableau croisé dynamique.

```csharp
public override string GetTextOfMultipleItems()
```

### Valeur de retour

Le texte de l’étiquette "(Multiple Items)"

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfMultipleItemsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter quelques données d'exemple pour le contexte
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
                // Obtenir le texte par défaut pour plusieurs éléments
                string multipleItemsText = settings.GetTextOfMultipleItems();
                Console.WriteLine($"Default text for multiple items: {multipleItemsText}");

                // Définir un texte personnalisé pour plusieurs éléments
                settings.SetTextOfMultipleItems("(Multiple Items Custom)");
                multipleItemsText = settings.GetTextOfMultipleItems();
                Console.WriteLine($"Updated text for multiple items: {multipleItemsText}");

                // Enregistrez le classeur
                workbook.Save("GetTextOfMultipleItemsDemo.xlsx");
                Console.WriteLine("GetTextOfMultipleItems method called successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfMultipleItems: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


