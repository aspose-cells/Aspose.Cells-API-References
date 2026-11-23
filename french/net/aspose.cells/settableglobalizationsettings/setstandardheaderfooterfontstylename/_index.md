---
title: "SettableGlobalizationSettings.SetStandardHeaderFooterFontStyleName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettableGlobalizationSettings. Définit le nom de fonction dépendant de la locale selon le nom de fonction standard fourni"
type: docs
url: /fr/net/aspose.cells/settableglobalizationsettings/setstandardheaderfooterfontstylename/
---
## SettableGlobalizationSettings.SetStandardHeaderFooterFontStyleName method

Définit le nom de fonction dépendant de la langue selon le nom de fonction standard donné.

```csharp
public void SetStandardHeaderFooterFontStyleName(string localfontStyleName, string standardName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| localfontStyleName | String | Nom du style de police local pour l'en-tête/pied de page. |
| standardName | String | Nom de fonction standard (locale en-US). |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetStandardHeaderFooterFontStyleNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez les options de mise en page pour la feuille de calcul
            PageSetup pageSetup = worksheet.PageSetup;

            // Définissez un en-tête avec du texte
            pageSetup.SetHeader(0, "&\"Arial\"&12This is a header");

            // Créez une instance des paramètres de mondialisation
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

            try
            {
                // Appelez la méthode SetStandardHeaderFooterFontStyleName
                globalizationSettings.SetStandardHeaderFooterFontStyleName("Arial", "Times New Roman");

                // Appliquer les paramètres de globalisation au classeur
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                Console.WriteLine("SetStandardHeaderFooterFontStyleName method executed successfully with parameters (\"Arial\", \"Times New Roman\")");

                // L'effet sera visible lorsque le document sera rendu ou imprimé
                // Le style de police "Arial" dans les en-têtes/pieds de page sera traité comme "Times New Roman"
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetStandardHeaderFooterFontStyleName method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("MethodSetStandardHeaderFooterFontStyleNameDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


