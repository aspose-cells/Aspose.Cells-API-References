---
title: "Classe MemoryFontSource"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.MemoryFontSource. Représente le fichier de police TrueType unique stocké en mémoire"
type: docs
url: /fr/net/aspose.cells/memoryfontsource/
---
## MemoryFontSource class

Représente le fichier de police TrueType unique stocké en mémoire.

```csharp
public class MemoryFontSource : FontSourceBase
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [MemoryFontSource](memoryfontsource/)(byte[]) | Constructeur. |

## Propriétés

| Nom | Description |
| --- | --- |
| [FontData](../../aspose.cells/memoryfontsource/fontdata/) { get; } | Données de police binaires. |
| override [Type](../../aspose.cells/memoryfontsource/type/) { get; } | Renvoie le type de la source de police. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsClassMemoryFontSourceDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Chargez un fichier de police TrueType en mémoire
            byte[] fontData = File.ReadAllBytes("arial.ttf");

            // Créez une instance de MemoryFontSource avec les données de police
            MemoryFontSource memoryFontSource = new MemoryFontSource(fontData);

            // Créez un tableau de sources de police contenant notre source de police en mémoire
            FontSourceBase[] fontSources = new FontSourceBase[] { memoryFontSource };

            // Définissez les sources de police en utilisant FontConfigs
            FontConfigs.SetFontSources(fontSources);

            // Utilisez la police personnalisée dans une cellule
            worksheet.Cells["A1"].PutValue("Text with custom font from memory");
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            worksheet.Cells["A1"].SetStyle(style);

            // Enregistrez le classeur
            workbook.Save("MemoryFontSourceDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [FontSourceBase](../fontsourcebase/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


