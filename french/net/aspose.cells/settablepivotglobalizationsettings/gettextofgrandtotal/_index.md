---
title: "SettablePivotGlobalizationSettings.GetTextOfGrandTotal"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettablePivotGlobalizationSettings. Obtient le texte de l'étiquette Grand Total dans le tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells/settablepivotglobalizationsettings/gettextofgrandtotal/
---
## SettablePivotGlobalizationSettings.GetTextOfGrandTotal method

Obtient le texte de l'étiquette "Grand Total" dans le tableau croisé dynamique.

```csharp
public override string GetTextOfGrandTotal()
```

### Valeur de retour

Le texte de l'étiquette "Grand Total"

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfGrandTotalDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur (juste pour le contexte)
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample");

            // Instance de SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Modifiez le texte par défaut "Grand Total"
                settings.SetTextOfGrandTotal("My Custom Grand Total");

                // Récupérez le texte actuel "Grand Total"
                string grandTotalText = settings.GetTextOfGrandTotal();

                Console.WriteLine($"Grand Total label text: {grandTotalText}");

                // Enregistrez le classeur (aucune table croisée dynamique n'est créée, mais le fichier est enregistré pour prouver l'exécution)
                workbook.Save("GetTextOfGrandTotalDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfGrandTotal: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


