---
title: "SettableGlobalizationSettings.GetStandardHeaderFooterFontStyleName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettableGlobalizationSettings. Obtient le nom de style de police anglais standard Regular Bold Italic pour l'en-tête/pied de page selon le nom de style de police local donné"
type: docs
url: /fr/net/aspose.cells/settableglobalizationsettings/getstandardheaderfooterfontstylename/
---
## SettableGlobalizationSettings.GetStandardHeaderFooterFontStyleName method

Obtient le nom de style de police anglais standard (Regular, Bold, Italic) pour En-tête/Pied de page selon le nom de style de police dépendant de la langue fourni.

```csharp
public override string GetStandardHeaderFooterFontStyleName(string localfontStyleName)
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

    public class SettableGlobalizationSettingsMethodGetStandardHeaderFooterFontStyleNameWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des paramètres de mondialisation personnalisés
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Définissez un mappage de nom de style de police d'en-tête/pied de page standard
            settings.SetStandardHeaderFooterFontStyleName("MyLocalFontStyle", "Arial");

            // Appliquer les paramètres au classeur
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Appelez la méthode GetStandardHeaderFooterFontStyleName avec un nom de style de police local
                string standardFontStyle = settings.GetStandardHeaderFooterFontStyleName("MyLocalFontStyle");
                
                // Afficher le résultat
                Console.WriteLine($"Standard font style name for 'MyLocalFontStyle': {standardFontStyle}");

                // Créez un en-tête avec le nom de style de police local
                worksheet.PageSetup.SetHeader(1, "&\"MyLocalFontStyle\"&12Test Header");

                // Montrez l'effet dans la feuille de calcul
                Console.WriteLine("Header set with local font style name 'MyLocalFontStyle'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardHeaderFooterFontStyleName method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("MethodGetStandardHeaderFooterFontStyleNameDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


