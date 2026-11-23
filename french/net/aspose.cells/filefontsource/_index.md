---
title: "Classe FileFontSource"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.FileFontSource. Représente le fichier de police TrueType unique stocké dans le système de fichiers"
type: docs
url: /fr/net/aspose.cells/filefontsource/
---
## FileFontSource class

Représente le fichier de police TrueType unique stocké dans le système de fichiers.

```csharp
public class FileFontSource : FontSourceBase
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [FileFontSource](filefontsource/)(string) | Constructeur. |

## Propriétés

| Nom | Description |
| --- | --- |
| [FilePath](../../aspose.cells/filefontsource/filepath/) { get; } | Chemin du fichier de police. |
| override [Type](../../aspose.cells/filefontsource/type/) { get; } | Renvoie le type de la source de police. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FileFontSourceDemo
    {
        public static void FileFontSourceExample()
        {
            // Spécifiez le chemin du fichier de police TrueType
            string fontFilePath = "C:\\Fonts\\CustomFont.ttf";

            // Créer une instance de FileFontSource
            FileFontSource fontSource = new FileFontSource(fontFilePath);

            // Afficher le type de source de police et le chemin du fichier
            Console.WriteLine("Font Source Type: " + fontSource.Type);
            Console.WriteLine("Font File Path: " + fontSource.FilePath);

            // Créer un objet Workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Définir une valeur de cellule
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Hello, Aspose!");

            // Appliquer la police personnalisée à la cellule
            Style style = cell.GetStyle();
            style.Font.Name = "CustomFont"; // Use the name of the font
            cell.SetStyle(style);

            // Enregistrez le classeur
            workbook.Save("FileFontSourceExample.xlsx");
            workbook.Save("FileFontSourceExample.pdf");
        }
    }
}
```

### Voir aussi

* class [FontSourceBase](../fontsourcebase/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


