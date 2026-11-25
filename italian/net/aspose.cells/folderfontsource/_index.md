---
title: "Class FolderFontSource"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.FolderFontSource class. Rappresenta la cartella che contiene i file di font TrueType"
type: docs
url: /it/net/aspose.cells/folderfontsource/
---
## FolderFontSource class

Rappresenta la cartella che contiene i file di font TrueType.

```csharp
public class FolderFontSource : FontSourceBase
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [FolderFontSource](folderfontsource/)(string, bool) | Ctor. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [FolderPath](../../aspose.cells/folderfontsource/folderpath/) { get; } | Percorso della cartella dei font. |
| [ScanSubFolders](../../aspose.cells/folderfontsource/scansubfolders/) { get; } | Determina se eseguire o meno la scansione delle sottocartelle. |
| override [Type](../../aspose.cells/folderfontsource/type/) { get; } | Restituisce il tipo della fonte del font. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FolderFontSourceDemo
    {
        public static void FolderFontSourceExample()
        {
            // Crea un'istanza di FolderFontSource
            string folderPath = @"C:\Fonts";
            bool scanSubfolders = true;
            FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);

            // Accesso alle proprietà
            Console.WriteLine("Folder Path: " + folderFontSource.FolderPath);
            Console.WriteLine("Scan Subfolders: " + folderFontSource.ScanSubFolders);
            Console.WriteLine("Font Source Type: " + folderFontSource.Type);

            // Crea un workbook e imposta le font sources
            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });

            // Salva la cartella di lavoro
            workbook.Save("FolderFontSourceExample.xlsx");
            workbook.Save("FolderFontSourceExample.pdf");
            return;
        }
    }
}
```

### Vedi anche

* class [FontSourceBase](../fontsourcebase/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


