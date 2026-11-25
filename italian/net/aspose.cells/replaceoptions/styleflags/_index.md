---
title: "ReplaceOptions.StyleFlags"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ReplaceOptions proprietà. Ottiene e imposta i flag per l'applicazione delle impostazioni del carattere"
type: docs
url: /it/net/aspose.cells/replaceoptions/styleflags/
---
## ReplaceOptions.StyleFlags property

Ottiene e imposta i flag per l'applicazione delle impostazioni del carattere.

```csharp
public StyleFlag[] StyleFlags { get; set; }
```

### Esempi

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
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi testo di esempio alla cella
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("test text");

            // Crea opzioni di sostituzione
            ReplaceOptions options = new ReplaceOptions();
            options.MatchEntireCellContents = false;
            options.CaseSensitive = false;

            // Crea impostazione del carattere e flag di stile
            string replacementText = "new text";
            FontSetting setting = new FontSetting(0, replacementText.Length, workbook.Worksheets);
            StyleFlag styleFlag = new StyleFlag();
            
            // Configura carattere e stile
            setting.Font.Color = Color.Red;
            setting.Font.Underline = FontUnderlineType.Single;
            styleFlag.FontColor = true;
            styleFlag.FontUnderline = true;

            // Applica impostazioni alle opzioni
            options.FontSettings = new FontSetting[] { setting };
            options.StyleFlags = new StyleFlag[] { styleFlag };

            // Esegui la sostituzione
            workbook.Replace("test", replacementText, options);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [StyleFlag](../../styleflag/)
* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


