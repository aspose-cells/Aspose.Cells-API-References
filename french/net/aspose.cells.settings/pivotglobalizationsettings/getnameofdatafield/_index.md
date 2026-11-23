---
title: "PivotGlobalizationSettings.GetNameOfDataField"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotGlobalizationSettings. Obtient le nom d'affichage du champ pivot de données. Le format par défaut est Sum Of Field"
type: docs
url: /fr/net/aspose.cells.settings/pivotglobalizationsettings/getnameofdatafield/
---
## PivotGlobalizationSettings.GetNameOfDataField method

Obtient le nom d'affichage du champ de données du tableau croisé dynamique. Le format par défaut est "Sum Of Field".

```csharp
public virtual string GetNameOfDataField(ConsolidationFunction function, string name)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fonction | ConsolidationFunction | La fonction est utilisée pour résumer les valeurs du champ pivot. |
| name | String | Le nom original du champ pivot. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Settings;
    using System;

    public class PivotGlobalizationSettingsMethodGetNameOfDataFieldWithConsolidationFuStringDemo
    {
        public static void Run()
        {
            try
            {
                // Créer une instance de PivotGlobalizationSettings
                PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

                // Définir les paramètres pour la méthode GetNameOfDataField
                ConsolidationFunction function = ConsolidationFunction.Sum;
                string fieldName = "Sales";

                // Appeler la méthode GetNameOfDataField
                string result = globalizationSettings.GetNameOfDataField(function, fieldName);

                // Afficher le résultat
                Console.WriteLine($"Localized name for data field '{fieldName}' with function '{function}': {result}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetNameOfDataField: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* enum [ConsolidationFunction](../../../aspose.cells/consolidationfunction/)
* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


