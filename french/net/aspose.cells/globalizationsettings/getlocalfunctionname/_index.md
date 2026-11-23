---
title: "GlobalizationSettings.GetLocalFunctionName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode GlobalizationSettings. Obtient le nom de fonction dépendant de la locale selon le nom de fonction standard donné"
type: docs
url: /fr/net/aspose.cells/globalizationsettings/getlocalfunctionname/
---
## GlobalizationSettings.GetLocalFunctionName method

Obtient le nom de fonction dépendant de la langue selon le nom de fonction standard fourni.

```csharp
public virtual string GetLocalFunctionName(string standardName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| standardName | String | Nom de fonction standard (locale en-US). |

### Valeur de retour

Nom de fonction dépendant de la locale. La locale a été spécifiée par le classeur pour lequel ces paramètres sont utilisés.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetLocalFunctionNameWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir des paramètres de globalisation personnalisés
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            // Ajoutez des données d'exemple
            worksheet.Cells["B1"].PutValue(5);
            worksheet.Cells["B2"].PutValue(15);

            // Créer une formule avec le nom de fonction localisé
            Cell cell = worksheet.Cells["B3"];
            cell.Formula = "=LOCALSUM(B1:B2)";

            try
            {
                workbook.CalculateFormula();
                Console.WriteLine($"Calculation result using localized function: {cell.DoubleValue}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Calculation error: {ex.Message}");
            }

            workbook.Save("GlobalizationSettingsFunctionDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override string GetLocalFunctionName(string standardName)
            {
                if (standardName == "SUM")
                {
                    return "LOCALSUM";
                }
                return base.GetLocalFunctionName(standardName);
            }
        }
    }
}
```

### Voir aussi

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


