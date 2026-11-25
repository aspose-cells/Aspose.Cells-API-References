---
title: "FolderFontSource.FolderPath"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FolderFontSource. Percorso della cartella dei font"
type: docs
url: /it/net/aspose.cells/folderfontsource/folderpath/
---
## FolderFontSource.FolderPath property

Percorso della cartella dei font.

```csharp
public string FolderPath { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FolderFontSourcePropertyFolderPathDemo
    {
        public static void Run()
        {
            // Crea una fonte di font da cartella
            string folderPath = @"C:\Windows\Fonts"; // Typical system fonts folder
            bool scanSubfolders = true;
            FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);

            // Dimostra l'uso della proprietà FolderPath
            Console.WriteLine("Font folder path: " + folderFontSource.FolderPath);
            Console.WriteLine("Scan subfolders: " + folderFontSource.ScanSubFolders);

            // Crea una cartella di lavoro con la fonte dei font
            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });

            // Dimostrazione semplice - aggiungi testo che potrebbe usare font personalizzati
            workbook.Worksheets[0].Cells["A1"].PutValue("Font Source Demo");
            
            // Salva i risultati
            workbook.Save("FolderFontSourceDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [FolderFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


