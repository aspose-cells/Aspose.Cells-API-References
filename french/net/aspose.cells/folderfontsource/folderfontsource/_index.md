---
title: "FolderFontSource.FolderFontSource"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur de FolderFontSource. Ctor"
type: docs
url: /fr/net/aspose.cells/folderfontsource/folderfontsource/
---
## FolderFontSource constructor

Constructeur.

```csharp
public FolderFontSource(string folderPath, bool scanSubfolders)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| folderPath | String | chemin du dossier de polices |
| scanSubfolders | Boolean | Détermine s'il faut ou non analyser les sous-dossiers. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FolderFontSourceMethodCtorWithStringBooleanDemo
    {
        public static void Run()
        {
            string folderPath = @"C:\Fonts";
            bool scanSubfolders = true;
            FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);

            Console.WriteLine("Folder Path: " + folderFontSource.FolderPath);
            Console.WriteLine("Scan Subfolders: " + folderFontSource.ScanSubFolders);

            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });
            workbook.Save("FolderFontSourceExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [FolderFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


