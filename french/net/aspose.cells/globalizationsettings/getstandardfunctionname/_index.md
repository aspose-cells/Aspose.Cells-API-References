---
title: "GlobalizationSettings.GetStandardFunctionName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "M\\u00e9thode GlobalizationSettings. Obtient le nom de fonction standard selon le nom de fonction d\\u00e9pendant de la locale fourni."
type: docs
url: /fr/net/aspose.cells/globalizationsettings/getstandardfunctionname/
---
## GlobalizationSettings.GetStandardFunctionName method

Obtient le nom de fonction standard selon le nom de fonction dépendant de la langue fourni.

```csharp
public virtual string GetStandardFunctionName(string localName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| localName | String | Nom de fonction dépendant de la locale. La locale a été spécifiée par le classeur pour lequel ces paramètres sont utilisés. |

### Valeur de retour

Nom de fonction standard (locale en-US).

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetStandardFunctionNameWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Pr\u00e9parer les donn\u00e9es d'exemple
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["A2"].PutValue(15);
            
            // Cr\u00e9er des param\u00e8tres de mondialisation personnalis\u00e9s et les assigner au classeur
            var customSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = customSettings;

            try
            {
                // D\u00e9montrer GetStandardFunctionName avec le nom de fonction SUM en allemand
                string localName = "SUMME";
                string standardName = customSettings.GetStandardFunctionName(localName);
                
                Console.WriteLine($"Local function name: {localName}");
                Console.WriteLine($"Standard function name: {standardName}");

                // Appliquer le nom de fonction localis\u00e9 dans la formule
                worksheet.Cells["A3"].Formula = "=SUMME(A1:A2)";
                workbook.CalculateFormula();
                
                Console.WriteLine($"Formula result: {worksheet.Cells["A3"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardFunctionName method: {ex.Message}");
            }

            workbook.Save("MethodGetStandardFunctionNameDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override string GetStandardFunctionName(string localName)
            {
                // Convertir le nom de fonction allemand en anglais standard
                if (localName.Equals("SUMME", StringComparison.OrdinalIgnoreCase))
                {
                    return "SUM";
                }
                return base.GetStandardFunctionName(localName);
            }
        }
    }
}
```

### Voir aussi

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


