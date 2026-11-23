---
title: "ReplaceOptions.FontSettings"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ReplaceOptions. Les paramètres formatés riches pour le texte remplacé"
type: docs
url: /fr/net/aspose.cells/replaceoptions/fontsettings/
---
## ReplaceOptions.FontSettings property

Les paramètres richement formatés pour le texte remplacé.

```csharp
public FontSetting[] FontSettings { get; set; }
```

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReplaceOptionsPropertyFontSettingsDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définissez le texte d’exemple dans la cellule A1
            worksheet.Cells["A1"].Value = "Sample text for replacement";
            
            // Créer des options de remplacement avec les paramètres de police
            ReplaceOptions options = new ReplaceOptions();
            options.MatchEntireCellContents = false;
            
            // Créer un paramètre de police pour le texte de remplacement
            FontSetting fontSetting = new FontSetting(0, 8, workbook.Worksheets);
            fontSetting.Font.IsBold = true;
            fontSetting.Font.Color = Color.Blue;
            
            // Appliquer les paramètres de police aux options de remplacement
            options.FontSettings = new FontSetting[] { fontSetting };
            
            // Effectuer le remplacement
            workbook.Replace("text", "REPLACED", options);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [FontSetting](../../fontsetting/)
* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


