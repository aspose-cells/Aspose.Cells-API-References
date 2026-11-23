---
title: "SettableGlobalizationSettings.SetLocalBuiltInName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettableGlobalizationSettings. Définit le texte dépendant de la locale pour le nom intégré avec le texte du nom standard fourni"
type: docs
url: /fr/net/aspose.cells/settableglobalizationsettings/setlocalbuiltinname/
---
## SettableGlobalizationSettings.SetLocalBuiltInName method

Définit le texte dépendant de la langue pour le nom intégré avec le texte du nom standard donné.

```csharp
public void SetLocalBuiltInName(string standardName, string localName, bool bidirectional)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| standardName | String | Texte du nom standard (locale en-US) du nom intégré. |
| localName | String | Texte du nom dépendant de la locale |
| bidirectional | Boolean | Indique si le texte du nom local doit être automatiquement mappé au texte du nom standard. Si vrai, le texte du nom local sera automatiquement mappé au texte du nom standard de sorte que l'utilisateur n'ait pas besoin d'appeler [`SetStandardBuiltInName`](../setstandardbuiltinname/) à nouveau pour la même paire de noms standard et local |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetLocalBuiltInNameWithStringStringBooleanDemo
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
                // Appeler SetLocalBuiltInName pour mapper un nom intégré standard à un nom local
                settings.SetLocalBuiltInName("SUM", "LOCAL_SUM", true);

                // Appliquer les paramètres au classeur
                workbook.Settings.GlobalizationSettings = settings;

                // Créer une formule en utilisant le nom intégré standard
                worksheet.Cells["A1"].Formula = "=SUM(B1:B3)";
                worksheet.Cells["B1"].Value = 5;
                worksheet.Cells["B2"].Value = 10;
                worksheet.Cells["B3"].Value = 15;

                // Calculer la formule
                workbook.CalculateFormula();

                Console.WriteLine("Formula with standard built-in name 'SUM' calculated successfully.");
                Console.WriteLine($"Result: {worksheet.Cells["A1"].Value}");

                // Vérifier le mappage du nom local
                string localName = settings.GetLocalBuiltInName("SUM");
                Console.WriteLine($"Local name for 'SUM': {localName}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetLocalBuiltInName method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("SetLocalBuiltInNameDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


