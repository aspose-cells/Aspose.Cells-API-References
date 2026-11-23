---
title: "FolderFontSource.FolderPath"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FolderFontSource. Chemin du dossier de polices"
type: docs
url: /fr/net/aspose.cells/folderfontsource/folderpath/
---
## FolderFontSource.FolderPath property

Chemin vers le dossier des polices.

```csharp
public string FolderPath { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FolderFontSourcePropertyFolderPathDemo
    {
        public static void Run()
        {
            // Créer une source de police de dossier
            string folderPath = @"C:\Windows\Fonts"; // Typical system fonts folder
            bool scanSubfolders = true;
            FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);

            // Démontrer l'utilisation de la propriété FolderPath
            Console.WriteLine("Font folder path: " + folderFontSource.FolderPath);
            Console.WriteLine("Scan subfolders: " + folderFontSource.ScanSubFolders);

            // Créer un classeur avec la source de police
            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });

            // Démo simple - ajouter du texte qui pourrait utiliser des polices personnalisées
            workbook.Worksheets[0].Cells["A1"].PutValue("Font Source Demo");
            
            // Enregistrer les sorties
            workbook.Save("FolderFontSourceDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [FolderFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


