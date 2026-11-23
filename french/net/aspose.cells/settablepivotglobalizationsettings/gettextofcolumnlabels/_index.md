---
title: "SettablePivotGlobalizationSettings.GetTextOfColumnLabels"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettablePivotGlobalizationSettings. Obtient le texte de l'étiquette Column Labels dans le PivotTable"
type: docs
url: /fr/net/aspose.cells/settablepivotglobalizationsettings/gettextofcolumnlabels/
---
## SettablePivotGlobalizationSettings.GetTextOfColumnLabels method

Obtient le texte de l'étiquette "Column Labels" dans le tableau croisé dynamique.

```csharp
public override string GetTextOfColumnLabels()
```

### Valeur de retour

Le texte des étiquettes de colonne

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfColumnLabelsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le contexte
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // Créer une instance de SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Obtenir le texte par défaut des étiquettes de colonne
                string columnLabelsText = settings.GetTextOfColumnLabels();
                Console.WriteLine($"Default text of Column Labels: {columnLabelsText}");

                // Définir un texte personnalisé pour les étiquettes de colonne
                settings.SetTextOfColumnLabels("Custom Column Headers");

                // Obtenir le texte mis à jour des étiquettes de colonne
                string updatedColumnLabelsText = settings.GetTextOfColumnLabels();
                Console.WriteLine($"Updated text of Column Labels: {updatedColumnLabelsText}");

                // Enregistrez le classeur
                workbook.Save("GetTextOfColumnLabelsDemo.xlsx");
                Console.WriteLine("GetTextOfColumnLabels method executed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfColumnLabels: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


