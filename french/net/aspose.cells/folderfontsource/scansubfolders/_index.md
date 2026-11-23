---
title: "FolderFontSource.ScanSubFolders"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FolderFontSource. Détermine s'il faut ou non analyser les sous-dossiers"
type: docs
url: /fr/net/aspose.cells/folderfontsource/scansubfolders/
---
## FolderFontSource.ScanSubFolders property

Détermine s’il faut ou non analyser les sous‑dossiers.

```csharp
public bool ScanSubFolders { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FolderFontSourcePropertyScanSubFoldersDemo
    {
        public static void Run()
        {
            // Créer une source de police de dossier avec l'analyse des sous-dossiers activée
            string folderPath = @"C:\Windows\Fonts"; // Typical system fonts folder
            bool scanSubfolders = true;
            FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);

            // Afficher les propriétés de la source de police
            Console.WriteLine("Folder Path: " + folderFontSource.FolderPath);
            Console.WriteLine("Scan Subfolders: " + folderFontSource.ScanSubFolders);

            // Créer un classeur et définir la source de police
            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });

            // Démontrer l'utilisation en définissant du texte
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Text with fonts from folder source");

            // Enregistrez le classeur
            workbook.Save("FolderFontSourceDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [FolderFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


