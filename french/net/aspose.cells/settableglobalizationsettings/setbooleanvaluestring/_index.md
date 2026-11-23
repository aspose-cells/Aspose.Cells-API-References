---
title: "SettableGlobalizationSettings.SetBooleanValueString"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettableGlobalizationSettings. Définit la chaîne d’affichage pour la valeur booléenne des cellules"
type: docs
url: /fr/net/aspose.cells/settableglobalizationsettings/setbooleanvaluestring/
---
## SettableGlobalizationSettings.SetBooleanValueString method

Définit la valeur de chaîne d'affichage pour la valeur booléenne de la cellule

```csharp
public void SetBooleanValueString(bool bv, string name)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| bv | Boolean | valeur booléenne |
| name | String | valeur chaîne de la valeur booléenne |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetBooleanValueStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer des paramètres de mondialisation personnalisés
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Définir les chaînes de valeurs booléennes personnalisées
            settings.SetBooleanValueString(true, "Yes");
            settings.SetBooleanValueString(false, "No");
            
            // Appliquer les paramètres au classeur
            workbook.Settings.GlobalizationSettings = settings;
            
            // Définir les valeurs booléennes dans les cellules
            worksheet.Cells["A1"].PutValue(true);
            worksheet.Cells["A2"].PutValue(false);
            
            // Définir le style d’affichage pour montrer les valeurs booléennes en texte
            Style style = workbook.CreateStyle();
            style.Custom = "BOOLEAN";
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["A2"].SetStyle(style);
            
            try
            {
                // Enregistrez le classeur
                workbook.Save("SetBooleanValueStringDemo.xlsx");
                Console.WriteLine("Workbook saved with custom boolean value strings.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving workbook: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


