---
title: "GlobalizationSettings.GetBooleanValueString"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode GlobalizationSettings. Obtient la valeur de chaîne d'affichage pour la valeur booléenne des cellules"
type: docs
url: /fr/net/aspose.cells/globalizationsettings/getbooleanvaluestring/
---
## GlobalizationSettings.GetBooleanValueString method

Obtient la chaîne d'affichage de la valeur booléenne de la cellule

```csharp
public virtual string GetBooleanValueString(bool bv)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| bv | Boolean | valeur booléenne |

### Valeur de retour

Par défaut, renvoie "TRUE" pour la valeur vraie et "FALSE" pour la valeur fausse.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetBooleanValueStringWithBooleanDemo
    {
        public static void Run()
        {
            // Cr\u00e9er un nouveau classeur avec des param\u00e8tres de mondialisation personnalis\u00e9s
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomBooleanGlobalizationSettings();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Démontrer GetBooleanValueString avec les deux valeurs booléennes
                var globalizationSettings = workbook.Settings.GlobalizationSettings;
                string trueResult = globalizationSettings.GetBooleanValueString(true);
                string falseResult = globalizationSettings.GetBooleanValueString(false);

                Console.WriteLine($"GetBooleanValueString(true) returns: {trueResult}");
                Console.WriteLine($"GetBooleanValueString(false) returns: {falseResult}");

                // Appliquer des valeurs booléennes aux cellules pour montrer l'effet sur la feuille de calcul
                worksheet.Cells["A1"].PutValue(true);
                worksheet.Cells["A2"].PutValue(false);

                workbook.Save("GlobalizationBooleanDemo.xlsx");
                Console.WriteLine("Workbook saved with custom boolean representations.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetBooleanValueString: {ex.Message}");
            }
        }
    }

    // Paramètres de mondialisation personnalisés qui remplacent la représentation de chaîne booléenne
    public class CustomBooleanGlobalizationSettings : GlobalizationSettings
    {
        public override string GetBooleanValueString(bool bv)
        {
            return bv ? "Enabled" : "Disabled";
        }
    }
}
```

### Voir aussi

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


