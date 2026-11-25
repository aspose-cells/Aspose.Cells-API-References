---
title: "Classe FontSourceBase"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.FontSourceBase. Questa è una classe base astratta per le classi che consentono all'utente di specificare varie font source"
type: docs
url: /it/net/aspose.cells/fontsourcebase/
---
## FontSourceBase class

Questa è una classe base astratta per le classi che consentono all'utente di specificare varie origini di font.

```csharp
public abstract class FontSourceBase
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| abstract [Type](../../aspose.cells/fontsourcebase/type/) { get; } | Restituisce il tipo della fonte del font. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFontSourceBaseDemo
    {
        public static void Run()
        {
            // Crea una fonte di font da cartella
            string fontFolder = @"C:\Windows\Fonts";
            FolderFontSource folderSource = new FolderFontSource(fontFolder, true);

            // Visualizza le proprietà della fonte di font
            Console.WriteLine($"Font folder: {folderSource.FolderPath}");
            Console.WriteLine($"Scan subfolders: {folderSource.ScanSubFolders}");
            Console.WriteLine($"Source type: {folderSource.Type}");

            // Crea una cartella di lavoro e imposta la fonte del carattere
            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderSource });

            // Salva con caratteri personalizzati
            workbook.Save("OutputWithCustomFonts.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


