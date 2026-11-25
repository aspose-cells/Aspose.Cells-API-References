---
title: "FolderFontSource.ScanSubFolders"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FolderFontSource. Determina se scansionare o meno le sottocartelle"
type: docs
url: /it/net/aspose.cells/folderfontsource/scansubfolders/
---
## FolderFontSource.ScanSubFolders property

Determina se eseguire o meno la scansione delle sottocartelle.

```csharp
public bool ScanSubFolders { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FolderFontSourcePropertyScanSubFoldersDemo
    {
        public static void Run()
        {
            // Crea una fonte di font da cartella con la scansione delle sottocartelle abilitata
            string folderPath = @"C:\Windows\Fonts"; // Typical system fonts folder
            bool scanSubfolders = true;
            FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);

            // Visualizza le proprietà della fonte di font
            Console.WriteLine("Folder Path: " + folderFontSource.FolderPath);
            Console.WriteLine("Scan Subfolders: " + folderFontSource.ScanSubFolders);

            // Crea una cartella di lavoro e imposta la fonte dei font
            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });

            // Dimostra l'uso impostando del testo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Text with fonts from folder source");

            // Salva la cartella di lavoro
            workbook.Save("FolderFontSourceDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [FolderFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


