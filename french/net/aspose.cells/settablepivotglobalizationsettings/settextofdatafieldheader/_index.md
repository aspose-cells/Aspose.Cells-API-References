---
title: "SettablePivotGlobalizationSettings.SetTextOfDataFieldHeader"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettablePivotGlobalizationSettings. Définit le texte de l'en-tête du champ de la zone de valeurs dans le tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells/settablepivotglobalizationsettings/settextofdatafieldheader/
---
## SettablePivotGlobalizationSettings.SetTextOfDataFieldHeader method

Définit le texte de l'en-tête du champ de la zone de valeurs dans le tableau croisé dynamique.

```csharp
public void SetTextOfDataFieldHeader(string text)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| texte | String | Le texte du nom de l'en-tête du champ de données |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfDataFieldHeaderWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);

            // Créer une instance de SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Définir un texte personnalisé pour l’en-tête du champ de données
                settings.SetTextOfDataFieldHeader("Custom Data Header");

                // Vérifier le changement en obtenant le texte actuel
                string currentHeaderText = settings.GetTextOfDataFieldHeader();
                Console.WriteLine($"Data field header text: {currentHeaderText}");

                // Enregistrez le classeur pour démontrer une exécution réussie
                workbook.Save("SetTextOfDataFieldHeaderDemo.xlsx");
                Console.WriteLine("SetTextOfDataFieldHeader method executed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfDataFieldHeader: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


