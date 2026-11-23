---
title: "GlobalizationSettings.GetStandardHeaderFooterFontStyleName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode GlobalizationSettings. Obtient le nom du style de police anglais standard Regular Bold Italic pour En-tête/Pied de page selon le nom du style de police de la locale donnée"
type: docs
url: /fr/net/aspose.cells/globalizationsettings/getstandardheaderfooterfontstylename/
---
## GlobalizationSettings.GetStandardHeaderFooterFontStyleName method

Obtient le nom de style de police anglais standard (Regular, Bold, Italic) pour En-tête/Pied de page selon le nom de style de police dépendant de la langue fourni.

```csharp
public virtual string GetStandardHeaderFooterFontStyleName(string localfontStyleName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| localfontStyleName | String | Nom du style de police local pour l'en-tête/pied de page. |

### Valeur de retour

Nom du style de police anglais standard (Regular, Bold, Italic)

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetStandardHeaderFooterFontStyleNameWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une instance de paramètres de mondialisation personnalisés
            var globalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // Démontrer l'appel de méthode avec le type de paramètre (String)
                string localStyle = "CustomBold";
                string standardStyle = globalizationSettings.GetStandardHeaderFooterFontStyleName(localStyle);
                Console.WriteLine($"Converted font style: {localStyle} -> {standardStyle}");

                // Appliquer les paramètres de mondialisation au classeur
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                // Définir l'en-tête avec un style de police personnalisé qui sera converti
                // Utiliser la méthode SetHeader avec le paramètre de section (0 = gauche, 1 = centre, 2 = droite)
                worksheet.PageSetup.SetHeader(1, "&\"Arial\"&\"CustomBold\"&12Header Text");

                // Enregistrer le classeur pour montrer l'effet
                workbook.Save("MethodGetStandardHeaderFooterFontStyleNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardHeaderFooterFontStyleName method: {ex.Message}");
            }
        }
    }

    // Implémentation des paramètres de globalisation personnalisés
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetStandardHeaderFooterFontStyleName(string localfontStyleName)
        {
            // Convertir les noms de styles de police personnalisés en noms standard
            return localfontStyleName switch
            {
                "CustomBold" => "Bold",
                "CustomItalic" => "Italic",
                _ => base.GetStandardHeaderFooterFontStyleName(localfontStyleName)
            };
        }
    }
}
```

### Voir aussi

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


