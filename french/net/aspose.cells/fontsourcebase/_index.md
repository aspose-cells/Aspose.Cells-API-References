---
title: "Classe FontSourceBase"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.FontSourceBase. Il s'agit d'une classe de base abstraite pour les classes qui permettent à l'utilisateur de spécifier diverses sources de police"
type: docs
url: /fr/net/aspose.cells/fontsourcebase/
---
## FontSourceBase class

Il s'agit d'une classe de base abstraite pour les classes qui permettent à l'utilisateur de spécifier diverses sources de police

```csharp
public abstract class FontSourceBase
```

## Propriétés

| Nom | Description |
| --- | --- |
| abstract [Type](../../aspose.cells/fontsourcebase/type/) { get; } | Renvoie le type de la source de police. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFontSourceBaseDemo
    {
        public static void Run()
        {
            // Créer une source de police de dossier
            string fontFolder = @"C:\Windows\Fonts";
            FolderFontSource folderSource = new FolderFontSource(fontFolder, true);

            // Afficher les propriétés de la source de police
            Console.WriteLine($"Font folder: {folderSource.FolderPath}");
            Console.WriteLine($"Scan subfolders: {folderSource.ScanSubFolders}");
            Console.WriteLine($"Source type: {folderSource.Type}");

            // Créer un classeur et définir la source de police
            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderSource });

            // Enregistrer avec des polices personnalisées
            workbook.Save("OutputWithCustomFonts.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


