---
title: "SettablePivotGlobalizationSettings.SetTextOfProtectedName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettablePivotGlobalizationSettings. Définit le texte pour un nom protégé spécifique"
type: docs
url: /fr/net/aspose.cells/settablepivotglobalizationsettings/settextofprotectedname/
---
## SettablePivotGlobalizationSettings.SetTextOfProtectedName method

Définit le texte pour un nom protégé spécifique.

```csharp
public void SetTextOfProtectedName(string protectedName, string text)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| protectedName | String | Le nom protégé dans le tableau croisé dynamique. |
| texte | String | Les noms protégés locaux du tableau croisé dynamique. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfProtectedNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter quelques données d'exemple pour le contexte
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Créer une instance de SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Définir un texte personnalisé pour un nom protégé
                settings.SetTextOfProtectedName("Sum", "Custom Sum Label");

                // Vérifier le changement en obtenant le texte actuel
                string currentText = settings.GetTextOfProtectedName("Sum");
                Console.WriteLine($"Text for protected name 'Sum': {currentText}");

                // Enregistrez le classeur pour démontrer une exécution réussie
                workbook.Save("SetTextOfProtectedNameDemo.xlsx");
                Console.WriteLine("SetTextOfProtectedName method executed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfProtectedName: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


