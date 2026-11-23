---
title: "GlobalizationSettings.GetLocalBuiltInName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode GlobalizationSettings. Obtient le texte dépendant de la locale pour le nom intégré selon le texte standard fourni"
type: docs
url: /fr/net/aspose.cells/globalizationsettings/getlocalbuiltinname/
---
## GlobalizationSettings.GetLocalBuiltInName method

Obtient le texte dépendant de la langue pour le nom intégré selon le texte standard fourni.

```csharp
public virtual string GetLocalBuiltInName(string standardName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| standardName | String | Texte Standard (locale en-US) du built-in Name. |

### Valeur de retour

Texte dépendant de la locale. La locale a été spécifiée par le classeur pour lequel ces paramètres sont utilisés.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetLocalBuiltInNameWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                string standardName = "Total";
                string localizedName = ((CustomGlobalizationSettings)workbook.Settings.GlobalizationSettings).GetLocalBuiltInName(standardName);

                Console.WriteLine($"Standard Name: {standardName}");
                Console.WriteLine($"Localized Name: {localizedName}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetLocalBuiltInName method: {ex.Message}");
            }

            workbook.Save("LocalizedBuiltInNameDemo.xlsx");
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetLocalBuiltInName(string standardName)
        {
            switch (standardName)
            {
                case "Total":
                    return "LocalizedTotal";
                case "Average":
                    return "LocalizedAverage";
                default:
                    return base.GetLocalBuiltInName(standardName);
            }
        }
    }
}
```

### Voir aussi

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


