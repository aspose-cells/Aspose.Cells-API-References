---
title: "Class FolderFontSource"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.FolderFontSource class. Représente le dossier contenant les fichiers de polices TrueType"
type: docs
url: /fr/net/aspose.cells/folderfontsource/
---
## FolderFontSource class

Représente le dossier contenant les fichiers de polices TrueType.

```csharp
public class FolderFontSource : FontSourceBase
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [FolderFontSource](folderfontsource/)(string, bool) | Constructeur. |

## Propriétés

| Nom | Description |
| --- | --- |
| [FolderPath](../../aspose.cells/folderfontsource/folderpath/) { get; } | Chemin vers le dossier des polices. |
| [ScanSubFolders](../../aspose.cells/folderfontsource/scansubfolders/) { get; } | Détermine s’il faut ou non analyser les sous‑dossiers. |
| override [Type](../../aspose.cells/folderfontsource/type/) { get; } | Renvoie le type de la source de police. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FolderFontSourceDemo
    {
        public static void FolderFontSourceExample()
        {
            // Créez une instance de FolderFontSource
            string folderPath = @"C:\Fonts";
            bool scanSubfolders = true;
            FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);

            // Accès aux propriétés
            Console.WriteLine("Folder Path: " + folderFontSource.FolderPath);
            Console.WriteLine("Scan Subfolders: " + folderFontSource.ScanSubFolders);
            Console.WriteLine("Font Source Type: " + folderFontSource.Type);

            // Créez un classeur et définissez les sources de police
            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });

            // Enregistrez le classeur
            workbook.Save("FolderFontSourceExample.xlsx");
            workbook.Save("FolderFontSourceExample.pdf");
            return;
        }
    }
}
```

### Voir aussi

* class [FontSourceBase](../fontsourcebase/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


