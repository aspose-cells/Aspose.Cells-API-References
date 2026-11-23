---
title: "SettablePivotGlobalizationSettings.GetTextOfTotal"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettablePivotGlobalizationSettings. Obtient le texte de l'étiquette Total dans le tableau croisé dynamique. Vous devez remplacer cette méthode lorsque le tableau croisé dynamique contient deux champs ou plus dans la zone de données."
type: docs
url: /fr/net/aspose.cells/settablepivotglobalizationsettings/gettextoftotal/
---
## SettablePivotGlobalizationSettings.GetTextOfTotal method

Obtient le texte de l'étiquette "Total" dans le tableau croisé dynamique. Vous devez remplacer cette méthode lorsque le tableau croisé dynamique contient deux champs ou plus dans la zone de données.

```csharp
public override string GetTextOfTotal()
```

### Valeur de retour

Le texte de l'étiquette "Total"

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfTotalDemo
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
                // Définir un texte personnalisé pour l'étiquette "Total"
                settings.SetTextOfTotal("Custom Total");

                // Obtenir le texte de l'étiquette "Total"
                string totalText = settings.GetTextOfTotal();

                Console.WriteLine($"Text of Total: {totalText}");

                // Enregistrez le classeur
                workbook.Save("GetTextOfTotalDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfTotal: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


