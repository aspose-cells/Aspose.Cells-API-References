---
title: "ReplaceOptions.FontSettings"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ReplaceOptions. Le impostazioni formattate riccamente per il testo sostituito"
type: docs
url: /it/net/aspose.cells/replaceoptions/fontsettings/
---
## ReplaceOptions.FontSettings property

Le impostazioni di formattazione ricca per il testo sostituito.

```csharp
public FontSetting[] FontSettings { get; set; }
```

### Esempi

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
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta testo di esempio nella cella A1
            worksheet.Cells["A1"].Value = "Sample text for replacement";
            
            // Crea le opzioni di sostituzione con impostazioni di carattere
            ReplaceOptions options = new ReplaceOptions();
            options.MatchEntireCellContents = false;
            
            // Crea l'impostazione del carattere per il testo di sostituzione
            FontSetting fontSetting = new FontSetting(0, 8, workbook.Worksheets);
            fontSetting.Font.IsBold = true;
            fontSetting.Font.Color = Color.Blue;
            
            // Applica le impostazioni del carattere alle opzioni di sostituzione
            options.FontSettings = new FontSetting[] { fontSetting };
            
            // Esegui la sostituzione
            workbook.Replace("text", "REPLACED", options);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [FontSetting](../../fontsetting/)
* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


