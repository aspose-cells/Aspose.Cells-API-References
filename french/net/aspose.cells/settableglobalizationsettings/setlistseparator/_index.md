---
title: "SettableGlobalizationSettings.SetListSeparator"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettableGlobalizationSettings. Définit le séparateur pour les paramètres de liste de la fonction ...etc"
type: docs
url: /fr/net/aspose.cells/settableglobalizationsettings/setlistseparator/
---
## SettableGlobalizationSettings.SetListSeparator method

Définit le séparateur pour la liste, les paramètres de la fonction, ...etc.

```csharp
public void SetListSeparator(char c)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| c | Char | le séparateur spécifié |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetListSeparatorWithCharDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer des paramètres de mondialisation personnalisés
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            try
            {
                // Appelez la méthode SetListSeparator avec un paramètre de type caractère
                settings.SetListSeparator(';');
                
                // Appliquer les paramètres au classeur
                workbook.Settings.GlobalizationSettings = settings;
                
                // Démontrez l'effet en créant une formule avec le séparateur de liste
                worksheet.Cells["A1"].Formula = "SUM(1;2;3)";
                worksheet.Cells["A2"].Value = "Formula using custom list separator: SUM(1;2;3)";
                
                Console.WriteLine("SetListSeparator method executed successfully with parameter ';'");
                Console.WriteLine("Formula using custom list separator created in cell A1");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetListSeparator method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("SetListSeparatorWithCharDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


