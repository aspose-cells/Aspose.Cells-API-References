---
title: "ReplaceOptions.StyleFlags"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ReplaceOptions. Obtient et définit les indicateurs d'application des paramètres de police"
type: docs
url: /fr/net/aspose.cells/replaceoptions/styleflags/
---
## ReplaceOptions.StyleFlags property

Obtient et définit les indicateurs d'application des paramètres de police.

```csharp
public StyleFlag[] StyleFlags { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ReplaceOptionsPropertyStyleFlagsDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter du texte d'exemple à la cellule
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("test text");

            // Créer des options de remplacement
            ReplaceOptions options = new ReplaceOptions();
            options.MatchEntireCellContents = false;
            options.CaseSensitive = false;

            // Créer un paramètre de police et un indicateur de style
            string replacementText = "new text";
            FontSetting setting = new FontSetting(0, replacementText.Length, workbook.Worksheets);
            StyleFlag styleFlag = new StyleFlag();
            
            // Configurer la police et le style
            setting.Font.Color = Color.Red;
            setting.Font.Underline = FontUnderlineType.Single;
            styleFlag.FontColor = true;
            styleFlag.FontUnderline = true;

            // Appliquer les paramètres aux options
            options.FontSettings = new FontSetting[] { setting };
            options.StyleFlags = new StyleFlag[] { styleFlag };

            // Effectuer le remplacement
            workbook.Replace("test", replacementText, options);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [StyleFlag](../../styleflag/)
* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


