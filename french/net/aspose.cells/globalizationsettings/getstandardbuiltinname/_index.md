---
title: "GlobalizationSettings.GetStandardBuiltInName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode GlobalizationSettings. Obtient le texte standard du builtin Name selon le texte dépendant de la locale donnée"
type: docs
url: /fr/net/aspose.cells/globalizationsettings/getstandardbuiltinname/
---
## GlobalizationSettings.GetStandardBuiltInName method

Obtient le texte standard du nom intégré selon le texte dépendant de la langue fourni.

```csharp
public virtual string GetStandardBuiltInName(string localName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| localName | String | Texte dépendant de la locale du nom intégré. La locale a été spécifiée par le Workbook pour lequel ces paramètres sont utilisés. |

### Valeur de retour

Texte standard (locale en-US).

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetStandardBuiltInNameWithStringDemo
    {
        public static void Run()
        {
            // Créer un classeur avec des paramètres de mondialisation personnalisés
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Initialiser les paramètres de mondialisation personnalisés et les affecter au classeur
            var globalizationSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = globalizationSettings;

            // Paramètre de test pour GetStandardBuiltInName
            string localFunctionName = "MyLocalSum";
            
            try
            {
                // Appeler GetStandardBuiltInName avec le nom de fonction local
                string standardName = globalizationSettings.GetStandardBuiltInName(localFunctionName);
                Console.WriteLine($"Local name: '{localFunctionName}' => Standard name: '{standardName}'");

                // Démontrer l'effet en utilisant le nom local dans une formule
                worksheet.Cells["A1"].Value = 5;
                worksheet.Cells["A2"].Value = 7;
                worksheet.Cells["A3"].Formula = $"{localFunctionName}(A1:A2)";

                // Calculer la formule pour montrer l'interprétation correcte
                workbook.CalculateFormula();
                Console.WriteLine($"Formula result: {worksheet.Cells["A3"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardBuiltInName: {ex.Message}");
            }

            // Enregistrer le classeur modifié
            workbook.Save("GlobalizationGetStandardBuiltInNameDemo.xlsx");
        }
    }

    // Paramètres de mondialisation personnalisés surchargeant GetStandardBuiltInName
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetStandardBuiltInName(string localName)
        {
            // Mapper le nom de fonction local personnalisé à la fonction SUM standard
            if (localName.Equals("MyLocalSum", StringComparison.OrdinalIgnoreCase))
            {
                return "SUM";
            }
            return base.GetStandardBuiltInName(localName);
        }
    }
}
```

### Voir aussi

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


