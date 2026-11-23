---
title: "SettableGlobalizationSettings.SetStandardBuiltInName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettableGlobalizationSettings. Définit le nom de fonction dépendant de la locale selon le nom de fonction standard fourni"
type: docs
url: /fr/net/aspose.cells/settableglobalizationsettings/setstandardbuiltinname/
---
## SettableGlobalizationSettings.SetStandardBuiltInName method

Définit le nom de fonction dépendant de la langue selon le nom de fonction standard donné.

```csharp
public void SetStandardBuiltInName(string localName, string standardName, bool bidirectional)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| localName | String | Nom de fonction dépendant de la locale |
| standardName | String | Nom de fonction standard (locale en-US). |
| bidirectional | Boolean | Indique si le texte du nom standard doit être mappé automatiquement au texte du nom local. Si vrai, le texte du nom standard sera mappé automatiquement au texte du nom local, de sorte que l'utilisateur n'a pas besoin d'appeler [`SetLocalBuiltInName`](../setlocalbuiltinname/) à nouveau pour la même paire de noms standard et local. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetStandardBuiltInNameWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Créer des paramètres de mondialisation personnalisés
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Définissez les paramètres de mondialisation pour le classeur
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Appelez SetStandardBuiltInName pour mapper un nom local à un nom standard intégré
                // Paramètres : localName, standardName, bidirectionnel
                settings.SetStandardBuiltInName("MyLocalName", "SUM", true);
                
                Console.WriteLine("SetStandardBuiltInName executed successfully with parameters (\"MyLocalName\", \"SUM\", true)");
                
                // Démontrez l'effet en utilisant le nom local dans une formule
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(20);
                worksheet.Cells["A3"].Formula = "=MyLocalName(A1:A2)";
                
                // Calculez la formule pour montrer qu'elle fonctionne avec le nom local
                workbook.CalculateFormula();
                Console.WriteLine("Result of formula with local name: " + worksheet.Cells["A3"].Value);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetStandardBuiltInName method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("SetStandardBuiltInNameDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


